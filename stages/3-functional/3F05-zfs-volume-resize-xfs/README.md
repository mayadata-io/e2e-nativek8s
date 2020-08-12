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
