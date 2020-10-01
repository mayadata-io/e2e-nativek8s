### 3F13-zfspv-snapshot-clone-btrfs-create

#### Description

This test takes the zfs volume snapshot and later use that snapshot to create clone volumes when application is deployed with btrfs file-system on top of zfs-localpv.

#### Steps involved

1. Deploy application `percona-mysql` using btrfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the test for creating the volume snapshot after dumping some data into the application mount point. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
4. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different `percona-mysql` application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
5. Deprovision the clone volume and its application.
6. Delete the volume snapshot.
7. Deprovision the application and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271274">271274</a>           |  create volume snapshot and clone when fstype is btrfs           | Thu Oct  1 17:19:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268088">268088</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep 22 13:35:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267975">267975</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep 22 11:41:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266918">266918</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Sep 18 16:50:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266579">266579</a>           |  create volume snapshot and clone when fstype is btrfs           | Thu Sep 17 11:21:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264791">264791</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep 15 20:21:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264747">264747</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep 15 19:17:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263023">263023</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Sep 14 12:47:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260596">260596</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Sep 11 09:11:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260183">260183</a>           |  create volume snapshot and clone when fstype is btrfs           | Thu Sep 10 21:32:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260063">260063</a>           |  create volume snapshot and clone when fstype is btrfs           | Thu Sep 10 19:58:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258069">258069</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep  8 11:39:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257843">257843</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Sep  7 18:09:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257565">257565</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Sep  4 15:56:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257539">257539</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Sep  4 12:02:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257345">257345</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Sep  2 16:14:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257319">257319</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Sep  2 13:40:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257293">257293</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Sep  2 10:20:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257184">257184</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep  1 20:24:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257158">257158</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep  1 19:13:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257131">257131</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep  1 13:07:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257106">257106</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Sep  1 12:03:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256998">256998</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 31 21:15:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256976">256976</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 31 13:28:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254811">254811</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 21 16:32:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253801">253801</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 19 16:03:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253186">253186</a>           |  create volume snapshot and clone when fstype is btrfs           | Sun Aug 16 12:34:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252967">252967</a>           |  create volume snapshot and clone when fstype is btrfs           | Sat Aug 15 23:48:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252571">252571</a>           |  create volume snapshot and clone when fstype is btrfs           | Sat Aug 15 10:34:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251952">251952</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 14 21:18:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251868">251868</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 14 20:31:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251846">251846</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251574">251574</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 14 11:45:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251550">251550</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug 14 10:51:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250278">250278</a>           |  create volume snapshot and clone when fstype is btrfs           | Thu Aug 13 10:40:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249613">249613</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 12 21:48:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249498">249498</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 12 19:38:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249414">249414</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 12 17:23:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249132">249132</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 12 11:57:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249109">249109</a>           |  create volume snapshot and clone when fstype is btrfs           | Wed Aug 12 10:40:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248775">248775</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Aug 11 17:47:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248269">248269</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Aug 11 10:24:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248216">248216</a>           |  create volume snapshot and clone when fstype is btrfs           | Tue Aug 11 09:33:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247069">247069</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 10 17:51:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246964">246964</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 10 17:06:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246917">246917</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 10 15:38:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246895">246895</a>           |  create volume snapshot and clone when fstype is btrfs           | Mon Aug 10 14:20:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245472">245472</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug  7 21:23:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245367">245367</a>           |  create volume snapshot and clone when fstype is btrfs           | Fri Aug  7 19:29:40 IST 2020  | Pass |
