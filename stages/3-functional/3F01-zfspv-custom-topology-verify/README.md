### 3F01-zfspv-custom-topology-verify

#### Description

This functional test validates the custom-topology support for zfs-localpv, where it verifies that volume provisioning is done on only such nodes which are labeled with custom-topology supported via storage-class.

#### Steps involved

- First we label the nodes and then provision the volume when volumeBindingMode is immediate
- Then verify that volume is provisioned on labeled nodes only.
- Secondly we label the nodes and then provision the volume when volumeBindingMode is WaitForFirstConsumer. In this case we need to restart the csi nodes so that csi nodes get aware of the labels.
- Again verify that volume is provisioned on labeled nodes only.
- For detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfspv-custom-topology).

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289828">289828</a>           |  verify the zfspv-custom-topology support           | Thu Nov 12 20:34:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289793">289793</a>           |  verify the zfspv-custom-topology support           | Thu Nov 12 18:05:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289679">289679</a>           |  verify the zfspv-custom-topology support           | Thu Nov 12 17:05:32 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289340">289340</a>           |  verify the zfspv-custom-topology support           | Thu Nov 12 08:59:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288879">288879</a>           |  verify the zfspv-custom-topology support           | Wed Nov 11 16:12:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288845">288845</a>           |  verify the zfspv-custom-topology support           | Wed Nov 11 12:54:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288810">288810</a>           |  verify the zfspv-custom-topology support           | Wed Nov 11 10:56:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288696">288696</a>           |  verify the zfspv-custom-topology support           | Wed Nov 11 08:30:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288470">288470</a>           |  verify the zfspv-custom-topology support           | Tue Nov 10 22:24:11 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288245">288245</a>           |  verify the zfspv-custom-topology support           | Tue Nov 10 18:30:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281242">281242</a>           |  verify the zfspv-custom-topology support           | Thu Oct 15 14:37:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280398">280398</a>           |  verify the zfspv-custom-topology support           | Wed Oct 14 22:02:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279624">279624</a>           |  verify the zfspv-custom-topology support           | Wed Oct 14 15:03:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279575">279575</a>           |  verify the zfspv-custom-topology support           | Wed Oct 14 13:38:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279279">279279</a>           |  verify the zfspv-custom-topology support           | Wed Oct 14 11:37:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279023">279023</a>           |  verify the zfspv-custom-topology support           | Wed Oct 14 10:45:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278909">278909</a>           |  verify the zfspv-custom-topology support           | Tue Oct 13 20:47:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278875">278875</a>           |  verify the zfspv-custom-topology support           | Tue Oct 13 19:01:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278841">278841</a>           |  verify the zfspv-custom-topology support           | Tue Oct 13 16:48:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277910">277910</a>           |  verify the zfspv-custom-topology support           | Mon Oct 12 21:45:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277096">277096</a>           |  verify the zfspv-custom-topology support           | Mon Oct 12 17:28:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276889">276889</a>           |  verify the zfspv-custom-topology support           | Mon Oct 12 15:39:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276439">276439</a>           |  verify the zfspv-custom-topology support           | Sat Oct 10 23:32:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276386">276386</a>           |  verify the zfspv-custom-topology support           | Sat Oct 10 19:46:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276352">276352</a>           |  verify the zfspv-custom-topology support           | Sat Oct 10 17:56:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276299">276299</a>           |  verify the zfspv-custom-topology support           | Sat Oct 10 16:55:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276246">276246</a>           |  verify the zfspv-custom-topology support           | Sat Oct 10 15:28:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274608">274608</a>           |  verify the zfspv-custom-topology support           | Fri Oct  9 11:23:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274549">274549</a>           |  verify the zfspv-custom-topology support           | Fri Oct  9 10:21:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271262">271262</a>           |  verify the zfspv-custom-topology support           | Thu Oct  1 17:22:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268076">268076</a>           |  verify the zfspv-custom-topology support           | Tue Sep 22 13:37:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267963">267963</a>           |  verify the zfspv-custom-topology support           | Tue Sep 22 11:44:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266906">266906</a>           |  verify the zfspv-custom-topology support           | Fri Sep 18 16:53:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266878">266878</a>           |  verify the zfspv-custom-topology support           | Fri Sep 18 16:32:28 IST 2020  | none |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266567">266567</a>           |  verify the zfspv-custom-topology support           | Thu Sep 17 11:23:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266424">266424</a>           |  verify the zfspv-custom-topology support           | Wed Sep 16 20:23:50 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264779">264779</a>           |  verify the zfspv-custom-topology support           | Tue Sep 15 20:21:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264735">264735</a>           |  verify the zfspv-custom-topology support           | Tue Sep 15 19:20:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263011">263011</a>           |  verify the zfspv-custom-topology support           | Mon Sep 14 12:51:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260584">260584</a>           |  verify the zfspv-custom-topology support           | Fri Sep 11 09:15:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260171">260171</a>           |  verify the zfspv-custom-topology support           | Thu Sep 10 21:37:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260142">260142</a>           |  verify the zfspv-custom-topology support           | Thu Sep 10 21:18:08 IST 2020  | none |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260051">260051</a>           |  verify the zfspv-custom-topology support           | Thu Sep 10 20:04:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258057">258057</a>           |  verify the zfspv-custom-topology support           | Tue Sep  8 11:42:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257831">257831</a>           |  verify the zfspv-custom-topology support           | Mon Sep  7 18:10:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257553">257553</a>           |  verify the zfspv-custom-topology support           | Fri Sep  4 15:59:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257527">257527</a>           |  verify the zfspv-custom-topology support           | Fri Sep  4 12:05:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257333">257333</a>           |  verify the zfspv-custom-topology support           | Wed Sep  2 16:16:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257307">257307</a>           |  verify the zfspv-custom-topology support           | Wed Sep  2 13:39:57 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257281">257281</a>           |  verify the zfspv-custom-topology support           | Wed Sep  2 10:23:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257172">257172</a>           |  verify the zfspv-custom-topology support           | Tue Sep  1 20:26:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257146">257146</a>           |  verify the zfspv-custom-topology support           | Tue Sep  1 19:12:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257119">257119</a>           |  verify the zfspv-custom-topology support           | Tue Sep  1 13:07:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257094">257094</a>           |  verify the zfspv-custom-topology support           | Tue Sep  1 12:05:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256986">256986</a>           |  verify the zfspv-custom-topology support           | Mon Aug 31 21:17:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256964">256964</a>           |  verify the zfspv-custom-topology support           | Mon Aug 31 13:28:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256767">256767</a>           |  verify the zfspv-custom-topology support           | Mon Aug 31 09:56:44 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256744">256744</a>           |  verify the zfspv-custom-topology support           | Mon Aug 31 07:15:41 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254799">254799</a>           |  verify the zfspv-custom-topology support           | Fri Aug 21 16:37:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253789">253789</a>           |  verify the zfspv-custom-topology support           | Wed Aug 19 16:05:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253174">253174</a>           |  verify the zfspv-custom-topology support           | Sun Aug 16 12:36:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252955">252955</a>           |  verify the zfspv-custom-topology support           | Sat Aug 15 23:50:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252930">252930</a>           |  verify the zfspv-custom-topology support           | Sat Aug 15 20:01:06 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252559">252559</a>           |  verify the zfspv-custom-topology support           | Sat Aug 15 10:34:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251940">251940</a>           |  verify the zfspv-custom-topology support           | Fri Aug 14 21:18:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251856">251856</a>           |  verify the zfspv-custom-topology support           | Fri Aug 14 20:31:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251834">251834</a>           |  verify the zfspv-custom-topology support           | Fri Aug 14 19:43:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251562">251562</a>           |  verify the zfspv-custom-topology support           | Fri Aug 14 11:45:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251538">251538</a>           |  verify the zfspv-custom-topology support           | Fri Aug 14 10:53:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250266">250266</a>           |  verify the zfspv-custom-topology support           | Thu Aug 13 10:43:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249601">249601</a>           |  verify the zfspv-custom-topology support           | Wed Aug 12 21:50:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249486">249486</a>           |  verify the zfspv-custom-topology support           | Wed Aug 12 19:38:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249402">249402</a>           |  verify the zfspv-custom-topology support           | Wed Aug 12 17:23:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249120">249120</a>           |  verify the zfspv-custom-topology support           | Wed Aug 12 11:57:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249097">249097</a>           |  verify the zfspv-custom-topology support           | Wed Aug 12 10:40:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248763">248763</a>           |  verify the zfspv-custom-topology support           | Tue Aug 11 17:47:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248257">248257</a>           |  verify the zfspv-custom-topology support           | Tue Aug 11 10:24:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248204">248204</a>           |  verify the zfspv-custom-topology support           | Tue Aug 11 09:35:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247057">247057</a>           |  verify the zfspv-custom-topology support           | Mon Aug 10 17:53:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246952">246952</a>           |  verify the zfspv-custom-topology support           | Mon Aug 10 17:06:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246905">246905</a>           |  verify the zfspv-custom-topology support           | Mon Aug 10 15:40:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246883">246883</a>           |  verify the zfspv-custom-topology support           | Mon Aug 10 14:20:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245460">245460</a>           |  verify the zfspv-custom-topology support           | Fri Aug  7 21:26:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245355">245355</a>           |  verify the zfspv-custom-topology support           | Fri Aug  7 19:29:24 IST 2020  | Pass |
