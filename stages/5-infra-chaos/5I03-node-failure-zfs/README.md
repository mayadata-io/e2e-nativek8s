### 5I03-node-failure-zfs

#### Description

This test fails the node on which zfs-localpv is provisioned. For this we first power off that particular machine on ESX and after some time we again power on it. In this process behaviour of zfs-localpv is observed.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the infra chaos with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264758">264758</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Tue Sep 15 19:36:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263034">263034</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Mon Sep 14 13:15:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260607">260607</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Fri Sep 11 09:33:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260194">260194</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Thu Sep 10 21:58:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260074">260074</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Thu Sep 10 20:22:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258080">258080</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Tue Sep  8 12:06:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257854">257854</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Mon Sep  7 18:33:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257576">257576</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Fri Sep  4 16:21:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257548">257548</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Fri Sep  4 12:25:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257354">257354</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Wed Sep  2 16:32:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257328">257328</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Wed Sep  2 13:59:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257302">257302</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Wed Sep  2 10:43:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257193">257193</a>           |  Power off and on the worker node machine where volume is provisioned and check the behaviour of zfs-localpv           | Tue Sep  1 20:47:26 IST 2020  | Pass |