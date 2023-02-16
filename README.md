# kubernets-dockerimage use the existing docker image
# How to create docker images: <a href="https://github.com/narayanab16/sampledocker" target="_blank">sampledocker</a>
    

    # Installed Softwares
    ---------------------
    minikube or k8s(kubernetes)
    docker community edition
    Git
    
    # Check out 
    git clone https://github.com/narayanab16/kubernets-dockerimage.git
    # change directory
    cd kubernets-dockerimage
    # Up and Running a kubernets engine
    kubectl apply -f javaweb.yml
    # get the pod status
    kubectl get pods
    # get the pod ip
    POD_IP=$(kubectl get pod javaweb -o yaml | grep podIP | awk '{print $2}'); echo $POD_IP
    # test url cURL
    curl $POD_IP:8080
    o/p: This is home page
    
    
    
    
    

