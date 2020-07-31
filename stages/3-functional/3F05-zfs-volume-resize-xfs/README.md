### 3F05-zfs-volume-resize-xfs

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zv-properties-verify)
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfs-volume-resize)
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|