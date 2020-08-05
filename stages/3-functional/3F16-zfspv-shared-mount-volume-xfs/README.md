### 3F16-zfspv-shared-mount-volume-xfs

#### Description

This functional test validates the successful provisioning of shared mount volume where multiple pods can use the same pvc, when application uses fstype as xfs. Applications who wants to share the volume can be deployed using the storage class with `shared: yes` parameter. 

#### Steps involved

1. Deploy busybox application with file-system xfs on top of zfs-localpv.
2. Verify that application pvc and pod are in Bound and running state respectively.
3. Dump some data to this application mount point and take the md5sum of that data.
4. As we used shared volume storage-class, scale the application deployment replicas.
5. Verify that dumped data is accessible now from the scaled application pod, and repeat this data consitency check this time after dumping the data from newly scaled application pod. So in short data should be accessible from all the applications which are sharing the volume. For detailed README of shared mount volume test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfspv-shared-mount)
6. Run the test for creating the volume snapshot for this shared volume. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfspv-snapshot
7. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfspv-clone)
8. Deprovision the resources created throughout the test. for e.g. clone volume, volume-snapshot and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|