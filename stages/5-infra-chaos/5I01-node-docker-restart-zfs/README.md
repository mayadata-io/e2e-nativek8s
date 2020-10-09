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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274629">274629</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Oct  9 11:41:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274570">274570</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Oct  9 10:39:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271283">271283</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Thu Oct  1 17:38:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268097">268097</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep 22 13:53:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267984">267984</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep 22 11:59:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266927">266927</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Sep 18 17:10:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266588">266588</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Thu Sep 17 11:42:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264800">264800</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep 15 20:37:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264756">264756</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep 15 19:36:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263032">263032</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Sep 14 13:15:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260605">260605</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Sep 11 09:34:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260192">260192</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Thu Sep 10 21:58:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260072">260072</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Thu Sep 10 20:22:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258078">258078</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep  8 12:06:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257852">257852</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Sep  7 18:33:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257574">257574</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Sep  4 16:21:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257546">257546</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Sep  4 12:25:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257352">257352</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Sep  2 16:32:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257326">257326</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Sep  2 13:59:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257300">257300</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Sep  2 10:43:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257191">257191</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep  1 20:47:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257165">257165</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep  1 19:32:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257138">257138</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep  1 13:23:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257113">257113</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Tue Sep  1 12:24:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257005">257005</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 31 21:37:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256980">256980</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 31 13:39:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256760">256760</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Mon Aug 31 07:27:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254815">254815</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 21 16:48:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253805">253805</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 19 16:20:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253190">253190</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Sun Aug 16 12:49:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252971">252971</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Sun Aug 16 00:05:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252946">252946</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Sat Aug 15 20:15:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252575">252575</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Sat Aug 15 10:49:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251956">251956</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 21:34:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251872">251872</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 20:43:45 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251850">251850</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 19:56:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251578">251578</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 12:00:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251554">251554</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Fri Aug 14 11:09:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250282">250282</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Thu Aug 13 10:56:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249617">249617</a>           |  Restart the docker services on application node and check the behaviour of zfs-localpv           | Wed Aug 12 22:05:28 IST 2020  | Pass |
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
