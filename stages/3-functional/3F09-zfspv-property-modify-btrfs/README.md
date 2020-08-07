### 3F09-zfspv-property-modify-btrfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is btrfs.

#### Steps involved

1. Deploy application `percona-mysql` using btrfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify)
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245052">245052</a>           |  zfspv property runtime modification when fstype is btrfs           | Fri Aug  7 12:11:36 IST 2020  | Pass |
