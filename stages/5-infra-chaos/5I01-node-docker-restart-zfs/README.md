### 5I01-node-docker-restart-zfs

#### Description

This test restarts the docker services on the node on which application is using zfs-local persistent volume. 

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the infra chaos with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246921">246921</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 15:54:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246899">246899</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 14:33:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245476">245476</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 21:39:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245371">245371</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 19:46:37 IST 2020  | Pass |
