### 3F15-zfspv-shared-mount-volume-ext4

#### Description

This functional test validates the successful provisioning of shared mount volume where multiple pods can use the same pvc, when application uses fstype as ext4. Applications who wants to share the volume can be deployed using the storage class with `shared: yes` parameter. 

#### Steps involved

1. Deploy busybox application with file-system ext4 on top of zfs-localpv.
2. Verify that application pvc and pod are in Bound and running state respectively.
3. Dump some data to this application mount point and take the md5sum of that data.
4. As we used shared volume storage-class, scale the application deployment replicas.
5. Verify that dumped data is accessible now from the scaled application pod, and repeat this data consitency check this time after dumping the data from newly scaled application pod. So in short data should be accessible from all the applications which are sharing the volume. For detailed README of shared mount volume test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-shared-mount).
6. Run the test for creating the volume snapshot for this shared volume. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
7. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
8. Deprovision the resources created throughout the test. for e.g. clone volume, volume-snapshot and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251552">251552</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 14 10:51:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250280">250280</a>           |  zfspv shared mount volume support when fstype is ext4           | Thu Aug 13 10:40:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249615">249615</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 12 21:48:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249500">249500</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 12 19:38:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249416">249416</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 12 17:23:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249134">249134</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 12 11:57:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249111">249111</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 12 10:40:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248777">248777</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Aug 11 17:47:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248271">248271</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Aug 11 10:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248218">248218</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Aug 11 09:33:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247071">247071</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 10 17:51:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246966">246966</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 10 17:06:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246919">246919</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 10 15:38:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246897">246897</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 10 14:20:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245474">245474</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug  7 21:23:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245369">245369</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug  7 19:29:42 IST 2020  | Pass |
