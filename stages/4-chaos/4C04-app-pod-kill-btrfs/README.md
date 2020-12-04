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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300769">300769</a>           |  Kill the application pod container when fstype is btrfs           | Fri Dec  4 19:01:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300735">300735</a>           |  Kill the application pod container when fstype is btrfs           | Fri Dec  4 17:37:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300588">300588</a>           |  Kill the application pod container when fstype is btrfs           | Fri Dec  4 14:32:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300554">300554</a>           |  Kill the application pod container when fstype is btrfs           | Fri Dec  4 12:11:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299821">299821</a>           |  Kill the application pod container when fstype is btrfs           | Wed Dec  2 22:25:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299787">299787</a>           |  Kill the application pod container when fstype is btrfs           | Wed Dec  2 18:14:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299751">299751</a>           |  Kill the application pod container when fstype is btrfs           | Wed Dec  2 12:43:07 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299316">299316</a>           |  Kill the application pod container when fstype is btrfs           | Mon Nov 30 22:21:36 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/294410">294410</a>           |  Kill the application pod container when fstype is btrfs           | Sun Nov 15 15:31:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292917">292917</a>           |  Kill the application pod container when fstype is btrfs           | Sat Nov 14 19:00:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292557">292557</a>           |  Kill the application pod container when fstype is btrfs           | Sat Nov 14 14:39:09 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292474">292474</a>           |  Kill the application pod container when fstype is btrfs           | Sat Nov 14 12:42:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290307">290307</a>           |  Kill the application pod container when fstype is btrfs           | Fri Nov 13 14:12:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290116">290116</a>           |  Kill the application pod container when fstype is btrfs           | Fri Nov 13 12:17:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290080">290080</a>           |  Kill the application pod container when fstype is btrfs           | Fri Nov 13 10:16:01 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289854">289854</a>           |  Kill the application pod container when fstype is btrfs           | Thu Nov 12 21:27:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289819">289819</a>           |  Kill the application pod container when fstype is btrfs           | Thu Nov 12 19:13:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289366">289366</a>           |  Kill the application pod container when fstype is btrfs           | Thu Nov 12 09:59:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288905">288905</a>           |  Kill the application pod container when fstype is btrfs           | Wed Nov 11 17:04:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288871">288871</a>           |  Kill the application pod container when fstype is btrfs           | Wed Nov 11 13:48:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288836">288836</a>           |  Kill the application pod container when fstype is btrfs           | Wed Nov 11 11:51:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288722">288722</a>           |  Kill the application pod container when fstype is btrfs           | Wed Nov 11 09:20:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288271">288271</a>           |  Kill the application pod container when fstype is btrfs           | Tue Nov 10 19:23:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281268">281268</a>           |  Kill the application pod container when fstype is btrfs           | Thu Oct 15 15:29:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280424">280424</a>           |  Kill the application pod container when fstype is btrfs           | Wed Oct 14 22:57:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279650">279650</a>           |  Kill the application pod container when fstype is btrfs           | Wed Oct 14 15:59:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279601">279601</a>           |  Kill the application pod container when fstype is btrfs           | Wed Oct 14 14:06:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279305">279305</a>           |  Kill the application pod container when fstype is btrfs           | Wed Oct 14 12:30:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278935">278935</a>           |  Kill the application pod container when fstype is btrfs           | Tue Oct 13 21:34:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278901">278901</a>           |  Kill the application pod container when fstype is btrfs           | Tue Oct 13 19:47:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278867">278867</a>           |  Kill the application pod container when fstype is btrfs           | Tue Oct 13 17:35:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277936">277936</a>           |  Kill the application pod container when fstype is btrfs           | Mon Oct 12 22:33:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277122">277122</a>           |  Kill the application pod container when fstype is btrfs           | Mon Oct 12 18:18:02 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276915">276915</a>           |  Kill the application pod container when fstype is btrfs           | Mon Oct 12 16:31:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276465">276465</a>           |  Kill the application pod container when fstype is btrfs           | Sun Oct 11 00:18:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276412">276412</a>           |  Kill the application pod container when fstype is btrfs           | Sat Oct 10 20:31:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276378">276378</a>           |  Kill the application pod container when fstype is btrfs           | Sat Oct 10 18:48:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276325">276325</a>           |  Kill the application pod container when fstype is btrfs           | Sat Oct 10 17:31:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276272">276272</a>           |  Kill the application pod container when fstype is btrfs           | Sat Oct 10 15:48:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274628">274628</a>           |  Kill the application pod container when fstype is btrfs           | Fri Oct  9 11:36:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274569">274569</a>           |  Kill the application pod container when fstype is btrfs           | Fri Oct  9 10:34:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271282">271282</a>           |  Kill the application pod container when fstype is btrfs           | Thu Oct  1 17:33:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268096">268096</a>           |  Kill the application pod container when fstype is btrfs           | Tue Sep 22 13:49:03 IST 2020  | Pass |
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