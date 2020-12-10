### 3F12-zfspv-snapshot-clone-xfs-create

#### Description

This test takes the zfs volume snapshot and later use that snapshot to create clone volumes when application is deployed with xfs file-system on top of zfs-localpv.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Apply tpcc loadgen on application
3. Run the test for creating the volume snapshot after dumping some data into the application mount point. For detailed README of this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-snapshot).
4. Run the test for creating the clone volumes from the snapshot created before and mount this clone volume into the different `percona-mysql` application pod. And then verify if data consistency is maintained. For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-clone).
5. Deprovision the clone volume and its application.
6. Delete the volume snapshot.
7. Deprovision the application and parent volume.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/303004">303004</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Dec 10 12:34:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/302425">302425</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Dec  9 12:34:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300979">300979</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Dec  5 10:56:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300754">300754</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Dec  4 18:13:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300720">300720</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Dec  4 16:44:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300573">300573</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Dec  4 13:43:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300539">300539</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Dec  4 11:26:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299806">299806</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Dec  2 21:35:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299772">299772</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Dec  2 17:02:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299736">299736</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Dec  2 11:28:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299301">299301</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Nov 30 21:38:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/294395">294395</a>           |  create volume snapshot and clone when fstype is xfs           | Sun Nov 15 14:19:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292902">292902</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Nov 14 17:44:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292542">292542</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Nov 14 13:43:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292459">292459</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Nov 14 11:44:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290292">290292</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Nov 13 13:14:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290101">290101</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Nov 13 11:22:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290065">290065</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Nov 13 09:24:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289839">289839</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Nov 12 20:32:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289804">289804</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Nov 12 18:02:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289351">289351</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Nov 12 08:56:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288890">288890</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Nov 11 16:10:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288856">288856</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Nov 11 12:53:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288821">288821</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Nov 11 10:54:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288707">288707</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Nov 11 08:27:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288256">288256</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Nov 10 18:27:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281253">281253</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Oct 15 14:31:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280409">280409</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Oct 14 22:01:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279635">279635</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Oct 14 15:00:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279586">279586</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Oct 14 13:35:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279290">279290</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Oct 14 11:35:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279034">279034</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Oct 14 10:43:12 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278920">278920</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Oct 13 20:45:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278886">278886</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Oct 13 18:58:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278852">278852</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Oct 13 16:45:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277921">277921</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Oct 12 21:42:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277107">277107</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Oct 12 17:26:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276900">276900</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Oct 12 15:37:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276450">276450</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Oct 10 23:30:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276397">276397</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Oct 10 19:41:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276363">276363</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Oct 10 17:56:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276310">276310</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Oct 10 16:50:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276257">276257</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Oct 10 15:28:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274619">274619</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Oct  9 11:23:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274560">274560</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Oct  9 10:19:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271273">271273</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Oct  1 17:19:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268087">268087</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep 22 13:35:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267974">267974</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep 22 11:38:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266917">266917</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep 18 16:49:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266578">266578</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Sep 17 11:21:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264790">264790</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep 15 20:21:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264746">264746</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep 15 19:17:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263022">263022</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Sep 14 12:47:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260595">260595</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep 11 09:11:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260182">260182</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Sep 10 21:32:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260062">260062</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Sep 10 20:01:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258068">258068</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  8 11:38:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257842">257842</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Sep  7 18:09:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257564">257564</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep  4 15:56:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257538">257538</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Sep  4 12:02:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257344">257344</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 16:14:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257318">257318</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 13:40:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257292">257292</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Sep  2 10:20:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257183">257183</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 20:24:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257157">257157</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 19:13:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257130">257130</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 13:07:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257105">257105</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Sep  1 12:02:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256997">256997</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 21:15:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256975">256975</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 13:28:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256778">256778</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 09:41:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256755">256755</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 31 07:00:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254810">254810</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 21 16:34:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253800">253800</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 19 16:03:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253185">253185</a>           |  create volume snapshot and clone when fstype is xfs           | Sun Aug 16 12:34:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252966">252966</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 23:48:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252941">252941</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 19:46:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252570">252570</a>           |  create volume snapshot and clone when fstype is xfs           | Sat Aug 15 10:34:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251951">251951</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 21:18:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251867">251867</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 20:31:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251845">251845</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 19:43:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251573">251573</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 11:45:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251549">251549</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug 14 10:51:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250277">250277</a>           |  create volume snapshot and clone when fstype is xfs           | Thu Aug 13 10:38:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249612">249612</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 21:48:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249497">249497</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 19:38:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249413">249413</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 17:23:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249131">249131</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 11:57:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249108">249108</a>           |  create volume snapshot and clone when fstype is xfs           | Wed Aug 12 10:40:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248774">248774</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 17:47:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248268">248268</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 10:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248215">248215</a>           |  create volume snapshot and clone when fstype is xfs           | Tue Aug 11 09:33:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247068">247068</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 17:51:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246963">246963</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 17:06:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246916">246916</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 15:38:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246894">246894</a>           |  create volume snapshot and clone when fstype is xfs           | Mon Aug 10 14:20:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245471">245471</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 21:23:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245366">245366</a>           |  create volume snapshot and clone when fstype is xfs           | Fri Aug  7 19:29:37 IST 2020  | Pass |
