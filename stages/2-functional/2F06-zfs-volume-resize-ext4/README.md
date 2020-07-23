### 2F06-zfs-volume-resize-ext4

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|