### 3F11-zfspv-snapshot-clone-ext4-create

#### Description

This test takes the zfs volume snapshot and later use that snapshot to create clone volumes when application is deployed with ext4 file-system on top of zfs-localpv.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the test for creating the volume snapshot after dumping some data into the application mount point. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
4. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different `percona-mysql` application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
5. Deprovision the clone volume and its application.
6. Delete the volume snapshot.
7. Deprovision the application and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248267">248267</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Aug 11 10:24:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248214">248214</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247067">247067</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 17:48:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246962">246962</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 17:06:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246915">246915</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 15:38:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246893">246893</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 14:20:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245470">245470</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug  7 21:23:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245365">245365</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug  7 19:29:40 IST 2020  | Pass |
