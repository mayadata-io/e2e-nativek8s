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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246955">246955</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 17:04:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246908">246908</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 15:37:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246886">246886</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 14:20:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245463">245463</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 21:23:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245358">245358</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 19:29:36 IST 2020  | Pass |
