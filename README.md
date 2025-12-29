# kubernetes-cluster-connection-with-azdevops
Creating a service connection through service account for kubernetes cluster connection to Azure DevOps



Create a service account on kubernetes

    kubectl create sa sa-azure-devops

Create a ClusterRole and ClusterRoleBinding ( Yaml file)

     vi yam-file-name

Create a secret (Yaml file )

    vi yaml-file-name

Apply all the yaml files.

      kubectl apply -f yaml-file-name

See the kube config file to have the server URL.

      kubectl config view --minify -o json

Get the secret as well.

     kubectl get secret sa-azure-devops-secret  -o json

On Azure DevOps, create a kubernetes service connection using the service account.

<img width="557" height="793" alt="image" src="https://github.com/user-attachments/assets/9568719f-7d7b-4cc3-8adf-a391a2607e8b" />
      


