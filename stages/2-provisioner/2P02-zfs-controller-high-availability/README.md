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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256963">256963</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 31 13:25:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256766">256766</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 31 09:38:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256743">256743</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Mon Aug 31 06:57:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254798">254798</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 21 16:31:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253788">253788</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Wed Aug 19 16:00:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253173">253173</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Sun Aug 16 12:31:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252954">252954</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Sat Aug 15 23:45:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252929">252929</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Sat Aug 15 19:42:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252558">252558</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Sat Aug 15 10:31:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251939">251939</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 14 21:15:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251855">251855</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 14 20:28:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251833">251833</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 14 19:40:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251561">251561</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 14 11:42:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251537">251537</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Fri Aug 14 10:48:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250265">250265</a>           |  Deploy zfs-localpv controller statefulset in high availability           | Thu Aug 13 10:37:40 IST 2020  | Pass |
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
