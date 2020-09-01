### Goal of this stage

The goal of this gitlab stage is to induce chaos on kubernetes infrastructure and check the behaviour of zfs-localpv components, application pods and its persistent volume.

### List of test cases in this stage

| TCID  |                Test case description                                                    |
|-------| --------------------------------------------------------------------------------------- |
| 5I01  | Restart the docker services on application node and check the behaviour of zfs-localpv  |
| 5I02  | Restart the kubelet services on application node and check the behaviour of zfs-localpv |
| 5I03  | Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv |
 