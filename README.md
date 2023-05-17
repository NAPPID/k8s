# k8s
Ansible playbooks for k8s cluster configuration with KUBEADM.

Have a seperate host file in a folder and update host pattrens along with host IP/hostnames.

Also have config file, update the config data. 


Some useful commands: 

kubectl get pods
kubectl get pods --all
kubectl get pods --show-labels
kubectl get deploy deploy-obj
kubectl describe deploy deploy-obj
kubectl delete --all --all
kubectl delete deploy deploy-obj
kubectl set image deploy deploy-obj deploy-cont=nginx:1.18
kubectl edit deploy deploy-obj
kubectl create deploy deploy2 --image=nginx --replicas=2  ### AdHoc command
kubectl scale deploy deploy2 --replicas=3
kubectl label deploy deploy2 role=dev  #### Adding Labels
kubectl label deploy deploy2 role-  ### Removing Labels
 kubectl set image deploy deploy-obj deploy-cont=tomcat
 kubectl rollout history deploy deploy-obj 
 kubectl rollout undo deploy deploy-obj --to-revision=1
 kubectl rollout status deploy deploy-obj
 


