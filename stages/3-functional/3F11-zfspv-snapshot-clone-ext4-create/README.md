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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281252">281252</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Oct 15 14:34:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280408">280408</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Oct 14 21:59:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279634">279634</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Oct 14 15:00:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279585">279585</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Oct 14 13:35:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279289">279289</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Oct 14 11:35:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279033">279033</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Oct 14 10:43:17 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278919">278919</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Oct 13 20:42:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278885">278885</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Oct 13 18:58:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278851">278851</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Oct 13 16:42:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277920">277920</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Oct 12 21:42:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277106">277106</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Oct 12 17:23:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276899">276899</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Oct 12 15:37:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276449">276449</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Oct 10 23:30:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276396">276396</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Oct 10 19:41:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276362">276362</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Oct 10 17:56:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276309">276309</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Oct 10 16:53:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276256">276256</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Oct 10 15:29:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274618">274618</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Oct  9 11:23:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274559">274559</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Oct  9 10:19:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271272">271272</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Oct  1 17:19:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268086">268086</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep 22 13:35:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267973">267973</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep 22 11:41:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266916">266916</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Sep 18 16:50:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266577">266577</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Sep 17 11:21:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264789">264789</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep 15 20:21:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264745">264745</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep 15 19:17:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263021">263021</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Sep 14 12:47:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260594">260594</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Sep 11 09:11:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260181">260181</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Sep 10 21:33:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260061">260061</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Sep 10 20:01:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258067">258067</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep  8 11:38:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257841">257841</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Sep  7 18:09:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257563">257563</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Sep  4 15:56:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257537">257537</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Sep  4 12:02:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257343">257343</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Sep  2 16:14:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257317">257317</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Sep  2 13:40:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257291">257291</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Sep  2 10:20:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257182">257182</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep  1 20:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257156">257156</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep  1 19:12:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257129">257129</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep  1 13:07:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257104">257104</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Sep  1 12:00:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256996">256996</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 31 21:12:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256974">256974</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 31 13:28:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256777">256777</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 31 09:38:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256754">256754</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 31 07:00:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254809">254809</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 21 16:32:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253799">253799</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 19 16:03:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253184">253184</a>           |  create volume snapshot and clone when fstype is ext4           | Sun Aug 16 12:34:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252965">252965</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Aug 15 23:48:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252940">252940</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Aug 15 19:43:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252569">252569</a>           |  create volume snapshot and clone when fstype is ext4           | Sat Aug 15 10:31:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251950">251950</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 14 21:18:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251866">251866</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 14 20:31:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251844">251844</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251572">251572</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 14 11:45:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251548">251548</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug 14 10:51:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250276">250276</a>           |  create volume snapshot and clone when fstype is ext4           | Thu Aug 13 10:38:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249611">249611</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 12 21:48:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249496">249496</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 12 19:38:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249412">249412</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 12 17:23:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249130">249130</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 12 11:57:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249107">249107</a>           |  create volume snapshot and clone when fstype is ext4           | Wed Aug 12 10:40:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248773">248773</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Aug 11 17:47:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248267">248267</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Aug 11 10:24:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248214">248214</a>           |  create volume snapshot and clone when fstype is ext4           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247067">247067</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 17:48:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246962">246962</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 17:06:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246915">246915</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 15:38:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246893">246893</a>           |  create volume snapshot and clone when fstype is ext4           | Mon Aug 10 14:20:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245470">245470</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug  7 21:23:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245365">245365</a>           |  create volume snapshot and clone when fstype is ext4           | Fri Aug  7 19:29:40 IST 2020  | Pass |
