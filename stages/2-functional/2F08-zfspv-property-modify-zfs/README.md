### 2F08-zfspv-property-modify-zfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is zfs.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zv-property-runtime-modify)
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
