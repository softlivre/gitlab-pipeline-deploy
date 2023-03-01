This pipeline is used to deploy a GitLab project to a server (CD/ Continuous Deployment).

It depends on variables defined in the GitLab project settings.

$SSH_PRIVATE_KEY : The private key used to connect to the server.

$SERVER_IP : The IP address of the server.

It will install the certificate on the runner, connect to the remote server, and then update the machine repository with the latest code from the GitLab project.

It will be triggered only when there is a merge to the master branch.

![alt text](https://github.com/softlivre/gitlab-pipeline-deploy/blob/main/pipeline.png?raw=true)