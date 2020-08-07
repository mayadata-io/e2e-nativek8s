### 3F08-zfspv-property-modify-xfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245294">245294</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug  7 15:14:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245272">245272</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug  7 14:15:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245051">245051</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug  7 12:11:38 IST 2020  | Pass |
