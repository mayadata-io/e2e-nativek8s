### Goal of this stage

The goal of this gitlab stage is to test functional tests of zfs-localpv features. This includes provisioning for zfs-localpv components, volume provisioning / deprovisioning, snapshot and clone, volume resize etc.

#### List of test cases in this stage

| TCID  |                Test case description                                                    |
|-------| --------------------------------------------------------------------------------------- |
| 3F01  | Provision of zfs-volume only on selected nodes using custom-topology support via storage-class|
| 3F02  | Provision of zfs-localpv for raw block volumes support                                  |
| 3F03  | Resize of zfs volume when application is deployed with zfs file system                  |
| 3F04  | Resize of zfs volume when application is deployed with ext4 file system                 |
| 3F05  | Resize of zfs volume when application is deployed with xfs file system                  |
| 3F06  | Modification of zfspv properties after provisioning the volume, when fstype is zfs      |
| 3F07  | Modification of zfspv properties after provisioning the volume, when fstype is ext4     |
| 3F08  | Modification of zfspv properties after provisioning the volume, when fstype is xfs      |
| 3F09  | Modification of zfspv properties after provisioning the volume, when fstype is btrfs    |
| 3F10  | Creation of volume snapshot and clone, when fstype is zfs                               |
| 3F11  | Creation of volume snapshot and clone, when fstype is ext4                              |
| 3F12  | Creation of volume snapshot and clone, when fstype is xfs                               |
| 3F13  | Creation of volume snapshot and clone, when fstype is btrfs                             |
| 3F14  | Shared mount support for zfspv, when fstype is zfs                                      |
| 3F15  | Shared mount support for zfspv, when fstype is ext4                                     |
| 3F16  | Shared mount support for zfspv, when fstype is xfs                                      |
| 3F17  | Shared mount support for zfspv, when fstype is btrfs                                    |