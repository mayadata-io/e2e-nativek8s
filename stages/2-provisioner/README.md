### Goal of this stage

The goal of this gitlab stage is to deploy the zfs-localpv provisioiner. This includes provisioning for zfs-localpv components, zfs-controller in high availability and required various storage classes for dynamic provisioning of zfs-local peristent volumes.

#### List of test cases in this stage

| TCID  |                Test case description                                                    |
|-------| --------------------------------------------------------------------------------------- |
| 2P01  | Provision the zfs-localpv driver                                                        |
| 2P02  | Deploy zfs-localpv controller statefulset in high availability                          |
