### 2P02-zfs-controller-high-availability

#### Description

This test deploys the zfs-controller in high availability (more than one replica) and checks the behaviour of zfs-localpv when one of the replica is down.

#### steps involved

- First deploy the zfs-controller with single replica
- Then scale the replicas of zfs-controller statefulset and verify the provision of volume when other replica is down.
- For more detailed README for the test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-controller-high-availability)

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245286">245286</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug  7 15:11:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245264">245264</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug  7 14:12:40 IST 2020  | Pass |