### 1S01-cluster-setup

#### Description
 
This test checks the health of the cluster, status of nodes and clones the required github repositories for performing zfs-localpv related functional and chaos (and infra-chaos) testing.

#### Prerequisites

- The host machines should be created and have the dependent packages installed in all the machines.
- All kubernetes nodes should be in ready state which will be verified by `kubectl get nodes` command to get their status.

#### Test Results

| Job ID  |      Test Description         | Execution Time |   Test Result   |
|---------|-------------------------------|----------------|-----------------|
