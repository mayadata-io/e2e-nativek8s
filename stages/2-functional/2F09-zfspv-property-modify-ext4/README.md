### 2F09-zfspv-property-modify-ext4

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here]()
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
