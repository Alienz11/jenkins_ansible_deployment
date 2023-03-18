# Microservices Deployment

This deployment uses Ansible to manage the configuration of a Kubernetes cluster on AWS. The application is deployed using Kubernetes manifests and consists of a web application with an Nginx frontend and a MongoDB backend. Monitoring is set up using Prometheus and logging is collected using Fluentd.

## Deployment Steps

1. Provision the AWS infrastructure using the `aws_ec2` module in Ansible.
2. Install Kubernetes using the `kubeadm` tool.
3. Deploy the web application and database using Kubernetes manifests.
4. Set up monitoring using Prometheus and Grafana.
5. Collect logs using Fluentd and store them in Elasticsearch.

## Deploy Pipeline

The deployment is automated using a Jenkins pipeline. The pipeline checks out the code from the repository, builds the Docker images, deploys the application to the Kubernetes cluster, and runs integration tests using Cypress.

## Security

The deployment is secured using Let's Encrypt certificates and network perimeter security access rules. Sensitive information is encrypted using Ansible Vault.
