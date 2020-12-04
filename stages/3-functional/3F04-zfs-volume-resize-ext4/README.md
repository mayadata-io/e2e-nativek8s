### 3F04-zfs-volume-resize-ext4

#### Description

This functional test verifies the csi volume resize feature when application which is using this volume is deployed with fstype as ext4.

#### Steps involved

1. Deploy application `percona-mysql` using ext4 file system on top of zfs-localpv
2. Verify the zfspv properties set via storage-class.  To know more about this [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zv-properties-verify).
3. Run the functional test for volume resize with data-persistence check enabled. To get detailed README for test [click here](https://github.com/openebs/e2e-tests/tree/master/experiments/zfs-localpv/functional/zfs-volume-resize).
4. Deprovision the application

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300746">300746</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Dec  4 18:13:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300712">300712</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Dec  4 16:46:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300565">300565</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Dec  4 13:43:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/300531">300531</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Dec  4 11:23:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299798">299798</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Dec  2 21:35:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299764">299764</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Dec  2 17:02:01 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299728">299728</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Dec  2 11:28:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/299293">299293</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Nov 30 21:38:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/294387">294387</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sun Nov 15 14:19:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292894">292894</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Nov 14 17:44:03 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292534">292534</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Nov 14 13:43:42 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/292451">292451</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Nov 14 11:41:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290284">290284</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Nov 13 13:14:47 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290093">290093</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Nov 13 11:22:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/290057">290057</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Nov 13 09:24:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289831">289831</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Nov 12 20:32:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289796">289796</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Nov 12 18:02:38 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/289343">289343</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Nov 12 08:56:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288882">288882</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Nov 11 16:10:16 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288848">288848</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Nov 11 12:53:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288813">288813</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Nov 11 10:54:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288699">288699</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Nov 11 08:24:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/288248">288248</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Nov 10 18:24:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/281245">281245</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Oct 15 14:34:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/280401">280401</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Oct 14 21:59:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279627">279627</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Oct 14 15:00:11 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279578">279578</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Oct 14 13:35:37 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279282">279282</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Oct 14 11:35:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/279026">279026</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Oct 14 10:42:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278912">278912</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Oct 13 20:45:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278878">278878</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Oct 13 18:58:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/278844">278844</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Oct 13 16:45:43 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277913">277913</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Oct 12 21:42:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/277099">277099</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Oct 12 17:26:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276892">276892</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Oct 12 15:34:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276442">276442</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Oct 10 23:30:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276389">276389</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Oct 10 19:43:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276355">276355</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Oct 10 17:53:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276302">276302</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Oct 10 16:52:34 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/276249">276249</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Oct 10 15:26:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274611">274611</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Oct  9 11:23:40 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/274552">274552</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Oct  9 10:18:54 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/271265">271265</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Oct  1 17:19:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/268079">268079</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 22 13:35:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/267966">267966</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 22 11:41:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266909">266909</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep 18 16:50:17 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/266570">266570</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Sep 17 11:21:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264782">264782</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 15 20:21:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/264738">264738</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep 15 19:15:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/263014">263014</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Sep 14 12:47:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260587">260587</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep 11 09:11:20 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260174">260174</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Sep 10 21:33:30 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/260054">260054</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Sep 10 20:01:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/258060">258060</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  8 11:38:50 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257834">257834</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Sep  7 18:09:07 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257556">257556</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep  4 15:56:48 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257530">257530</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Sep  4 12:02:36 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257336">257336</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 16:14:05 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257310">257310</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 13:39:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257284">257284</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Sep  2 10:20:32 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257175">257175</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 20:24:18 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257149">257149</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 19:12:52 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257122">257122</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 13:07:45 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/257097">257097</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Sep  1 12:02:44 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256989">256989</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 21:15:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256967">256967</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 13:26:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256770">256770</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 09:41:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256747">256747</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 31 07:00:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254802">254802</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 21 16:35:04 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253792">253792</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 19 16:03:13 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253177">253177</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sun Aug 16 12:34:23 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252958">252958</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 23:48:31 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252933">252933</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 19:45:55 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252562">252562</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Sat Aug 15 10:31:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251943">251943</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 21:18:06 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251859">251859</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 20:31:10 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251837">251837</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 19:43:19 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251565">251565</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 11:44:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251541">251541</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug 14 10:51:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250269">250269</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Thu Aug 13 10:40:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249604">249604</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 21:48:22 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249489">249489</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 19:38:28 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249405">249405</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 17:22:59 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249123">249123</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 11:57:25 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249100">249100</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Wed Aug 12 10:40:08 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248766">248766</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 17:47:41 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248260">248260</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 10:24:12 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248207">248207</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Tue Aug 11 09:33:27 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247060">247060</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 17:51:15 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246955">246955</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 17:04:21 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246908">246908</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 15:37:58 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246886">246886</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Mon Aug 10 14:20:53 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245463">245463</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 21:23:33 IST 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245358">245358</a>           |  zv property verify and zfs volume resize when fstype is ext4           | Fri Aug  7 19:29:36 IST 2020  | Pass |
