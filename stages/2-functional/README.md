### Goal of this stage

The goal of this gitlab stage is to test functional tests of zfs-localpv features. This includes provisioning for zfs-localpv components, volume provisioning / deprovisioning, snapshot and clone, volume resize etc.

#### List of test cases in this stage

| TCID  |                Test case description                                                    |
|-------| --------------------------------------------------------------------------------------- |
| 2F01  | Install zfs-localpv components which includes zfs-controller and csi node-agent daemonset  |
| 2F02  | Install zfs-controller in high availability                                             |
| 2F03  | Provision of zfs-volume only on selected nodes using custom-topology support via storage-class|
| 2F04  | Provision of zfs-localpv for raw block volumes support                                  |
| 2F05  | Resize of zfs volume when application is deployed with zfs file system                  |
| 2F06  | Resize of zfs volume when application is deployed with ext4 file system                 |
| 2F07  | Resize of zfs volume when application is deployed with xfs file system                  |
| 2F08  | Modification of zfspv properties after provisioning the volume, when fstype is zfs      |
| 2F09  | Modification of zfspv properties after provisioning the volume, when fstype is ext4     |
| 2F10  | Modification of zfspv properties after provisioning the volume, when fstype is xfs      |
| 2F11  | Modification of zfspv properties after provisioning the volume, when fstype is btrfs    |
| 2F12  | Creation of volume snapshot and clone, when fstype is zfs                               |
| 2F13  | Creation of volume snapshot and clone, when fstype is ext4                              |
| 2F14  | Creation of volume snapshot and clone, when fstype is xfs                               |
| 2F15  | Creation of volume snapshot and clone, when fstype is btrfs                             |