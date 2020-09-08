### 4C02-app-pod-kill-xfs

#### Description

This test kills the container of application pod consuming zfs-localpv backed by xfs file-system. Pumba tool is used for this test to execute.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the application pod kill test with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258075">258075</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep  8 11:59:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257849">257849</a>           |  Kill the application pod container when fstype is xfs           | Mon Sep  7 18:27:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257571">257571</a>           |  Kill the application pod container when fstype is xfs           | Fri Sep  4 16:15:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257544">257544</a>           |  Kill the application pod container when fstype is xfs           | Fri Sep  4 12:19:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257350">257350</a>           |  Kill the application pod container when fstype is xfs           | Wed Sep  2 16:28:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257324">257324</a>           |  Kill the application pod container when fstype is xfs           | Wed Sep  2 13:54:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257298">257298</a>           |  Kill the application pod container when fstype is xfs           | Wed Sep  2 10:38:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257189">257189</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep  1 20:42:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257163">257163</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep  1 19:27:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257136">257136</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep  1 13:18:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257111">257111</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep  1 12:20:18 IST 2020  | Pass |