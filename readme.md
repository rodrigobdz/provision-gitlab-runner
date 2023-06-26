# Provision GitLab Runner Manager

Automation scripts to provision a GitLab Runner manager on AWS EC2. Based on the [GitLab Runner Autoscale](https://docs.gitlab.com/runner/configuration/autoscale.html) documentation.

Follow the guide [Autoscaling GitLab Runner on AWS EC2](https://docs.gitlab.com/runner/configuration/runner_autoscale_aws/) and use this repo to automate the section [Prepare the runner manager instance](https://docs.gitlab.com/runner/configuration/runner_autoscale_aws/#prepare-the-runner-manager-instance).

A copy of the `/etc/gitlab-runner/config.toml` is in the repo as [config.toml](./etc/gitlab-runner/config.toml) for reference.

## Usage

- Bootstrap the GitLab Runner manager instance

    ```sh
    ./script/bootstrap-ubuntu
    ```

- Register GitLab Runner

    ```sh
    ./script/register-runner
    ```