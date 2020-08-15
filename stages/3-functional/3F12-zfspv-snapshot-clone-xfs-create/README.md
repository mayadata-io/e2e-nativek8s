### 3F12-zfspv-snapshot-clone-xfs-create

#### Description

This test takes the zfs volume snapshot and later use that snapshot to create clone volumes when application is deployed with xfs file-system on top of zfs-localpv.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the test for creating the volume snapshot after dumping some data into the application mount point. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
4. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different `percona-mysql` application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
5. Deprovision the clone volume and its application.
6. Delete the volume snapshot.
7. Deprovision the application and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252941">252941</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 19:46:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252570">252570</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 10:34:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251951">251951</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 21:18:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251867">251867</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 20:31:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251845">251845</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251573">251573</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 11:45:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251549">251549</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 10:51:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250277">250277</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Aug 13 10:38:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249612">249612</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 21:48:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249497">249497</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 19:38:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249413">249413</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 17:23:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249131">249131</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 11:57:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249108">249108</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 10:40:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248774">248774</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 17:47:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248268">248268</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 10:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248215">248215</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 09:33:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247068">247068</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 17:51:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246963">246963</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 17:06:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246916">246916</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 15:38:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246894">246894</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 14:20:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245471">245471</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 21:23:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245366">245366</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 19:29:37 IST 2020  | Pass |
