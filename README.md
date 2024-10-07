# Anotações-kubernetes-alura-3
 Neste repositório irei deixar algumas anotações sobre o terceiro curso da alura de Kubernetes


kubectl get cj = Lista todos os Agendamentos 

kubectl api-resources = mostra tudo o que está disponivel no cluster

O nodeport não é recomendado para utilizar no kubernetes, porém pode ser utilizado no minikube 

Nós criamos um persistentVolumeclaim para guardar os arquivos que serao guardados nos volumes 

Node port não é muito recomendado em ambiente com varios pods

O loadBalancer ele usa o balanceador que vai estar sendo disponibilizado pelo seu ambiente, tipo aws, azure



head -c 32 /dev/urandom | base64 = comando para gerar as chaves de criptografia randomicas 


minikube mount ./config:/var/lib/minikube/certs/config = comando para criar a pasta onde estará nosso arquivo de criptografia, crypt.yaml dentro do minikube



minikube start --extra-config=apiserver.encryption-provider-config=/var/lib/minikube/certs/config/crypt.yaml = comando para iniciar o minikube com o arquivo de criptografia


o Cronjob serve para agendar o Backup do banco de dados