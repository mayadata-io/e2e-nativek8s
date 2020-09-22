### 4C04-app-pod-kill-btrfs

#### Description

This test kills the container of application pod consuming zfs-localpv backed by btrfs file-system. Pumba tool is used for this test to execute.

#### Steps involved

1. Deploy application `percona-mysql` using btrfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the application pod kill test with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267983">267983</a>           |  Kill the application pod container when fstype is btrfs           | Tue Sep 22 11:55:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266926">266926</a>           |  Kill the application pod container when fstype is btrfs           | Fri Sep 18 17:05:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266587">266587</a>           |  Kill the application pod container when fstype is btrfs           | Thu Sep 17 11:36:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264799">264799</a>           |  Kill the application pod container when fstype is btrfs           | Tue Sep 15 20:33:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264755">264755</a>           |  Kill the application pod container when fstype is btrfs           | Tue Sep 15 19:31:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263031">263031</a>           |  Kill the application pod container when fstype is btrfs           | Mon Sep 14 13:09:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260604">260604</a>           |  Kill the application pod container when fstype is btrfs           | Fri Sep 11 09:28:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260191">260191</a>           |  Kill the application pod container when fstype is btrfs           | Thu Sep 10 21:51:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260071">260071</a>           |  Kill the application pod container when fstype is btrfs           | Thu Sep 10 20:17:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258077">258077</a>           |  Kill the application pod container when fstype is btrfs           | Tue Sep  8 11:59:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257851">257851</a>           |  Kill the application pod container when fstype is btrfs           | Mon Sep  7 18:27:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257573">257573</a>           |  Kill the application pod container when fstype is btrfs           | Fri Sep  4 16:15:07 IST 2020  | Pass |