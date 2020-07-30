### 2F02-zfs-controller-high-availability

#### Description

This test deploys the zfs-controller in high availability (more than one replica) and checks the behaviour of zfs-localpv when one of the replica is down.

#### steps involved

- First deploy the zfs-controller with single replica
- Then scale the replicas of zfs-controller statefulset and verify the provision of volume when other replica is down.
- For more detailed README for the test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfs-controller-high-availability)

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|