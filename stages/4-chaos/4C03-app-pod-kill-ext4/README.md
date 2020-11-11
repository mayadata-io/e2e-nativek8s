### 4C03-app-pod-kill-ext4

#### Description

This test kills the container of application pod consuming zfs-localpv backed by ext4 file-system. Pumba tool is used for this test to execute.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the application pod kill test with data-persistence check enabled. To get detailed README for test [click here]()
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288870">288870</a>           |  Kill the application pod container when fstype is ext4           | Wed Nov 11 13:48:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288835">288835</a>           |  Kill the application pod container when fstype is ext4           | Wed Nov 11 11:52:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288721">288721</a>           |  Kill the application pod container when fstype is ext4           | Wed Nov 11 09:20:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288270">288270</a>           |  Kill the application pod container when fstype is ext4           | Tue Nov 10 19:23:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281267">281267</a>           |  Kill the application pod container when fstype is ext4           | Thu Oct 15 15:29:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280423">280423</a>           |  Kill the application pod container when fstype is ext4           | Wed Oct 14 22:57:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279649">279649</a>           |  Kill the application pod container when fstype is ext4           | Wed Oct 14 15:59:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279600">279600</a>           |  Kill the application pod container when fstype is ext4           | Wed Oct 14 14:06:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279304">279304</a>           |  Kill the application pod container when fstype is ext4           | Wed Oct 14 12:30:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278934">278934</a>           |  Kill the application pod container when fstype is ext4           | Tue Oct 13 21:34:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278900">278900</a>           |  Kill the application pod container when fstype is ext4           | Tue Oct 13 19:47:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278866">278866</a>           |  Kill the application pod container when fstype is ext4           | Tue Oct 13 17:35:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277935">277935</a>           |  Kill the application pod container when fstype is ext4           | Mon Oct 12 22:33:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277121">277121</a>           |  Kill the application pod container when fstype is ext4           | Mon Oct 12 18:18:01 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276914">276914</a>           |  Kill the application pod container when fstype is ext4           | Mon Oct 12 16:31:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276464">276464</a>           |  Kill the application pod container when fstype is ext4           | Sun Oct 11 00:18:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276411">276411</a>           |  Kill the application pod container when fstype is ext4           | Sat Oct 10 20:30:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276377">276377</a>           |  Kill the application pod container when fstype is ext4           | Sat Oct 10 18:48:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276324">276324</a>           |  Kill the application pod container when fstype is ext4           | Sat Oct 10 17:31:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276271">276271</a>           |  Kill the application pod container when fstype is ext4           | Sat Oct 10 15:47:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274627">274627</a>           |  Kill the application pod container when fstype is ext4           | Fri Oct  9 11:36:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274568">274568</a>           |  Kill the application pod container when fstype is ext4           | Fri Oct  9 10:34:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271281">271281</a>           |  Kill the application pod container when fstype is ext4           | Thu Oct  1 17:33:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268095">268095</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep 22 13:49:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267982">267982</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep 22 11:55:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266925">266925</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep 18 17:05:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266586">266586</a>           |  Kill the application pod container when fstype is ext4           | Thu Sep 17 11:36:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264798">264798</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep 15 20:33:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264754">264754</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep 15 19:31:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263030">263030</a>           |  Kill the application pod container when fstype is ext4           | Mon Sep 14 13:09:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260603">260603</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep 11 09:28:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260190">260190</a>           |  Kill the application pod container when fstype is ext4           | Thu Sep 10 21:51:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260070">260070</a>           |  Kill the application pod container when fstype is ext4           | Thu Sep 10 20:17:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258076">258076</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  8 11:59:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257850">257850</a>           |  Kill the application pod container when fstype is ext4           | Mon Sep  7 18:27:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257572">257572</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep  4 16:15:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257545">257545</a>           |  Kill the application pod container when fstype is ext4           | Fri Sep  4 12:19:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257351">257351</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 16:28:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257325">257325</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 13:54:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257299">257299</a>           |  Kill the application pod container when fstype is ext4           | Wed Sep  2 10:38:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257190">257190</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 20:42:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257164">257164</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 19:27:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257137">257137</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 13:18:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257112">257112</a>           |  Kill the application pod container when fstype is ext4           | Tue Sep  1 12:20:19 IST 2020  | Pass |