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
