### 5I02-node-kubelet-restart-zfs

#### Description

This test restarts the kubelet services on the node on which application is using zfs-local persistent volume. 

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the infra chaos with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254816">254816</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 21 16:48:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253806">253806</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 19 16:19:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253191">253191</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Sun Aug 16 12:49:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252972">252972</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Sun Aug 16 00:05:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252947">252947</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Sat Aug 15 20:15:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252576">252576</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Sat Aug 15 10:49:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251957">251957</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 21:34:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251873">251873</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 20:43:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251851">251851</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 19:56:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251579">251579</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 12:00:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251555">251555</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 11:09:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250283">250283</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Thu Aug 13 10:56:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249618">249618</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 22:05:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249503">249503</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 19:51:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249419">249419</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 17:39:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249137">249137</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 12:10:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249114">249114</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 10:50:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248780">248780</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 18:01:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248274">248274</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 10:39:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248221">248221</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 09:48:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247074">247074</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 18:10:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246969">246969</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 17:18:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246922">246922</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 15:54:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246900">246900</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 14:33:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245477">245477</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 21:39:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245372">245372</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 19:46:32 IST 2020  | Pass |
