### 3F07-zfspv-property-modify-ext4

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251840">251840</a>           |  zfspv property runtime modification when fstype is ext4           | Fri Aug 14 19:43:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251568">251568</a>           |  zfspv property runtime modification when fstype is ext4           | Fri Aug 14 11:45:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251544">251544</a>           |  zfspv property runtime modification when fstype is ext4           | Fri Aug 14 10:51:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250272">250272</a>           |  zfspv property runtime modification when fstype is ext4           | Thu Aug 13 10:40:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249607">249607</a>           |  zfspv property runtime modification when fstype is ext4           | Wed Aug 12 21:48:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249492">249492</a>           |  zfspv property runtime modification when fstype is ext4           | Wed Aug 12 19:38:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249408">249408</a>           |  zfspv property runtime modification when fstype is ext4           | Wed Aug 12 17:23:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249126">249126</a>           |  zfspv property runtime modification when fstype is ext4           | Wed Aug 12 11:57:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249103">249103</a>           |  zfspv property runtime modification when fstype is ext4           | Wed Aug 12 10:37:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248769">248769</a>           |  zfspv property runtime modification when fstype is ext4           | Tue Aug 11 17:47:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248263">248263</a>           |  zfspv property runtime modification when fstype is ext4           | Tue Aug 11 10:24:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248210">248210</a>           |  zfspv property runtime modification when fstype is ext4           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247063">247063</a>           |  zfspv property runtime modification when fstype is ext4           | Mon Aug 10 17:51:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246958">246958</a>           |  zfspv property runtime modification when fstype is ext4           | Mon Aug 10 17:04:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246911">246911</a>           |  zfspv property runtime modification when fstype is ext4           | Mon Aug 10 15:35:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246889">246889</a>           |  zfspv property runtime modification when fstype is ext4           | Mon Aug 10 14:20:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245466">245466</a>           |  zfspv property runtime modification when fstype is ext4           | Fri Aug  7 21:23:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245361">245361</a>           |  zfspv property runtime modification when fstype is ext4           | Fri Aug  7 19:29:32 IST 2020  | Pass |

