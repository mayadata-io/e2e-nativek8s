### 3F14-zfspv-shared-mount-volume-zfs

#### Description

This functional test validates the successful provisioning of shared mount volume where multiple pods can use the same pvc, when application uses fstype as zfs. Applications who wants to share the volume can be deployed using the storage class with `shared: yes` parameter. 

#### Steps involved

1. Deploy busybox application with file-system zfs on top of zfs-localpv.
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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251869">251869</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 14 20:31:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251847">251847</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251575">251575</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 14 11:45:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251551">251551</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 14 10:51:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250279">250279</a>           |  zfspv shared mount volume support when fstype is zfs           | Thu Aug 13 10:40:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249614">249614</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 12 21:48:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249499">249499</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 12 19:38:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249415">249415</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 12 17:23:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249133">249133</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 12 11:57:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249110">249110</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 12 10:40:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248776">248776</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Aug 11 17:47:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248270">248270</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Aug 11 10:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248217">248217</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Aug 11 09:33:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247070">247070</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 10 17:51:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246965">246965</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 10 17:06:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246918">246918</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 10 15:38:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246896">246896</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 10 14:20:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245473">245473</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug  7 21:23:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245368">245368</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug  7 19:29:40 IST 2020  | Pass |
