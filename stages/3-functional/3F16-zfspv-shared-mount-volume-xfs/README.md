### 3F16-zfspv-shared-mount-volume-xfs

#### Description

This functional test validates the successful provisioning of shared mount volume where multiple pods can use the same pvc, when application uses fstype as xfs. Applications who wants to share the volume can be deployed using the storage class with `shared: yes` parameter. 

#### Steps involved

1. Deploy busybox application with file-system xfs on top of zfs-localpv.
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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253804">253804</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 19 16:03:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253189">253189</a>           |  zfspv shared mount volume support when fstype is xfs           | Sun Aug 16 12:34:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252970">252970</a>           |  zfspv shared mount volume support when fstype is xfs           | Sat Aug 15 23:48:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252574">252574</a>           |  zfspv shared mount volume support when fstype is xfs           | Sat Aug 15 10:34:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251955">251955</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug 14 21:18:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251871">251871</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug 14 20:31:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251849">251849</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug 14 19:43:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251577">251577</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug 14 11:45:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251553">251553</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug 14 10:51:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250281">250281</a>           |  zfspv shared mount volume support when fstype is xfs           | Thu Aug 13 10:40:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249616">249616</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 12 21:48:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249501">249501</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 12 19:38:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249417">249417</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 12 17:23:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249135">249135</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 12 11:57:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249112">249112</a>           |  zfspv shared mount volume support when fstype is xfs           | Wed Aug 12 10:40:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248778">248778</a>           |  zfspv shared mount volume support when fstype is xfs           | Tue Aug 11 17:47:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248272">248272</a>           |  zfspv shared mount volume support when fstype is xfs           | Tue Aug 11 10:24:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248219">248219</a>           |  zfspv shared mount volume support when fstype is xfs           | Tue Aug 11 09:33:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247072">247072</a>           |  zfspv shared mount volume support when fstype is xfs           | Mon Aug 10 17:51:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246967">246967</a>           |  zfspv shared mount volume support when fstype is xfs           | Mon Aug 10 17:06:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246920">246920</a>           |  zfspv shared mount volume support when fstype is xfs           | Mon Aug 10 15:38:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246898">246898</a>           |  zfspv shared mount volume support when fstype is xfs           | Mon Aug 10 14:20:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245475">245475</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug  7 21:23:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245370">245370</a>           |  zfspv shared mount volume support when fstype is xfs           | Fri Aug  7 19:29:45 IST 2020  | Pass |
