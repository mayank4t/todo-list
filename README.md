****#Simple todolist kubernetes deployment ****

This is a todolist application deployed in the K8.

Pipeline steps:- Git Clone, build Docker image, Push docker image to Hub, and Deploy to Kubernetes using hub image.

Docker File:-  nginx base image

Prerequisite:-

Update deployment.yaml for external Ip for loadbalancer,

Jenkins file:- credential required for git, Docker, and Kubernetes

Install Plugin for Jenkins:- Kubernetes

download admin.conf from master using below command, to cloudshell for the Jenkins connection with the K8 :- gcloud compute ssh --zone "asia-south2-a" "master" --project "kubernetestestmayank" --command "sudo cat /etc/kubernetes/admin.conf" > admin.conf
