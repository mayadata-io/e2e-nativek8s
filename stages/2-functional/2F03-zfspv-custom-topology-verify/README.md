### 2F03-zfspv-custom-topology-verify

#### Description

This functional test validates the custom-topology support for zfs-localpv, where it verifies that volume provisioning is done on only such nodes which are labeled with custom-topology supported via storage-class.

#### Steps involved

- First we label the nodes and then provision the volume when volumeBindingMode is immediate
- Then verify that volume is provisioned on labeled nodes only.
- Secondly we label the nodes and then provision the volume when volumeBindingMode is WaitForFirstConsumer. In this case we need to restart the csi nodes so that csi nodes get aware of the labels.
- Again verify that volume is provisioned on labeled nodes only.
- For detailed README for this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/functional/zfspv-custom-topology)

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|