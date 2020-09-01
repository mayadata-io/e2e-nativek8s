### 3F05-zfs-volume-resize-xfs

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-properties-verify).
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-volume-resize).
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257176">257176</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 20:24:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257150">257150</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 19:12:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257123">257123</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 13:07:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257098">257098</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 12:02:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256990">256990</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 21:15:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256968">256968</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 13:26:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256771">256771</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 09:41:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256748">256748</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 07:00:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254803">254803</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 21 16:34:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253793">253793</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 19 16:02:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253178">253178</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sun Aug 16 12:34:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252959">252959</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 23:48:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252934">252934</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 19:46:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252563">252563</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 10:31:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251944">251944</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 21:15:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251860">251860</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 20:31:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251838">251838</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 19:43:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251566">251566</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 11:44:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251542">251542</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 10:51:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250270">250270</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Aug 13 10:40:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249605">249605</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 21:48:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249490">249490</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 19:38:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249406">249406</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 17:23:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249124">249124</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 11:57:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249101">249101</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 10:40:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248767">248767</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 17:47:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248261">248261</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 10:24:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248208">248208</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 09:31:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247061">247061</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 17:48:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246956">246956</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 17:04:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246909">246909</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 15:38:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246887">246887</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 14:20:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245464">245464</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug  7 21:23:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245359">245359</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug  7 19:29:22 IST 2020  | Pass |
