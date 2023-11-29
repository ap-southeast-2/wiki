# CISSP RAID

## RAID 0-10

| RAID | Description | Fault tolerance | Min storage disks |
|-|-|-|-|
| RAID 0 = Block striping | Block-level striping where a data set is striped (split) evenly across the disks. | The failure of any storage disk in the set will result in data loss. | 2 |
| RAID 1 = Mirroring | An exact mirror (copy) of a data set on all disks. | RAID 1 can survive 1x storage disk failure without data loss. | 2 |
| RAID 2 = Bit striping + Hamming code | Bit-level striping with Hamming code for error correction. Rarely used. | | 3 |
| RAID 3 = Byte striping + dedicated parity | Byte-level striping with a dedicated parity storage disk. Rarely used. | RAID 3 can survive 1x storage failure. | 3 |
| RAID 4 = Block striping + dedicated parity | Block-level striping with a dedicated parity storage disk. | RAID 4 can survive 1x storage disk failure. | 3 |
| RAID 5 = Block striping + distributed parity | Block-level striping with distributed parity, where parity data is distributed among the storage disks. | RAID 5 can survive 1x storage disk failure. | 3 |
| RAID 6 = Block striping + double parity | Block-level striping with double distributed parity, where two parity blocks are distributed across all storage disks. | RAID 6 can survive 2x storage disk failure. | 4 |
| RAID 01 = Mirror of stripes | A mirror (RAID 1) of block-level striped storage disks (RAID 0). No parity. | | 4 |
| RAID 10 = Mirroring with striping inside | Block-level striping (RAID 1) among mirrored storage disks (RAID 0). No parity. | | 4 |

## RAID terms
- Striping: Data is split across multiple storage disks.
- Mirroring: Data is copied between multiple storage disks.
- Parity: Used to recreate data in the event of a storage disk failure.

## RAID links
https://en.wikipedia.org/wiki/Standard_RAID_levels
https://en.wikipedia.org/wiki/Nested_RAID_levels
https://www.snia.org/education/online-dictionary/R

