### 2P01-zfs-localpv-provisioner-deploy

#### Description

This test deploys the zfs-localpv components in the `kube-system` namespace which includes zfs-controller and csi node agent daemonset. Apart from this, storage-classes with different type of file-system for dynamic provisioning of the volumes and volume snapshot class for creation of volume snapshot are also getting created in this test.

#### Steps involved

- First zpool is created on each compute nodes.
- Then apply the zfs-operator file for desired version
- Verify the running state of zfs-localpv components and create storage-classes.
- To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/zfs-localpv-provisioner).

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267961">267961</a>           |  Provision the zfs-localpv driver           | Tue Sep 22 11:34:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266904">266904</a>           |  Provision the zfs-localpv driver           | Fri Sep 18 16:46:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266876">266876</a>           |  Provision the zfs-localpv driver           | Fri Sep 18 16:28:18 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266565">266565</a>           |  Provision the zfs-localpv driver           | Thu Sep 17 11:15:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266422">266422</a>           |  Provision the zfs-localpv driver           | Wed Sep 16 20:06:45 IST 2020  | Fail |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264777">264777</a>           |  Provision the zfs-localpv driver           | Tue Sep 15 20:16:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264733">264733</a>           |  Provision the zfs-localpv driver           | Tue Sep 15 19:12:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263009">263009</a>           |  Provision the zfs-localpv driver           | Mon Sep 14 12:41:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260582">260582</a>           |  Provision the zfs-localpv driver           | Fri Sep 11 09:05:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260169">260169</a>           |  Provision the zfs-localpv driver           | Thu Sep 10 21:29:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260140">260140</a>           |  Provision the zfs-localpv driver           | Thu Sep 10 21:10:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260049">260049</a>           |  Provision the zfs-localpv driver           | Thu Sep 10 19:55:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258055">258055</a>           |  Provision the zfs-localpv driver           | Tue Sep  8 11:33:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257829">257829</a>           |  Provision the zfs-localpv driver           | Mon Sep  7 18:03:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257551">257551</a>           |  Provision the zfs-localpv driver           | Fri Sep  4 15:51:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257525">257525</a>           |  Provision the zfs-localpv driver           | Fri Sep  4 11:56:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257331">257331</a>           |  Provision the zfs-localpv driver           | Wed Sep  2 16:08:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257305">257305</a>           |  Provision the zfs-localpv driver           | Wed Sep  2 13:34:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257279">257279</a>           |  Provision the zfs-localpv driver           | Wed Sep  2 10:15:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257170">257170</a>           |  Provision the zfs-localpv driver           | Tue Sep  1 20:18:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257144">257144</a>           |  Provision the zfs-localpv driver           | Tue Sep  1 19:07:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257117">257117</a>           |  Provision the zfs-localpv driver           | Tue Sep  1 13:02:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257092">257092</a>           |  Provision the zfs-localpv driver           | Tue Sep  1 11:57:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256984">256984</a>           |  Provision the zfs-localpv driver           | Mon Aug 31 21:09:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256962">256962</a>           |  Provision the zfs-localpv driver           | Mon Aug 31 13:23:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256765">256765</a>           |  Provision the zfs-localpv driver           | Mon Aug 31 09:35:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256742">256742</a>           |  Provision the zfs-localpv driver           | Mon Aug 31 06:54:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254797">254797</a>           |  Provision the zfs-localpv driver           | Fri Aug 21 16:29:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253787">253787</a>           |  Provision the zfs-localpv driver           | Wed Aug 19 15:57:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253172">253172</a>           |  Provision the zfs-localpv driver           | Sun Aug 16 12:28:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252953">252953</a>           |  Provision the zfs-localpv driver           | Sat Aug 15 23:42:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252928">252928</a>           |  Provision the zfs-localpv driver           | Sat Aug 15 19:40:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252557">252557</a>           |  Provision the zfs-localpv driver           | Sat Aug 15 10:28:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251938">251938</a>           |  Provision the zfs-localpv driver           | Fri Aug 14 21:12:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251854">251854</a>           |  Provision the zfs-localpv driver           | Fri Aug 14 20:25:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251832">251832</a>           |  Provision the zfs-localpv driver           | Fri Aug 14 19:37:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251560">251560</a>           |  Provision the zfs-localpv driver           | Fri Aug 14 11:39:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251536">251536</a>           |  Provision the zfs-localpv driver           | Fri Aug 14 10:45:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250264">250264</a>           |  Provision the zfs-localpv driver           | Thu Aug 13 10:34:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249599">249599</a>           |  Provision the zfs-localpv driver           | Wed Aug 12 21:42:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249484">249484</a>           |  Provision the zfs-localpv driver           | Wed Aug 12 19:33:02 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249400">249400</a>           |  Provision the zfs-localpv driver           | Wed Aug 12 17:17:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249118">249118</a>           |  Provision the zfs-localpv driver           | Wed Aug 12 11:51:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249095">249095</a>           |  Provision the zfs-localpv driver           | Wed Aug 12 10:34:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248761">248761</a>           |  Provision the zfs-localpv driver           | Tue Aug 11 17:41:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248255">248255</a>           |  Provision the zfs-localpv driver           | Tue Aug 11 10:18:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248202">248202</a>           |  Provision the zfs-localpv driver           | Tue Aug 11 09:27:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247055">247055</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 17:45:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246950">246950</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 17:01:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246903">246903</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 15:32:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246881">246881</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 14:14:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245458">245458</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 21:17:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245353">245353</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 19:23:42 IST 2020  | Pass |
