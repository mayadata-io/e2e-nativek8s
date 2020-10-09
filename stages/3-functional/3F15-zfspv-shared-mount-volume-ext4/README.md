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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274563">274563</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Oct  9 10:18:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271276">271276</a>           |  zfspv shared mount volume support when fstype is ext4           | Thu Oct  1 17:19:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268090">268090</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep 22 13:35:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267977">267977</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep 22 11:41:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266920">266920</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Sep 18 16:50:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266581">266581</a>           |  zfspv shared mount volume support when fstype is ext4           | Thu Sep 17 11:21:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264793">264793</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep 15 20:21:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264749">264749</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep 15 19:17:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263025">263025</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Sep 14 12:47:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260598">260598</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Sep 11 09:11:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260185">260185</a>           |  zfspv shared mount volume support when fstype is ext4           | Thu Sep 10 21:33:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260065">260065</a>           |  zfspv shared mount volume support when fstype is ext4           | Thu Sep 10 20:01:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258071">258071</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep  8 11:39:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257845">257845</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Sep  7 18:09:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257567">257567</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Sep  4 15:56:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257541">257541</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Sep  4 12:02:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257347">257347</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Sep  2 16:14:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257321">257321</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Sep  2 13:40:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257295">257295</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Sep  2 10:20:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257186">257186</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep  1 20:24:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257160">257160</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep  1 19:13:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257133">257133</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep  1 13:08:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257108">257108</a>           |  zfspv shared mount volume support when fstype is ext4           | Tue Sep  1 12:02:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257000">257000</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 31 21:15:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256978">256978</a>           |  zfspv shared mount volume support when fstype is ext4           | Mon Aug 31 13:28:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254813">254813</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 21 16:35:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253803">253803</a>           |  zfspv shared mount volume support when fstype is ext4           | Wed Aug 19 16:03:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253188">253188</a>           |  zfspv shared mount volume support when fstype is ext4           | Sun Aug 16 12:34:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252969">252969</a>           |  zfspv shared mount volume support when fstype is ext4           | Sat Aug 15 23:48:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252573">252573</a>           |  zfspv shared mount volume support when fstype is ext4           | Sat Aug 15 10:34:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251954">251954</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 14 21:18:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251870">251870</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 14 20:31:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251848">251848</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251576">251576</a>           |  zfspv shared mount volume support when fstype is ext4           | Fri Aug 14 11:45:09 IST 2020  | Pass |
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
