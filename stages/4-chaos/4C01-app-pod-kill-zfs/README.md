### 4C01-app-pod-kill-zfs

#### Description

This test kills the container of application pod consuming zfs-localpv backed by zfs file-system. Pumba tool is used for this test to execute.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the application pod kill test with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266584">266584</a>           |  Kill the application pod container when fstype is zfs           | Thu Sep 17 11:36:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264796">264796</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep 15 20:32:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264752">264752</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep 15 19:31:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263028">263028</a>           |  Kill the application pod container when fstype is zfs           | Mon Sep 14 13:09:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260601">260601</a>           |  Kill the application pod container when fstype is zfs           | Fri Sep 11 09:28:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260188">260188</a>           |  Kill the application pod container when fstype is zfs           | Thu Sep 10 21:51:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260068">260068</a>           |  Kill the application pod container when fstype is zfs           | Thu Sep 10 20:17:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258074">258074</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep  8 11:59:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257848">257848</a>           |  Kill the application pod container when fstype is zfs           | Mon Sep  7 18:27:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257570">257570</a>           |  Kill the application pod container when fstype is zfs           | Fri Sep  4 16:14:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257543">257543</a>           |  Kill the application pod container when fstype is zfs           | Fri Sep  4 12:19:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257349">257349</a>           |  Kill the application pod container when fstype is zfs           | Wed Sep  2 16:28:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257323">257323</a>           |  Kill the application pod container when fstype is zfs           | Wed Sep  2 13:54:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257297">257297</a>           |  Kill the application pod container when fstype is zfs           | Wed Sep  2 10:38:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257188">257188</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep  1 20:42:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257162">257162</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep  1 19:27:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257135">257135</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep  1 13:18:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257110">257110</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep  1 12:20:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257002">257002</a>           |  Kill the application pod container when fstype is zfs           | Mon Aug 31 21:31:39 IST 2020  | Fail |