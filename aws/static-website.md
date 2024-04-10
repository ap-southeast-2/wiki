# How to setup a static website in AWS

In this article I wanted to group together the relevant articles required to setup a static website in AWS, using nothing but AWS cloud services. Unfortunately, there are a lot of AWS articles that are now out of date or fail to cover off more than the basic functionality.

## Initial setup

Follow this article that describes the main legwork involved in getting a domain (Route 53), requesting a certificate (ACM), HTML file storage (S3 Buckets), and CDN (CloudFront).
- [Use an Amazon CloudFront distribution to serve a static website](https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/getting-started-cloudfront-overview.html)

Different from instructions elsewhere, the S3 Buckets are never made public. Instead, they require policy (S3 Bucket) for the CDN (CloudFront) to access the HTML file storage (S3 Buckets).

At the end of the steps, you should be able to access either:
- [example.com/index.html](https://example.com/index.html)
- [example.cloudfront.net/index.html](https://example.cloudfront.net/index.html)


## 403 error

The examples above referred to the index.html file. Requests to just example.com will result in a 403 error. Redirection requires the use of CloudFront Functions, using a piece of JavaScript.

- [Introducing CloudFront Functions – Run Your Code at the Edge with Low Latency at Any Scale](https://aws.amazon.com/blogs/aws/introducing-cloudfront-functions-run-your-code-at-the-edge-with-low-latency-at-any-scale/)
- [Redirect to index.html for S3 subfolder](https://stackoverflow.com/questions/49082709/redirect-to-index-html-for-s3-subfolder)

		function handler(event) {
			var request = event.request;

			if (request.uri !== "/" && (request.uri.endsWith("/") || request.uri.lastIndexOf(".") < request.uri.lastIndexOf("/"))) {
				if (request.uri.endsWith("/")) {
					request.uri = request.uri.concat("index.html");
				} else {
					request.uri = request.uri.concat("/index.html");
				}
			}
			return request;
		}



Hope this helps,
Matt
