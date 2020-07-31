# e2e-nativek8s

This repository's `master` branch contains README's and the test results for each indivisual test which is meant to run for inducing chaos and testing zfs-localpv components. It includes several stages to perform different scenraios in end to end work-flow. To see the plateform execution scripts for the tests switch to the `release-branch` of this repository.

To see the CI/E2E summary of the gitlab pipelines for e2e-nativek8s project visit `openebs.ci` and switch to `k8s` tab under `stable releases` category.

## Pipeline stages for running against release-branch

1. cluster-setup
2. provisioner
3. functional
4. chaos
5. infra-chaos
6. cleanup

## Upgrade-testing

The other branch of this repository `zfslocalpv-upgrade` consists the code for testing the upgrade of zfs-localpv components from any previous version to the any latest version. Work-flow for this branch is as following:
 - First    configure the cluster to make it ready to run pipeline
 - Second   Provision the zfs-localpv components for any previous versoin
 - Third    Deploy multiple application and dump some data for to perform functional test after upgrade
 - Fourth   Upgrade the zfs-localpv components to the newer version and verify the successful upgrade
 - Fifth    Perform functional test on the volume to verify that it is intact in process of upgrade
 - Sixth    Clean-up the resources and revert the cluster back to its initial state
