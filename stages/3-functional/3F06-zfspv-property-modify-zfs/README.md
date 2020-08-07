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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245292">245292</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 15:14:37 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245270">245270</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 14:15:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245049">245049</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 12:11:40 IST 2020  | Pass |
