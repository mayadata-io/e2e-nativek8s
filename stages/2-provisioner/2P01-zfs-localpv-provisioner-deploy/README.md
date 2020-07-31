### 2P01-zfs-localpv-provisioner-deploy

#### Description

This test deploys the zfs-localpv components in the `kube-system` namespace which includes zfs-controller and csi node agent daemonset. Apart from this, storage-classes with different type of file-system for dynamic provisioning of the volumes and volume snapshot class for creation of volume snapshot is also gets created in this test.

#### Steps involved

- First zpool is created on each compute nodes.
- Then apply the zfs-operator file for desired version
- Verify the running state of zfs-localpv components and create storage-classes.
- To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/zfs-localpv-provisioner).

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|