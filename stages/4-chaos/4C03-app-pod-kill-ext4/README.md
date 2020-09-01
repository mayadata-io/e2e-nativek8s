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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257164">257164</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 19:27:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257137">257137</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 13:18:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257112">257112</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 12:20:19 IST 2020  | Pass |