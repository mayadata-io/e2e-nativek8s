### 3F03-zfs-volume-resize-zfs

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as zfs.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class. To know more about this [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zv-properties-verify) 
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfs-volume-resize)
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245046">245046</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 12:11:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/244617">244617</a>           |  zv property verify and zfs volume resize when fstype is zfs           | Fri Aug  7 11:08:51 IST 2020  | Pass |
|        <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/233379">233379</a>        |  zv property verify and zfs volume resize when fstype is zfs           | Thu Aug 6 19:34:27 IST 2020  | Pass |