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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245048">245048</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug  7 12:11:38 IST 2020  | Pass |