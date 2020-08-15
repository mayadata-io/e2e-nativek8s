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
