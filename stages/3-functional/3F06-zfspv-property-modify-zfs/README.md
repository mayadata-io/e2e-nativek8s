### 3F06-zfspv-property-modify-zfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is zfs.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246957">246957</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 17:04:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246910">246910</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 15:38:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246888">246888</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 14:20:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245465">245465</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 21:23:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245360">245360</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 19:29:27 IST 2020  | Pass |
