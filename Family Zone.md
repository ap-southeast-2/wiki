# Family Zone - Initial Security Assessment - Android Mobile App

## Introduction

We were asked by a client based in Australia / New Zealand to perform an initial security assessment of Family Zone. The client's child was asked by their school to install the Kids version of the Android mobile app. The items above are in scope for the initial security assessment.

The Family Zone mobile app can also be installed onto Apple devices. The client would install the Parent version of the Family Zone mobile app to manage screen time, get alerts, view reports, and more. Family Zone also offers the Family Zone Appliance for schools to control the network while students are at school. The items above are out of scope for the initial security assessment.

Family Zone has the following web sites:
- familyzone.io in the United States.
- familyzone.com/nz in New Zealand.
- familyzone.com/au in Australia.

We hope this helps,
ap-southeast-2

## Summary
1. The Family Zone mobile app captures multiple types of data that includes the child's location and locale, and their internet usage on the child's Android mobile device. The Apple mobile app also includes detailed information about the device and other apps on the child's Apple mobile device. There is an option to disable or opt-out of some types of data, there are exceptions that cannot be disabled.

2. The Android permissions required by the Google Play Store grant the Family Zone mobile app access to detailed information about the device and other apps on the child's Android mobile device, as well as access to USB storage, camera, photos/media/files, available wifi and network connections, and Bluetooth settings and pairings.

3. Data may be transferred to countries outside of Australia and New Zealand as part of the service. In legal terms, the child's data will not be protected by the Australian and New Zealand Privacy Acts. 

4. The Family Zone service is delivered using Amazon, Conexim and other third parties used in the processing of data. Introducing more third parties increases the likelihood that the child's data will be exposed by one of the third parties, for example through accidental mishandling or through a security breach (ie. "hacked").

5. Out of Family Zone, Amazon, Conexim, and the third parties used to deliver the Family Zone service, we are only able to evidence that Amazon adheres to internationally rocognised security standards, including ISO/IEC 27001 and SOC 2 Type 2.

6. There is no firm data retention policy specified in days, such as "all of the child's data is deleted after 30 days". It is unclear whether "de-identifying" means just removing the account details, or whether it also mean removing the child's location and locale, and their internet usage, detailed device information, USB storage, camera, photos/media/files, available wifi and network connections, and Bluetooth settings and pairing.

## 1. Types of Data Collected About The Child 

Sub-section '1.2 Our Privacy Policy' and section '3. The Information We Collect' outline the various types of data that are collected by Family Zone. This includes account and address details, support and survey information, along with cookies and web analytics (metadata). The Family Zone Privacy Policy states that credit card payments are handled by a separate company that is a compliant payment gateway.

Together, the different types of data described above represent the risk impact for the subsequent risks described below. This gives us the answer to the question "what is the worst that could happen?" This includes exposing the child's location and locale, and their internet usage. 

Section '2. Privacy & Mobile Device Management' states the use of Apple Mobile Device Management (MDM), stating "We use Apple Mobile Device Management (MDM) for some of our Services" and "Scanning Apple devices for new Apps so we can notify you". MDM is used to access to detailed information about the child's device and other apps on the child's Apple mobile device.

There is an option to disable or opt-out of some types of data. Exceptions that cannot be disabled include:
- Mobile Apps - Use of applications, including what applications are installed or attempted to be installed, are used and for how long, are blocked or permitted to be used, and related information such as device details, time and date.
- Transactional - Our Products log certain transactions for the purpose of notifying and reporting system events. 

Refer to:
- ['Legal Documents - Privacy Policy' section 'Family Zone Privacy Policy'](https://www.familyzone.com/anz/legal)


## 2. Additional Android Permissions

Sub-section '1.2 Our Privacy Policy' and '2.1 Apple Mobile Device Management', and section '3. The Information We Collect' outline the various types of data that are collected by Family Zone, including this statement:

> 3. Does Family Zone access personal data on devices?
> No. The only data the App needs is device identifiers eg MAC, IMEI, UID and App IDs (ie the codes of the apps installed on the device).
> We absolutely do not access photos, contacts, messages etc.

However, the permissions required by the Android mobile app in the Google Play Store give the mobile app permissions that do not seem to be explicitly stated in the Family Zone Privacy Policy. The full list of privileges described in Appendx A (see below) augment the answer to the question "what is the worst that could happen?"

Section '2. Privacy & Mobile Device Management' states the use of Apple Mobile Device Management (MDM) used to deliver some parts of the Family Zone service on Apple devices. However, the following Android permissions are required:

> Device ID & call information
> - read phone status and identity
> Device & app history
> - retrieve running apps
> Phone
> - read phone status and identity

The 'Customer Detail & Security' section '3. Does Family Zone access personal data on devices?' explicitly states that "We absolutely do not access photos, contacts, messages etc." but the Android permissions include:

> Storage
> - modify or delete the contents of your USB storage
> - read the contents of your USB storage
> Camera
> - take pictures and videos
> Photos/Media/Files
> - modify or delete the contents of your USB storage
> - read the contents of your USB storage

The following Android permissions are not explicitly stated in the Family Zone Privacy Policy:

> Wi-Fi connection information
> - view Wi-Fi connections
> Other
> - pair with Bluetooth devices
> - view network connections
> - access Bluetooth settings
> - prevent device from sleeping

Refer to:
- Appendix A - Mobile Zone for Child Devices Permissions
- [Customer Detail & Security](https://www.familyzone.com/anz/legal)
- [Android mobile app in the Google Play Store permissions](https://play.google.com/store/apps/details?id=au.com.familyzone)
- ['Legal Documents - Privacy Policy' section 'Family Zone Privacy Policy'](https://www.familyzone.com/anz/legal)

## 3. Data Outside of Australia & New Zealand

Sub-section '6.2 International Privacy' describes how data may be transferred to countries outside of Australia and New Zealand as part of the service. In legal terms, the data will not be protected by the Australian and New Zealand Privacy Acts, but the Family Zone Privacy Policy states that "we agree to take reasonable steps to ensure they use and manage it in a manner consistent with this policy".

Refer to:
- ['Legal Documents - Privacy Policy' section 'Family Zone Privacy Policy'](https://www.familyzone.com/anz/legal)

## 4. Third Parties

Section 1. of the 'Customer Detail & Security' mentions two third parties explicitly:

> 1. Can 3rd parties access Family Zone to identify kids' usage?
> Our cloud servers are hosted by Amazon and we engage leading provider Conexim to manage the services and security.

Amazon is the cloud hosting provider and Conexim is the service management provider. 

Sub-section 6.2 of the Family Zone Privacy Policy describes other third parties used in the processing of data. 

Introducing more third parties increases the likelihood that the child's data will be exposed by one of the third parties, for example through accidental mishandling or through a security breach (ie. "hacked"). 

Refer to:
- ['Legal Documents - Privacy Policy' section 'Family Zone Privacy Policy'](https://www.familyzone.com/anz/legal)

## 5. Internationally Recognised Security Standards

Section 1. of the 'Customer Detail & Security' states three security features:

> We use HTTPS for all incoming/outgoing data transfer
> Our User Interface only provides access to this data to Zone (ie network) Owners and CSRs/Admins.
> We apply all industry security standards. All servers are firewalled and require security certificates and strong passwords. There is no direct or password only access to production servers.

The use of HTTPS protects data as it moves across the Internet, privileges are used to limit access, and industry security standards are applied. However, applying standards is different from being able to evidence that the Family Zone service consistently adheres to internationally rocognised security standards on an annual basis (eg. ISO/IEC 27001) or on-going basis (eg. SOC 2 Type 2).

Of Family Zone, the cloud hosting provider, service management provider, and other third parties used to deliver the Family Zone service, only Amazon is able to evidence that it adheres to internationally rocognised security standards, including ISO/IEC 27001 and SOC 2 Type 2.

Refer to:
- [Customer Detail & Security](https://www.familyzone.com/anz/legal)

## 6. No Clear Deletion Date

Sub-section '3.8 End User Cyber Safety Data' includes this statement regarding data retention:
> We will hold this information as long as reasonably necessary. This is typically 30 days after which time we will de-identify it. You can access this information directly through your Account.
Sub-section '6.6 How long we keep information' contains this statement:
> Notwithstanding the foregoing, Personally Identifiable Information stored by us relating to End Users under the age of 18 will be deleted in all cases (to the extent that it is reasonably and commercially possible to do so) when it is no longer needed for the purpose for which it was collected.
There is no firm retention policy specified in days, such as "all of the child's data is deleted after 30 days".

It is unclear whether "de-identifying" means removing all the following types of the child's data:
- The account details, the child's location and locale, and their internet usage.
- Detailed information about the device and other apps on the child's mobile device.
- USB storage, camera, photos/media/files, available wifi and network connections, Bluetooth settings and pairing.

Refer to:
- ['Legal Documents - Privacy Policy' section 'Family Zone Privacy Policy'](https://www.familyzone.com/anz/legal)

## Appendix A - Mobile Zone for Child Devices Permissions

We looked at Family Zone:
- Kids version 2.5.2, updated April 17, 2020.

FAMILY ZONE CYBER SAFETY LIMITED
Showing permissions for all versions of this app

This app has access to:
Device ID & call information
- read phone status and identity

Device & app history
- retrieve running apps

Storage
- modify or delete the contents of your USB storage
- read the contents of your USB storage

Camera
- take pictures and videos

Location
- precise location (GPS and network-based)
- approximate location (network-based)

Photos/Media/Files
- modify or delete the contents of your USB storage
- read the contents of your USB storage

Phone
- read phone status and identity

Wi-Fi connection information
- view Wi-Fi connections

Other
- add or remove a device admin
- update component usage statistics
- receive data from Internet
- connect and disconnect from Wi-Fi
- full network access
- pair with Bluetooth devices
- close other apps
- change network connectivity
- view network connections
- access Bluetooth settings
- prevent device from sleeping
- draw over other apps
- run at startup
