# Mendix_Final
# Please execute command in below order
 - Install helm, Terraform & Gcloud SDK on local env
 - terraform init
 - terraform apply --auto-approve
 
 **Post installation, execute below commands**
 
    **For Linux**
         export KUBECONFIG=kubeconfig-prod
         Execute kubectl cmd to see whether Jenkins Statefulset & Pods are up and running 
         - kubectl get pods
         - kubectl get statefulset
          
        If kubectl command gives unauthorized error then run below commands:
        - gcloud container clusters get-credentials learnk8s-cluster-prod
        - gcloud auth login default
        

    **For Windows**
         set KUBECONFIG=kubeconfig-prod
         Execute kubectl cmd to see whether Jenkins Statefulset & Pods are up and running 
         - kubectl get pods
         - kubectl get statefulset
          
        If kubectl command gives unauthorized error then run below commands:
        - gcloud container clusters get-credentials learnk8s-cluster-prod
        - gcloud auth login default
