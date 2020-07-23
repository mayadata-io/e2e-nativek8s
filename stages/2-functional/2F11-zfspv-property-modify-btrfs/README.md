### 2F11-zfspv-property-modify-btrfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is btrfs.

#### Steps involved

1. Deploy application `percona-mysql` using btrfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here]()
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
