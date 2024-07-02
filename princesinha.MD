Cluster é o agrupamento de todos os Nodes

Node é o computador físico ou virtual onde são criados os pods

Pod é onde são criados os containers, podendo ser um ou mais.

Container é onde fica a aplicação e os arquivos necessários

Deployment é um gerenciador de pods, com ele que criamos os pods e o numero de replicas, assim como o template do container

Replicas é o numero de pod, podendo ser um ou mais

Template são as informações referente a criação dos containers

kubectl run nomedopod (argumento) --image=nomedaimagem
    ele cria um pod com o nome que vc passou no argumento --image você a imagem que vai usada

kubectl get pods 
    ele lista os pods

kubectl apply --filename "-f" nomedoarquivo.yaml
    ele aplica o arquivo, o arquivo pode conter as informações para a criação de "pod" ou um "deployment" 

kubectl get nodes
    ele lista todos os nodes

kubectl delete pod (ou o nome do recurso que eu quero) nomedorecurso
    ele vai deletar o pod que você quer ou outro recurso

kubectl delete pods --all
    delete todos pods

kubectl delete -f nomedoarquivo.yaml
    exclui todos os recursos dentro do arquivo




