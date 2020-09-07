### 3F03-zfs-volume-resize-zfs

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as zfs.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class. To know more about this [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-properties-verify).
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-volume-resize).
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257833">257833</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Sep  7 18:09:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257555">257555</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Sep  4 15:56:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257529">257529</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Sep  4 12:02:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257335">257335</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Sep  2 16:11:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257309">257309</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Sep  2 13:39:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257283">257283</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Sep  2 10:18:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257174">257174</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Sep  1 20:24:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257148">257148</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Sep  1 19:12:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257121">257121</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Sep  1 13:07:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257096">257096</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Sep  1 12:02:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256988">256988</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 31 21:15:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256966">256966</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 31 13:26:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256769">256769</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 31 09:41:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256746">256746</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 31 07:00:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254801">254801</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 21 16:34:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253791">253791</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 19 16:02:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253176">253176</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Sun Aug 16 12:31:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252957">252957</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Sat Aug 15 23:48:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252932">252932</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Sat Aug 15 19:46:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252561">252561</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Sat Aug 15 10:31:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251942">251942</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 14 21:18:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251858">251858</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 14 20:31:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251836">251836</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 14 19:40:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251564">251564</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 14 11:42:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251540">251540</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug 14 10:51:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250268">250268</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Thu Aug 13 10:40:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249603">249603</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 12 21:46:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249488">249488</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 12 19:38:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249404">249404</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 12 17:22:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249122">249122</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 12 11:57:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249099">249099</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Wed Aug 12 10:40:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248765">248765</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Aug 11 17:47:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248259">248259</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Aug 11 10:24:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248206">248206</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Tue Aug 11 09:31:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247059">247059</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 17:51:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246954">246954</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 17:04:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246907">246907</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 15:38:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246885">246885</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 14:20:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245462">245462</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 21:23:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245357">245357</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 19:29:29 IST 2020  | Pass |
