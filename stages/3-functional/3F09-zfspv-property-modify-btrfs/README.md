### 3F09-zfspv-property-modify-btrfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is btrfs.

#### Steps involved

1. Deploy application `percona-mysql` using btrfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249494">249494</a>           |  zfspv property runtime modification when fstype is btrfs           | Wed Aug 12 19:36:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249410">249410</a>           |  zfspv property runtime modification when fstype is btrfs           | Wed Aug 12 17:23:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249128">249128</a>           |  zfspv property runtime modification when fstype is btrfs           | Wed Aug 12 11:57:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249105">249105</a>           |  zfspv property runtime modification when fstype is btrfs           | Wed Aug 12 10:40:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248771">248771</a>           |  zfspv property runtime modification when fstype is btrfs           | Tue Aug 11 17:47:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248265">248265</a>           |  zfspv property runtime modification when fstype is btrfs           | Tue Aug 11 10:24:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248212">248212</a>           |  zfspv property runtime modification when fstype is btrfs           | Tue Aug 11 09:33:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247065">247065</a>           |  zfspv property runtime modification when fstype is btrfs           | Mon Aug 10 17:51:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246960">246960</a>           |  zfspv property runtime modification when fstype is btrfs           | Mon Aug 10 17:04:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246913">246913</a>           |  zfspv property runtime modification when fstype is btrfs           | Mon Aug 10 15:35:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246891">246891</a>           |  zfspv property runtime modification when fstype is btrfs           | Mon Aug 10 14:20:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245468">245468</a>           |  zfspv property runtime modification when fstype is btrfs           | Fri Aug  7 21:21:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245363">245363</a>           |  zfspv property runtime modification when fstype is btrfs           | Fri Aug  7 19:29:37 IST 2020  | Pass |

