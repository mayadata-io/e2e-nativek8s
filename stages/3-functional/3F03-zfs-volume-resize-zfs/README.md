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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246954">246954</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 17:04:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246907">246907</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 15:38:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246885">246885</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Mon Aug 10 14:20:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245462">245462</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 21:23:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245357">245357</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 19:29:29 IST 2020  | Pass |
