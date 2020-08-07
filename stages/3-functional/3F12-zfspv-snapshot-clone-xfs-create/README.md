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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245298">245298</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 15:14:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245276">245276</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 14:15:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245055">245055</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 12:11:47 IST 2020  | Pass |