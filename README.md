sudo yum update -y

	curl -O https://s3.us-west-2.amazonaws.com/amazon-eks/1.29.0/2024-01-04/bin/darwin/amd64/kubectl
	
	
	
	sudo curl -o /usr/local/bin/kubectl https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/linux/amd64/kubectl

curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"

sudo chmod +x /usr/local/bin/kubectl

kubectl version --client

					kubectl get all


aws configure

aws eks update-kubeconfig --region ap-south-2 --name eks-cluster-1 

-----------------------------------------------------------------------


aws eks update-kubeconfig --region ap-south-2 --name  eks-B0ezDN1t

kubectl cluster-info

kubectl get nodes


kubectl apply -f jenkins-deployment.yaml

kubectl apply -f jenkins-service.yaml

kubectl get svc jenkins



kubectl apply -f maven-job-config.yaml

kubectl apply -f jenkins-deployment.yaml

kubectl apply -f jenkins-service.yaml

kubectl apply -f jenkins-job.yaml

kubectl get nodes -o wide



kubectl get pods -o wide

sudo find / -name initialAdminPassword





kubectl port-forward svc/jenkins 8080:8080    

kubectl delete pods --all

kubectl delete pods --all -n <namespace>




-----------------------------------------------------------

sudo yum update –y

sudo wget -O /etc/yum.repos.d/jenkins.repo \
    https://pkg.jenkins.io/redhat-stable/jenkins.repo

sudo rpm --import https://pkg.jenkins.io/redhat-stable/jenkins.io-2023.key

 sudo yum upgrade

sudo yum install java-17-amazon-corretto -y

sudo yum install jenkins -y


sudo systemctl enable jenkins

sudo systemctl start jenkins


sudo systemctl status jenkins


----------------------------------------------------------------

aws eks --region ap-south-2 update-kubeconfig --name eks-cluster-1
