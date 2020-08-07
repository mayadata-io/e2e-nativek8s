### 3F04-zfs-volume-resize-ext4

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zv-properties-verify)
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfs-volume-resize)
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245047">245047</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 12:11:37 IST 2020  | Pass |