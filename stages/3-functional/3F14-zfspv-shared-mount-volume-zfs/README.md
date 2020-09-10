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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260184">260184</a>           |  zfspv shared mount volume support when fstype is zfs           | Thu Sep 10 21:33:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260064">260064</a>           |  zfspv shared mount volume support when fstype is zfs           | Thu Sep 10 20:01:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258070">258070</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Sep  8 11:39:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257844">257844</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Sep  7 18:09:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257566">257566</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Sep  4 15:56:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257540">257540</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Sep  4 12:02:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257346">257346</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Sep  2 16:14:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257320">257320</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Sep  2 13:40:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257294">257294</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Sep  2 10:20:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257185">257185</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Sep  1 20:24:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257159">257159</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Sep  1 19:13:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257132">257132</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Sep  1 13:08:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257107">257107</a>           |  zfspv shared mount volume support when fstype is zfs           | Tue Sep  1 12:03:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256999">256999</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 31 21:15:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256977">256977</a>           |  zfspv shared mount volume support when fstype is zfs           | Mon Aug 31 13:28:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254812">254812</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 21 16:35:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253802">253802</a>           |  zfspv shared mount volume support when fstype is zfs           | Wed Aug 19 16:03:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253187">253187</a>           |  zfspv shared mount volume support when fstype is zfs           | Sun Aug 16 12:34:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252968">252968</a>           |  zfspv shared mount volume support when fstype is zfs           | Sat Aug 15 23:48:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252572">252572</a>           |  zfspv shared mount volume support when fstype is zfs           | Sat Aug 15 10:34:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251953">251953</a>           |  zfspv shared mount volume support when fstype is zfs           | Fri Aug 14 21:18:21 IST 2020  | Pass |
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
