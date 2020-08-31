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
