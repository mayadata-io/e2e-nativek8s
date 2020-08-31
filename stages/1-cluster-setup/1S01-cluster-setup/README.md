### 1S01-cluster-setup

#### Description
 
This test checks the health of the cluster, status of nodes and clones the required github repositories for performing zfs-localpv related functional and chaos (and infra-chaos) testing.

#### Prerequisites

- The host machines should be created and have the dependent packages installed in all the machines.
- All kubernetes nodes should be in ready state which will be verified by `kubectl get nodes` command to get their status.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/256741">256741</a>           |  Configure the cluster and get it ready           | Mon Aug 31 01:21:06 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/254796">254796</a>           |  Configure the cluster and get it ready           | Fri Aug 21 10:55:26 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253786">253786</a>           |  Configure the cluster and get it ready           | Wed Aug 19 10:23:55 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/253171">253171</a>           |  Configure the cluster and get it ready           | Sun Aug 16 06:53:48 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252952">252952</a>           |  Configure the cluster and get it ready           | Sat Aug 15 18:08:55 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252927">252927</a>           |  Configure the cluster and get it ready           | Sat Aug 15 14:06:40 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/252556">252556</a>           |  Configure the cluster and get it ready           | Sat Aug 15 04:54:22 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251937">251937</a>           |  Configure the cluster and get it ready           | Fri Aug 14 15:38:18 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251853">251853</a>           |  Configure the cluster and get it ready           | Fri Aug 14 14:51:21 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251831">251831</a>           |  Configure the cluster and get it ready           | Fri Aug 14 14:02:59 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251559">251559</a>           |  Configure the cluster and get it ready           | Fri Aug 14 06:05:24 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/251535">251535</a>           |  Configure the cluster and get it ready           | Fri Aug 14 05:11:52 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/250263">250263</a>           |  Configure the cluster and get it ready           | Thu Aug 13 05:01:37 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249598">249598</a>           |  Configure the cluster and get it ready           | Wed Aug 12 16:08:45 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249483">249483</a>           |  Configure the cluster and get it ready           | Wed Aug 12 13:59:19 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249399">249399</a>           |  Configure the cluster and get it ready           | Wed Aug 12 11:43:36 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249117">249117</a>           |  Configure the cluster and get it ready           | Wed Aug 12 06:18:00 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/249094">249094</a>           |  Configure the cluster and get it ready           | Wed Aug 12 05:01:11 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248760">248760</a>           |  Configure the cluster and get it ready           | Tue Aug 11 12:07:34 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248254">248254</a>           |  Configure the cluster and get it ready           | Tue Aug 11 04:44:49 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/248201">248201</a>           |  Configure the cluster and get it ready           | Tue Aug 11 03:54:05 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/247054">247054</a>           |  Configure the cluster and get it ready           | Mon Aug 10 12:11:15 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246949">246949</a>           |  Configure the cluster and get it ready           | Mon Aug 10 11:27:38 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246902">246902</a>           |  Configure the cluster and get it ready           | Mon Aug 10 09:59:02 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/246880">246880</a>           |  Configure the cluster and get it ready           | Mon Aug 10 08:40:59 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245457">245457</a>           |  Configure the cluster and get it ready           | Fri Aug  7 15:44:29 UTC 2020  | Pass |
|     <a href="https://gitlab.openebs.ci/openebs/e2e-nativek8s/-/jobs/245352">245352</a>           |  Configure the cluster and get it ready           | Fri Aug  7 13:50:10 UTC 2020  | Pass |

