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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263030">263030</a>           |  Kill the application pod container when fstype is ext4           | Mon Sep 14 13:09:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260603">260603</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep 11 09:28:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260190">260190</a>           |  Kill the application pod container when fstype is ext4           | Thu Sep 10 21:51:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260070">260070</a>           |  Kill the application pod container when fstype is ext4           | Thu Sep 10 20:17:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258076">258076</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  8 11:59:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257850">257850</a>           |  Kill the application pod container when fstype is ext4           | Mon Sep  7 18:27:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257572">257572</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep  4 16:15:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257545">257545</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep  4 12:19:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257351">257351</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 16:28:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257325">257325</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 13:54:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257299">257299</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 10:38:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257190">257190</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 20:42:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257164">257164</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 19:27:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257137">257137</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 13:18:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257112">257112</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 12:20:19 IST 2020  | Pass |