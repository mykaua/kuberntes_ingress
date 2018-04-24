# Install and configre kubernetes

1) https://kubernetes.io/docs/setup/independent/install-kubeadm/
2) SWAP should be disabled.
3) get token for joining:
	 kubeadm init --apiserver-advertise-address=EXTERNAL_IP_SERVER --pod-network-cidr=10.244.0.0/16 
4) create deployments adn services, check files
5) Install and configure Nginx ingress:
	https://koudingspawn.de/install-kubernetes-ingress/
	https://github.com/kubernetes/ingress-nginx/tree/master/deploy#mandatory-commands
	https://medium.com/southbridge/configure-ingress-on-kubernetes-using-azure-container-service-f72b5cee41f3
	https://hackernoon.com/setting-up-nginx-ingress-on-kubernetes-2b733d8d2f45

6) check ingress:
	curl http://EXTERNAL_IP_Server:30080/pai/ -H "Host: domain_in_ingress.com"
