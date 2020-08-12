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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249502">249502</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 19:51:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249418">249418</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 17:39:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249136">249136</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 12:10:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249113">249113</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 10:50:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248779">248779</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 18:01:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248273">248273</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 10:39:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248220">248220</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Aug 11 09:48:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247073">247073</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 18:10:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246968">246968</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 17:18:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246921">246921</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 15:54:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246899">246899</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 10 14:33:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245476">245476</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 21:39:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245371">245371</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug  7 19:46:37 IST 2020  | Pass |
