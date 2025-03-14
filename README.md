```
    1  docker ps
    2  docker ps -a
    3  [ $(uname -m) = x86_64 ] && curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.27.0/kind-linux-amd64
    4  chmod +x ./kind
    5  sudo mv ./kind /usr/local/bin/kind
    6  kind --version
    7  echo "$(cat kubectl.sha256)  kubectl" | sha256sum --check
    8  sudo install -o root -g root -m 0755 kubectl /usr/local/bin/kubectl
    9  chmod +x kubectl
   10  mkdir -p ~/.local/bin
   11  mv ./kubectl ~/.local/bin/kubectl
   12  kubectl version --client
   13  kubectl get pods
   14  kubectl config current-context
   15  ls
   16  mkdir projects
   17  cd projects/
   18  ls
   19  mkdir kind-cluster
   20  cd kind-cluster/
   21  ls
   22  vim kind-cluster.yml
   23  kind create-cluster --config kind-cluster.yml 
   24  kind create cluster --config kind-cluster.yml 
   25  vim kind-cluster.yml
   26  kind create cluster --config kind-cluster.yml 
   27  kubecctl get pods
   28  kubectl get pods
   29  kubectl get nodes
   30  kubectl config view
   31  kind create cluster --config=kind-cluster.yml 
   32  vim kind-cluster.yml
   33  kind create cluster --config=kind-cluster.yml 
   34  kubectl get nodes
   35  kind create cluster --config=kind-cluster.yml 
   36  kind cluster
   37  kind 
   38  kind delete my-cluster
   39  kind get
   40  kind get cluster
   41  kind get clusters
   42  kind delete my-cluster
   43  kind delete cluster my-cluster
   44  kind delete cluster
   45  kind get clusters
   46  kind delete clusters my-cluster
   47  kind get clusters
   48  kind create cluster --config=kind-cluster.yml 
   49  kind get clusters
   50  kind delete clusters my-cluster
   51  vim kind-cluster.yml
   52  kind create cluster --config=kind-cluster.yml 
   53  kubectl get nodes
   54  kubectl get pods
   55  vim first-app-ns.yml
   56  kubectl apply -f first-app-ns.yml 
   57  kubectl get ns
   58  pwd
   59  ls
   60  sudo apt-get update
   61  sudo apt-get install docker.io
   62  docker ps
   63  sudo moduser -aG docker $USER
   64  sudo usermod -aG docker $USER
   65  newgrp docker
   66  ls
   67  cd projects/
   68  ls
   69  kubectl get nodes
   70  cd kind-cluster/
   71  ls
   72  kubectl get namespace
   73  vim deployment.yml
   74  kubectl apply -f deployment.yml 
   75  kubectl get pods
   76  kubectl describe pod portfolio-deployment-56f855c4b-45kkq
   77  kubectl get pods
   78  vim deployment.yml
   79  kubectl get ns
   80  kubectl apply -f deployment.yml 
   81  vim deployment.yml
   82  kubectl apply -f deployment.yml 
   83  vim deployment.yml
   84  kubectl apply -f deployment.yml 
   85  vim first-app-ns.yml 
   86  kubectl delete -f first-app-ns.yml 
   87  vim first-app-ns.yml 
   88  kubectl apply -f first-app-ns.yml 
   89  kubectl get namespce
   90  kubectl get namespces
   91  kubectl get namespaces
   92  kubectl apply -f deployment.yml 
   93  kubectl get pods
   94  kubectl get all
   95  kubect get deployment --namespace=first-app-ns
   96  kubectl get deployment --namespace=first-app-ns
   97  kubectl get pods --namespace=first-app-ns
   98  kubectl get pods -A
   99  kubectl delete -f deployment.yml 
  100  vim deployment.yml 
  101  kubectl get deployments
  102  kubectl delete portfolio-deployment
  103  kubectl delete deployment portfolio-deployment
  104  kubectl get deployments
  105  kubectl get nodes
  106  kubectl get pods
  107  kubectl get all --ns=first-app-ns
  108  kubectl get all --namespace=first-app-ns
  109  kubectl apply -f deployment.yml 
  110  kubectl get all --namespace=first-app-ns
  111  vim deployment.yml 
  112  cat deployment.yml 
  113  kubectl get all -n first-app-nx
  114  kubectl get all -n first-app-ns
  115  kubectl get all -n first-app-ns -o wide
  116  kubectl scale deployment portfolio-deployment -n first-app-ns --replicas=5
  117  kubectl get all -n first-app-ns -o wide
  118  kubectl scale deployment portfolio-deployment -n first-app-ns --replicas=1
  119  kubectl get all -n first-app-ns -o wide
  120  kubectl apply -f deployment.yml 
  121  kubectl get all -n first-app-ns -o wide
  122  free -m
  123  kubectl delete -f .
  124  kubectl delete -f . -n first-app-ns
  125  ls
  126  cd projects/
  127  ls
  128  cd kind-cluster/
  129  ls
  130  kubectl get pods
  131  kubectl get pods -n first-app-ns
  132  kubectl apply -f first-app-ns.yml 
  133  kubectl get nodes
  134  kubectl apply -f deployment.yml 
  135  kubectl get pods -n first-app-ns
  136  vim deployment.yml 
  137  kubectl get pods -n first-app-ns
  138  kubectl apply -f deployment.yml 
  139  kubectl get pods -n first-app-ns
  140  kubectl get all -n first-app-ns
  141  kubectl delete -f deployment.yml 
  142  vim deployment.yml 
  143  kubectl apply -f deployment.yml 
  144  kubectl get all -n first-app-ns
  145  ls
  146  kubectl get all -n first-app
  147  cd projects/kind-cluster/
  148  ls
  149  kubectl get nodes
  150  kubectl apply -f first-app-ns.yml 
  151  vim deployment.yml 
  152  kubectl apply -f deployment.yml 
  153  kubectl get all -n first-ap-ns
  154  kubectl get all
  155  kubectl get ns
  156  kubectl get pods -n first-app-ns
  157  kubectl get deploy
  158  kubectl get deploy -n first-app-ns
  159  vim service.yml
  160  kubectl apply -f service.yml 
  161  kubectl get svc
  162  kubectl delete svc portfolio-service
  163  vim service.yml 
  164  kubectl apply -f service.yml 
  165  kubectl get svc
  166  kubectl get svc -n first-app-ns
  167  kubectl port-forward service portfolio-service 80:80 --address 0.0.0.0
  168  kubectl port-forward service/portfolio-service 80:80 --address 0.0.0.0
  169  kubectl get all -n first-app-ns
  170  kubectl port-forward service/portfolio-service -n first-app-ns 80:80 --address 0.0.0.0
  171  vim service.yml 
  172  vim deployment.yml 
  173  kubectl delete -f service.yml 
  174  kubectl delete -f deployment.yml 
  175  vim service.yml 
  176  vim deployment.yml 
  177  kubectl apply -f deployment.yml -f service.yml 
  178  kubectl port-forward service/portfolio-service -n first-app-ns 3000:3000 --address 0.0.0.0
  179  vim service.yml 
  180  kubectl apply -f service.yml 
  181  kubectl port-forward service/portfolio-service -n first-app-ns 80wq:80 --address 0.0.0.0
  182  kubectl port-forward service/portfolio-service -n first-app-ns 80:80 --address 0.0.0.0
  183  vim service.yml 
  184  kubectl port-forward service/portfolio-service -n first-app-ns 80:3000 --address 0.0.0.0
  185  kubectl apply -f service.yml 
  186  kubectl port-forward service/portfolio-service -n first-app-ns 80:3000 --address 0.0.0.0
  187  kubectl port-forward service/portfolio-service -n first-app-ns 3000:3000 --address 0.0.0.0
  188  kubectl get all -n first-app-ns
  189  vim service.yml 
  190  kubectl apply service.yml 
  191  kubectl apply -f service.yml
  192  kubectl port-forward service/portfolio-service -n first-app-ns 3001:3001 --address 0.0.0.0
  193  cd projects/kind-cluster/
  194  ls
  195  kubectl get nodes
  196  kubectl get all -n first-app-ns
  197  kubectl port-forward service/portfolio-service -n first-app-ns 5000:3001 --address 0.0.0.0
  198  vim service.yml 
  199  kubectl apply -f service.yml 
  200  kubectl port-forward service/portfolio-service -n first-app-ns 80:3000 --address 0.0.0.0
  201  kubectl port-forward service/portfolio-service -n first-app-ns 5000:3000 --address 0.0.0.0
  202  vim service.yml 
  203  vim deployment.yml 
  204  ls
  205  cd projects/kind-cluster/
  206  ls
  207  cd ..
  208  cd kind-cluster/
  209  cat service.yml 
  210  kubectl apply -f https://kind.sigs.k8s.io/examples/ingress/deploy-ingress-nginx.yaml
  211  kubectl get ns
  212  kubectl get svc -n ingress-nginx
  213  vim ingress.yml
  214  kubectl apply -f ingress.yml 
  215  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-ngix 80:3000 --address=0.0.0.0
  216  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-nginx 80:3000 --address=0.0.0.0
  217  vim service.yml 
  218  vim ingress.yml 
  219  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-nginx 80:80 --address=0.0.0.0
  220  vim ingress.yml 
  221  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-nginx 80:80 --address=0.0.0.0
  222  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-nginx 80:803000 --address=0.0.0.0
  223  sudo -E kubectl port-forward svc/ingress-nginx-controller -n ingress-nginx 80:80 --address=0.0.0.0
  224  vim service.yml 
  225  kubectl delete -f ingress.yml 
  226  cat service.yml 
  227  vim ingress.yml
  228  kubectl apply -f ingress.yml 
  229  kubectl get ing -n first-app-ns
  230  kubectl delete -f ingress.yml 
  231  vim ingress.yml 
  232  kubectl apply -f ingress.yml 
  233  kubectl delete -f ingress.yml 
  234  vim ingress.yml 
  235  kubectl apply -f ingress.yml 
  236  kubectl delete -f ingress.yml 
  237  vim ingress.yml 
  238  kubectl apply -f ingress.yml 
  239  kubectl delete -f ingress.yml 
  240  vim ingress.yml 
  241  kubectl apply -f ingress.yml 
  242  vim deployment-nginx.yml 
  243  kubectl apply -f deployment-nginx.yml 
  244  cat service.yml 
  245  vim service-nginx.yml
  246  kubectl delete -f deployment-nginx.yml 
  247  vim deployment-nginx.yml 
  248  kubectl applty deployment-nginx.yml 
  249  kubectl apply deployment-nginx.yml 
  250  kubectl apply -f deployment-nginx.yml 
  251  kubectl apply -f service-nginx.yml 
  252  vim ingress.yml 
  253  cat service-nginx.yml 
  254  vim service-nginx.yml 
  255  vim ingress.yml 
  256  kubectl apply -f ingress.yml 
  257  kubectl get all -n first-app-ns
  258  ls
  259  vim sql-deployment.yml
  260  kubectl apply -f s
  261  kubectl apply -f sql-deployment.yml 
  262  kubect get pods
  263  kubectl get pods
  264  kubectl describe pod sql-deployment-769fcf8c-fg54j
  265  kubectl logs pod sql-deployment-769fcf8c-fg54j
  266  kubectl logs sql-deployment-769fcf8c-fg54j
  267  vim sql-secret.yml
  268  vim sql-deployment.yml 
  269  cat sql-deployment.yml 
  270  cat sql-secret.yml 
  271  kubectl apply -f sql-secret.yml 
  272  kubectl apply -f sql-deployment.yml 
  273  vim sql-deployment.yml 
  274  vim sql-secret.yml 
  275  kubectl apply -f sql-secret.yml 
  276  kubectl apply -f sql-deployment.yml 
  277  vim sql-secret.yml 
  278  vim sql-deployment.yml 
  279  kubectl apply -f sql-deployment.yml 
  280  kubectl get pods
  281  vim sql-config-map.yml
  282  kubectl apply sql-config-map.yml 
  283  kubectl apply -f sql-config-map.yml 
  284  vim sql-deployment.yml 
  285  kubectl apply -f sql-deployment.yml 
  286  kubectl get pods
  287  kubectl exec -it sql-deployment-5f86bc85d6-555wn -- bash
  288  cat sql-deployment.yml 
  289  ls
  290  mkdir cluster
  291  pwd
  292  mv kind-cluster.yml /home/ubuntu/projects/kind-cluster/kind-cluster.yml
  293  mv kind-cluster.yml /home/ubuntu/projects/kind-cluster/cluster/kind-cluster.yml
  294  ls
  295  kubectl delete -f .
  296  kubectl get pods

kubectl apply -f https://github.com/kubernetes-sigs/metrics-server/releases/latest/download/components.yaml
```
