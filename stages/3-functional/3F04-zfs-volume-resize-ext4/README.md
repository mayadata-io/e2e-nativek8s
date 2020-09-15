### 3F04-zfs-volume-resize-ext4

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-properties-verify).
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-volume-resize).
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264782">264782</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 15 20:21:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264738">264738</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 15 19:15:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263014">263014</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Sep 14 12:47:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260587">260587</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep 11 09:11:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260174">260174</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Sep 10 21:33:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260054">260054</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Sep 10 20:01:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258060">258060</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  8 11:38:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257834">257834</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Sep  7 18:09:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257556">257556</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep  4 15:56:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257530">257530</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep  4 12:02:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257336">257336</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 16:14:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257310">257310</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 13:39:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257284">257284</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 10:20:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257175">257175</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 20:24:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257149">257149</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 19:12:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257122">257122</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 13:07:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257097">257097</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 12:02:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256989">256989</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 21:15:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256967">256967</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 13:26:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256770">256770</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 09:41:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256747">256747</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 07:00:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254802">254802</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 21 16:35:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253792">253792</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 19 16:03:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253177">253177</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sun Aug 16 12:34:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252958">252958</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 23:48:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252933">252933</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 19:45:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252562">252562</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 10:31:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251943">251943</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 21:18:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251859">251859</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 20:31:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251837">251837</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 19:43:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251565">251565</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 11:44:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251541">251541</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 10:51:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250269">250269</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Aug 13 10:40:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249604">249604</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 21:48:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249489">249489</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 19:38:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249405">249405</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 17:22:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249123">249123</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 11:57:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249100">249100</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 10:40:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248766">248766</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 17:47:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248260">248260</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 10:24:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248207">248207</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247060">247060</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 17:51:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246955">246955</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 17:04:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246908">246908</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 15:37:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246886">246886</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 14:20:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245463">245463</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 21:23:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245358">245358</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 19:29:36 IST 2020  | Pass |
