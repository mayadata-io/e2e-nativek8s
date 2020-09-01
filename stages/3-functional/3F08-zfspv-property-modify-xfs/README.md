### 3F08-zfspv-property-modify-xfs

#### Description

This functional test validates the successful modification of zfspv properties after provisioning the volume when fstype used for application is xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Run the test for zfspv-property-modify. To get the detailed README for this test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-property-runtime-modify).
3. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257126">257126</a>           |  zfspv property runtime modification when fstype is xfs           | Tue Sep  1 13:07:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257101">257101</a>           |  zfspv property runtime modification when fstype is xfs           | Tue Sep  1 12:02:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256993">256993</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 31 21:15:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256971">256971</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 31 13:26:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256774">256774</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 31 09:41:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256751">256751</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 31 06:57:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254806">254806</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 21 16:34:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253796">253796</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 19 16:00:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253181">253181</a>           |  zfspv property runtime modification when fstype is xfs           | Sun Aug 16 12:34:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252962">252962</a>           |  zfspv property runtime modification when fstype is xfs           | Sat Aug 15 23:46:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252937">252937</a>           |  zfspv property runtime modification when fstype is xfs           | Sat Aug 15 19:46:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252566">252566</a>           |  zfspv property runtime modification when fstype is xfs           | Sat Aug 15 10:31:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251947">251947</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 14 21:18:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251863">251863</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 14 20:31:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251841">251841</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 14 19:43:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251569">251569</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 14 11:45:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251545">251545</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug 14 10:51:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250273">250273</a>           |  zfspv property runtime modification when fstype is xfs           | Thu Aug 13 10:40:35 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249608">249608</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 12 21:48:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249493">249493</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 12 19:38:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249409">249409</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 12 17:20:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249127">249127</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 12 11:57:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249104">249104</a>           |  zfspv property runtime modification when fstype is xfs           | Wed Aug 12 10:40:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248770">248770</a>           |  zfspv property runtime modification when fstype is xfs           | Tue Aug 11 17:47:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248264">248264</a>           |  zfspv property runtime modification when fstype is xfs           | Tue Aug 11 10:24:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248211">248211</a>           |  zfspv property runtime modification when fstype is xfs           | Tue Aug 11 09:33:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247064">247064</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 10 17:51:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246959">246959</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 10 17:04:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246912">246912</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 10 15:38:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246890">246890</a>           |  zfspv property runtime modification when fstype is xfs           | Mon Aug 10 14:20:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245467">245467</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug  7 21:23:24 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245362">245362</a>           |  zfspv property runtime modification when fstype is xfs           | Fri Aug  7 19:29:37 IST 2020  | Pass |
