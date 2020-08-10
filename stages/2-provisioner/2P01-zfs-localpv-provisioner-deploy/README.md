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
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246950">246950</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 17:01:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246903">246903</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 15:32:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246881">246881</a>           |  Provision the zfs-localpv driver           | Mon Aug 10 14:14:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245458">245458</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 21:17:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245353">245353</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 19:23:42 IST 2020  | Pass |
