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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245460">245460</a>           |  verify the zfspv-custom-topology support           | Fri Aug  7 21:26:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245355">245355</a>           |  verify the zfspv-custom-topology support           | Fri Aug  7 19:29:24 IST 2020  | Pass |
