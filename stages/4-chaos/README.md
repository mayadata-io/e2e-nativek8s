### Goal of this stage

The goal for this gitlab stage is to induce chaos into zfs-localpv components, zpool, application using localpv and other resources and verify the behaviour of zfs-localpv. The system in state should be capable to withstand in any turbulent condition in production.

### List of test cases in this stage

| TCID  |                 Test case description                                        |
|-------|------------------------------------------------------------------------------|
| 4C01  | Kill the application pod container when fstype is zfs                        |
| 4C02  | Kill the application pod container when fstype is xfs                        |
| 4C03  | Kill the application pod container when fstype is ext4                       |