minikube start

kubectl apply -f kured-v3.yaml

 // helm install pleaserun kubereboot/kured

kubectl get daemonset
minikube ssh
sudo touch /var/run/reboot-required
exit

add this line somewhere in the kured deployment file - 
            - '--period=1m'

kubectl logs -n default -l app.kubernetes.io/name=kured
