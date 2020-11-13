### 3F17-zfspv-shared-mount-volume-btrfs

#### Description

This functional test validates the successful provisioning of shared mount volume where multiple pods can use the same pvc, when application uses fstype as btrfs. Applications who wants to share the volume can be deployed using the storage class with `shared: yes` parameter. 

#### Steps involved

1. Deploy busybox application with file-system btrfs on top of zfs-localpv.
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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290297">290297</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Nov 13 13:15:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290106">290106</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Nov 13 11:22:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290070">290070</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Nov 13 09:24:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289844">289844</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Nov 12 20:32:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289809">289809</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Nov 12 18:02:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289356">289356</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Nov 12 08:59:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288895">288895</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Nov 11 16:10:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288861">288861</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Nov 11 12:53:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288826">288826</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Nov 11 10:54:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288712">288712</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Nov 11 08:27:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288261">288261</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Nov 10 18:27:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281258">281258</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Oct 15 14:34:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280414">280414</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Oct 14 22:02:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279640">279640</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Oct 14 15:00:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279591">279591</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Oct 14 13:36:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279295">279295</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Oct 14 11:35:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279039">279039</a>           |  zfspv shared mount volume support when fstype is btrfs           | Wed Oct 14 10:43:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278925">278925</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Oct 13 20:45:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278891">278891</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Oct 13 18:58:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278857">278857</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Oct 13 16:45:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277926">277926</a>           |  zfspv shared mount volume support when fstype is btrfs           | Mon Oct 12 21:42:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277112">277112</a>           |  zfspv shared mount volume support when fstype is btrfs           | Mon Oct 12 17:25:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276905">276905</a>           |  zfspv shared mount volume support when fstype is btrfs           | Mon Oct 12 15:37:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276455">276455</a>           |  zfspv shared mount volume support when fstype is btrfs           | Sat Oct 10 23:30:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276402">276402</a>           |  zfspv shared mount volume support when fstype is btrfs           | Sat Oct 10 19:43:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276368">276368</a>           |  zfspv shared mount volume support when fstype is btrfs           | Sat Oct 10 17:56:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276315">276315</a>           |  zfspv shared mount volume support when fstype is btrfs           | Sat Oct 10 16:53:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276262">276262</a>           |  zfspv shared mount volume support when fstype is btrfs           | Sat Oct 10 15:29:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274624">274624</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Oct  9 11:24:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274565">274565</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Oct  9 10:19:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271278">271278</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Oct  1 17:19:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268092">268092</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Sep 22 13:35:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267979">267979</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Sep 22 11:41:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266922">266922</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Sep 18 16:50:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266583">266583</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Sep 17 11:21:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264795">264795</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Sep 15 20:21:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264751">264751</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Sep 15 19:17:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263027">263027</a>           |  zfspv shared mount volume support when fstype is btrfs           | Mon Sep 14 12:47:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260600">260600</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Sep 11 09:11:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260187">260187</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Sep 10 21:33:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260067">260067</a>           |  zfspv shared mount volume support when fstype is btrfs           | Thu Sep 10 20:01:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258073">258073</a>           |  zfspv shared mount volume support when fstype is btrfs           | Tue Sep  8 11:39:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257847">257847</a>           |  zfspv shared mount volume support when fstype is btrfs           | Mon Sep  7 18:09:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257569">257569</a>           |  zfspv shared mount volume support when fstype is btrfs           | Fri Sep  4 15:57:02 IST 2020  | Pass |