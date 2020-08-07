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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245304">245304</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 15:27:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245282">245282</a>           |  Restart the kubelet services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 14:31:06 IST 2020  | Pass |