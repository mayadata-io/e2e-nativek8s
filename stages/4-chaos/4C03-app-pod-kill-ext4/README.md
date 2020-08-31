### 4C03-app-pod-kill-ext4

#### Description

This test kills the container of application pod consuming zfs-localpv backed by ext4 file-system. Pumba tool is used for this test to execute.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the application pod kill test with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|