### 3F10-zfspv-snapshot-clone-zfs-create

#### Description

This test takes the zfs volume snapshot and later use that snapshot to create clone volumes when application is deployed with zfs file-system on top of zfs-localpv.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the test for creating the volume snapshot after dumping some data into the application mount point. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
4. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different `percona-mysql` application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
5. Deprovision the clone volume and its application.
6. Delete the volume snapshot.
7. Deprovision the application and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263020">263020</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Sep 14 12:45:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260593">260593</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Sep 11 09:09:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260180">260180</a>           |  create volume snapshot and clone when fstype is zfs           | Thu Sep 10 21:33:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260060">260060</a>           |  create volume snapshot and clone when fstype is zfs           | Thu Sep 10 20:01:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258066">258066</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Sep  8 11:39:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257840">257840</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Sep  7 18:09:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257562">257562</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Sep  4 15:56:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257536">257536</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Sep  4 12:00:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257342">257342</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Sep  2 16:14:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257316">257316</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Sep  2 13:40:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257290">257290</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Sep  2 10:20:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257181">257181</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Sep  1 20:21:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257155">257155</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Sep  1 19:13:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257128">257128</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Sep  1 13:07:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257103">257103</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Sep  1 12:02:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256995">256995</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 31 21:15:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256973">256973</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 31 13:28:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256776">256776</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 31 09:41:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256753">256753</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 31 06:57:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254808">254808</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 21 16:35:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253798">253798</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 19 16:00:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253183">253183</a>           |  create volume snapshot and clone when fstype is zfs           | Sun Aug 16 12:34:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252964">252964</a>           |  create volume snapshot and clone when fstype is zfs           | Sat Aug 15 23:48:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252939">252939</a>           |  create volume snapshot and clone when fstype is zfs           | Sat Aug 15 19:46:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252568">252568</a>           |  create volume snapshot and clone when fstype is zfs           | Sat Aug 15 10:34:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251949">251949</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 14 21:18:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251865">251865</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 14 20:31:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251843">251843</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251571">251571</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 14 11:45:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251547">251547</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug 14 10:51:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250275">250275</a>           |  create volume snapshot and clone when fstype is zfs           | Thu Aug 13 10:40:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249610">249610</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 12 21:48:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249495">249495</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 12 19:38:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249411">249411</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 12 17:23:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249129">249129</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 12 11:57:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249106">249106</a>           |  create volume snapshot and clone when fstype is zfs           | Wed Aug 12 10:40:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248772">248772</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Aug 11 17:47:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248266">248266</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Aug 11 10:24:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248213">248213</a>           |  create volume snapshot and clone when fstype is zfs           | Tue Aug 11 09:33:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247066">247066</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 10 17:51:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246961">246961</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 10 17:06:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246914">246914</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 10 15:38:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246892">246892</a>           |  create volume snapshot and clone when fstype is zfs           | Mon Aug 10 14:20:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245469">245469</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug  7 21:21:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245364">245364</a>           |  create volume snapshot and clone when fstype is zfs           | Fri Aug  7 19:29:37 IST 2020  | Pass |
