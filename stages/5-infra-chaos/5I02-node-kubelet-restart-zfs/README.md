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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248780">248780</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 18:01:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248274">248274</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 10:39:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248221">248221</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 09:48:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247074">247074</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 18:10:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246969">246969</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 17:18:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246922">246922</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 15:54:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246900">246900</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 14:33:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245477">245477</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 21:39:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245372">245372</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 19:46:32 IST 2020  | Pass |
