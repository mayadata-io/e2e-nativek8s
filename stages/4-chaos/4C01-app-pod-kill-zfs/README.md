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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276912">276912</a>           |  Kill the application pod container when fstype is zfs           | Mon Oct 12 16:31:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276462">276462</a>           |  Kill the application pod container when fstype is zfs           | Sun Oct 11 00:18:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276409">276409</a>           |  Kill the application pod container when fstype is zfs           | Sat Oct 10 20:30:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276375">276375</a>           |  Kill the application pod container when fstype is zfs           | Sat Oct 10 18:48:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276322">276322</a>           |  Kill the application pod container when fstype is zfs           | Sat Oct 10 17:31:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276269">276269</a>           |  Kill the application pod container when fstype is zfs           | Sat Oct 10 15:47:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274625">274625</a>           |  Kill the application pod container when fstype is zfs           | Fri Oct  9 11:36:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274566">274566</a>           |  Kill the application pod container when fstype is zfs           | Fri Oct  9 10:34:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271279">271279</a>           |  Kill the application pod container when fstype is zfs           | Thu Oct  1 17:33:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268093">268093</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep 22 13:48:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267980">267980</a>           |  Kill the application pod container when fstype is zfs           | Tue Sep 22 11:55:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266923">266923</a>           |  Kill the application pod container when fstype is zfs           | Fri Sep 18 17:05:16 IST 2020  | Pass |
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