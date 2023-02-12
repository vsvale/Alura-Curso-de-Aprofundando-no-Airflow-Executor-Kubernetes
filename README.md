# [Alura Curso de Aprofundando no Airflow Executor Kubernetes](https://cursos.alura.com.br/course/aprofundando-airflow-executor-kubernetes)

## Description
    Aprenda a configurar um cluster Kubernetes utilizando o minikube
    Saiba como criar volumes persistentes
    Entenda o funcionamento do executor Kubernetes do Airflow
    Conheça as principais vantagens do executor Kubernetes
    Crie uma imagem customizada para o Airflow
    Saiba como configurar o Airflow no Kubernetes
    Desenvolva e execute um DAG no Airflow

## What I have done
### Update system
    - `sudo -- sh -c 'apt-get update; apt-get upgrade -y; apt-get dist-upgrade -y; apt-get autoremove -y; apt-get autoclean -y'`
### Install git
    - sudo apt install git

### Install Docker:
    - `sudo apt update`
    - `sudo apt install -y ca-certificates curl gnupg lsb-release apt-transport-https software-properties-common`
    - `curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg`
    - `echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null`
    - `sudo apt-get update`
    - `sudo apt install docker-ce docker-ce-cli containerd.io -y`
    - `sudo chmod 666 /var/run/docker.sock`
    - `sudo usermod -aG docker $USER && newgrp docker`
### Install Helm:
    - `curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null`
    - `sudo apt-get install apt-transport-https --yes`
    - `echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list`
    - `sudo apt-get update`
    - `sudo apt-get install helm`
    - `helm repo add argo https://argoproj.github.io/argo-helm && helm repo add kubecost https://kubecost.github.io/cost-analyzer/ && helm repo add stable https://charts.helm.sh/stable && helm repo add bitnami https://charts.bitnami.com/bitnami && helm repo add yugabytedb https://charts.yugabyte.com && helm repo add lensesio https://helm.repo.lenses.io/ && helm repo add pinot https://raw.githubusercontent.com/apache/pinot/master/kubernetes/helm && helm repo add minio https://operator.min.io/ && helm repo add strimzi https://strimzi.io/charts/ && helm repo add elastic https://helm.elastic.co && helm repo add prometheus-community https://prometheus-community.github.io/helm-charts && helm repo add apache-airflow https://airflow.apache.org/ && helm repo add spark-operator https://googlecloudplatform.github.io/spark-on-k8s-operator && helm repo add valeriano-manassero https://valeriano-manassero.github.io/helm-charts && helm repo add jetstack https://charts.jetstack.io && helm repo add kong https://charts.konghq.com
    - `helm repo update`
### 
