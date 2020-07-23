### 2F10-zfspv-property-modify-xfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here]()
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
