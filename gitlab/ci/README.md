# install gitlab runners
## https://docs.gitlab.com/runner/install/linux-manually.html

## Linux x86-64
    sudo wget -O /usr/local/bin/gitlab-runner https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-amd64

## or Linux x86
    sudo wget -O /usr/local/bin/gitlab-runner https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-386

## or Linux arm
    sudo wget -O /usr/local/bin/gitlab-runner https://gitlab-runner-downloads.s3.amazonaws.com/latest/binaries/gitlab-runner-linux-arm

    sudo chmod +x /usr/local/bin/gitlab-runner

    curl -sSL https://get.docker.com/ | sh

    sudo useradd --comment 'GitLab Runner' --create-home gitlab-runner --shell /bin/bash

    sudo gitlab-runner install --user=gitlab-runner --working-directory=/home/gitlab-runner
    sudo gitlab-runner start






# Registering Runners

    sudo gitlab-runner register

# gitlab-ci coordinator URL
   Setting > CI/CD > Set up a specific Runner manually
# gitlab-ci token
   Setting > CI/CD > Set up a specific Runner manually


# debug runner
    gitlab-runner — debug run
or
    gitlab-ci-multi-runner –debug run
