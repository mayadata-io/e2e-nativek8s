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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257842">257842</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Sep  7 18:09:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257564">257564</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep  4 15:56:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257538">257538</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep  4 12:02:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257344">257344</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 16:14:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257318">257318</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 13:40:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257292">257292</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 10:20:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257183">257183</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 20:24:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257157">257157</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 19:13:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257130">257130</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 13:07:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257105">257105</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 12:02:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256997">256997</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 21:15:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256975">256975</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 13:28:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256778">256778</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 09:41:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256755">256755</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 07:00:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254810">254810</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 21 16:34:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253800">253800</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 19 16:03:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253185">253185</a>           |  create volume snapshot and clone when fstype is xfs           | Sun Aug 16 12:34:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252966">252966</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 23:48:36 IST 2020  | Pass |
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
