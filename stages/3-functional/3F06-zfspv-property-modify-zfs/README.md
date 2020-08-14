### 3F06-zfspv-property-modify-zfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is zfs.

#### Steps involved

1. Deploy application `percona-mysql` using zfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251543">251543</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug 14 10:48:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250271">250271</a>           |  zfspv property runtime modification when fstype is zfs           | Thu Aug 13 10:40:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249606">249606</a>           |  zfspv property runtime modification when fstype is zfs           | Wed Aug 12 21:46:00 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249491">249491</a>           |  zfspv property runtime modification when fstype is zfs           | Wed Aug 12 19:38:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249407">249407</a>           |  zfspv property runtime modification when fstype is zfs           | Wed Aug 12 17:23:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249125">249125</a>           |  zfspv property runtime modification when fstype is zfs           | Wed Aug 12 11:57:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249102">249102</a>           |  zfspv property runtime modification when fstype is zfs           | Wed Aug 12 10:40:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248768">248768</a>           |  zfspv property runtime modification when fstype is zfs           | Tue Aug 11 17:45:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248262">248262</a>           |  zfspv property runtime modification when fstype is zfs           | Tue Aug 11 10:24:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248209">248209</a>           |  zfspv property runtime modification when fstype is zfs           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247062">247062</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 17:51:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246957">246957</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 17:04:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246910">246910</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 15:38:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246888">246888</a>           |  zfspv property runtime modification when fstype is zfs           | Mon Aug 10 14:20:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245465">245465</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 21:23:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245360">245360</a>           |  zfspv property runtime modification when fstype is zfs           | Fri Aug  7 19:29:27 IST 2020  | Pass |
