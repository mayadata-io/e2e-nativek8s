### Goal of this stage

The goal of this gitlab stage is to check the health of the on-premise cluster created on vSphere based virtual machines and to get it ready for carrying out zfs-localpv related functional and chaos (and infra-chaos) testing.

### cluster details

#### k8s version:
               v1.17.2 (1 master + 3 worker_node cluster)

#### zfs version: 
               $ modinfo zfs | grep -iw version
               version: 0.8.1-1ubuntu14.4

#### OS details:
               $ cat /etc/os-release
               NAME="Ubuntu"
               VERSION="18.04.3 LTS (Bionic Beaver)"
               ID=ubuntu
               ID_LIKE=debian
               PRETTY_NAME="Ubuntu 18.04.3 LTS"
               VERSION_ID="18.04"
               HOME_URL="https://www.ubuntu.com/"
               SUPPORT_URL="https://help.ubuntu.com/"
               BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
               PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
               VERSION_CODENAME=bionic
               UBUNTU_CODENAME=bionic


### The test cases in cluster-setup stage

| S.No | TID  | Test case description                  |
| ---- | ---- | ---------------------------------------|
| 1    | 1C01 | Configure the cluster and get it ready |

