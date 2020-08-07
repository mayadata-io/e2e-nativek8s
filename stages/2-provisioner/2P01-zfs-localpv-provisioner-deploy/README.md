### 2P01-zfs-localpv-provisioner-deploy

#### Description

This test deploys the zfs-localpv components in the `kube-system` namespace which includes zfs-controller and csi node agent daemonset. Apart from this, storage-classes with different type of file-system for dynamic provisioning of the volumes and volume snapshot class for creation of volume snapshot are also getting created in this test.

#### Steps involved

- First zpool is created on each compute nodes.
- Then apply the zfs-operator file for desired version
- Verify the running state of zfs-localpv components and create storage-classes.
- To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/experiments/zfs-localpv/zfs-localpv-provisioner).

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245263">245263</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 14:10:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245042">245042</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 12:07:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/244617">244617</a>           |  Provision the zfs-localpv driver           | Fri Aug  7 11:14:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/244617">244617</a>           |  Provision the zfs-localpv driver           | ""  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/244617">244617</a>           |  Provision the zfs-localpv driver           | Fri Aug 7 10:52:27 IST 2020  | Pass |
|        <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/233379">233379</a>        |  Provision the zfs-localpv driver           | Thu Aug 6 19:34:27 IST 2020  | Pass |