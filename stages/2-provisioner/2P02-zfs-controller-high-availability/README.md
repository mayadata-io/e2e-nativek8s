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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249600">249600</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 12 21:45:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249485">249485</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 12 19:35:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249401">249401</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 12 17:20:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249119">249119</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 12 11:54:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249096">249096</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 12 10:37:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248762">248762</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Tue Aug 11 17:44:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248256">248256</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Tue Aug 11 10:21:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248203">248203</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Tue Aug 11 09:30:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247056">247056</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 10 17:48:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246951">246951</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 10 17:03:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246904">246904</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 10 15:35:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246882">246882</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 10 14:17:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245459">245459</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug  7 21:20:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245354">245354</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug  7 19:26:32 IST 2020  | Pass |
