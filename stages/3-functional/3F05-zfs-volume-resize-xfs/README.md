### 3F05-zfs-volume-resize-xfs

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as xfs.

#### Steps involved

1. Deploy application `percona-mysql` using xfs file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-properties-verify).
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-volume-resize).
4. Deprovision the application.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292452">292452</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Nov 14 11:41:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290285">290285</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Nov 13 13:12:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290094">290094</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Nov 13 11:20:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290058">290058</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Nov 13 09:24:14 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289832">289832</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Nov 12 20:32:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289797">289797</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Nov 12 18:02:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289344">289344</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Nov 12 08:56:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288883">288883</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Nov 11 16:07:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288849">288849</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Nov 11 12:53:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288814">288814</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Nov 11 10:51:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288700">288700</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Nov 11 08:27:26 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288249">288249</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Nov 10 18:27:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281246">281246</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Oct 15 14:34:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280402">280402</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Oct 14 21:59:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279628">279628</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Oct 14 14:57:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279579">279579</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Oct 14 13:35:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279283">279283</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Oct 14 11:32:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279027">279027</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Oct 14 10:42:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278913">278913</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Oct 13 20:45:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278879">278879</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Oct 13 18:58:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278845">278845</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Oct 13 16:42:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277914">277914</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Oct 12 21:42:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277100">277100</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Oct 12 17:25:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276893">276893</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Oct 12 15:37:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276443">276443</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Oct 10 23:30:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276390">276390</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Oct 10 19:43:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276356">276356</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Oct 10 17:53:49 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276303">276303</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Oct 10 16:52:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276250">276250</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Oct 10 15:26:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274612">274612</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Oct  9 11:23:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274553">274553</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Oct  9 10:18:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271266">271266</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Oct  1 17:19:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268080">268080</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep 22 13:35:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267967">267967</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep 22 11:41:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266910">266910</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Sep 18 16:50:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266571">266571</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Sep 17 11:20:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264783">264783</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep 15 20:21:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264739">264739</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep 15 19:17:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263015">263015</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Sep 14 12:47:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260588">260588</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Sep 11 09:11:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260175">260175</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Sep 10 21:33:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260055">260055</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Sep 10 20:01:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258061">258061</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  8 11:38:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257835">257835</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Sep  7 18:09:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257557">257557</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Sep  4 15:56:46 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257531">257531</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Sep  4 12:02:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257337">257337</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Sep  2 16:14:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257311">257311</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Sep  2 13:39:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257285">257285</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Sep  2 10:20:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257176">257176</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 20:24:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257150">257150</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 19:12:51 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257123">257123</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 13:07:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257098">257098</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Sep  1 12:02:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256990">256990</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 21:15:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256968">256968</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 13:26:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256771">256771</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 09:41:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256748">256748</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 31 07:00:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254803">254803</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 21 16:34:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253793">253793</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 19 16:02:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253178">253178</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sun Aug 16 12:34:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252959">252959</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 23:48:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252934">252934</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 19:46:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252563">252563</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Sat Aug 15 10:31:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251944">251944</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 21:15:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251860">251860</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 20:31:29 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251838">251838</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 19:43:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251566">251566</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 11:44:56 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251542">251542</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug 14 10:51:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250270">250270</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Thu Aug 13 10:40:39 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249605">249605</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 21:48:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249490">249490</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 19:38:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249406">249406</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 17:23:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249124">249124</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 11:57:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249101">249101</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Wed Aug 12 10:40:09 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248767">248767</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 17:47:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248261">248261</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 10:24:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248208">248208</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Tue Aug 11 09:31:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247061">247061</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 17:48:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246956">246956</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 17:04:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246909">246909</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 15:38:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246887">246887</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Mon Aug 10 14:20:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245464">245464</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug  7 21:23:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245359">245359</a>           |  zv property verify and zfs volume resize when fstype is xfs           | Fri Aug  7 19:29:22 IST 2020  | Pass |
