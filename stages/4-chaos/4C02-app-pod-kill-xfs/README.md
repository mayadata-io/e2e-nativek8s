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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279599">279599</a>           |  Kill the application pod container when fstype is xfs           | Wed Oct 14 14:06:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279303">279303</a>           |  Kill the application pod container when fstype is xfs           | Wed Oct 14 12:30:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278933">278933</a>           |  Kill the application pod container when fstype is xfs           | Tue Oct 13 21:34:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278899">278899</a>           |  Kill the application pod container when fstype is xfs           | Tue Oct 13 19:47:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278865">278865</a>           |  Kill the application pod container when fstype is xfs           | Tue Oct 13 17:35:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277934">277934</a>           |  Kill the application pod container when fstype is xfs           | Mon Oct 12 22:33:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277120">277120</a>           |  Kill the application pod container when fstype is xfs           | Mon Oct 12 18:17:57 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276913">276913</a>           |  Kill the application pod container when fstype is xfs           | Mon Oct 12 16:31:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276463">276463</a>           |  Kill the application pod container when fstype is xfs           | Sun Oct 11 00:18:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276410">276410</a>           |  Kill the application pod container when fstype is xfs           | Sat Oct 10 20:30:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276376">276376</a>           |  Kill the application pod container when fstype is xfs           | Sat Oct 10 18:48:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276323">276323</a>           |  Kill the application pod container when fstype is xfs           | Sat Oct 10 17:31:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276270">276270</a>           |  Kill the application pod container when fstype is xfs           | Sat Oct 10 15:47:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274626">274626</a>           |  Kill the application pod container when fstype is xfs           | Fri Oct  9 11:36:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274567">274567</a>           |  Kill the application pod container when fstype is xfs           | Fri Oct  9 10:34:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271280">271280</a>           |  Kill the application pod container when fstype is xfs           | Thu Oct  1 17:33:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268094">268094</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep 22 13:48:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267981">267981</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep 22 11:55:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266924">266924</a>           |  Kill the application pod container when fstype is xfs           | Fri Sep 18 17:05:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266585">266585</a>           |  Kill the application pod container when fstype is xfs           | Thu Sep 17 11:37:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264797">264797</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep 15 20:33:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264753">264753</a>           |  Kill the application pod container when fstype is xfs           | Tue Sep 15 19:31:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263029">263029</a>           |  Kill the application pod container when fstype is xfs           | Mon Sep 14 13:09:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260602">260602</a>           |  Kill the application pod container when fstype is xfs           | Fri Sep 11 09:28:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260189">260189</a>           |  Kill the application pod container when fstype is xfs           | Thu Sep 10 21:51:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260069">260069</a>           |  Kill the application pod container when fstype is xfs           | Thu Sep 10 20:17:17 IST 2020  | Pass |
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