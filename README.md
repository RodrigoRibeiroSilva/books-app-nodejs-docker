﻿# Books App

<p>Segue a lista com os principais comandos docker/docker-compose:</p>

<ul><li>Comandos relacionados à informações<ul><li><code>docker version</code>  <strong>-</strong> exibe a versão do docker que está instalada.</li><li><code>docker inspect ID_CONTAINER</code> <strong>-</strong> retorna diversas informações sobre o container.</li><li><code>docker ps</code>  <strong>-</strong> exibe todos os containers em execução no momento.</li><li><code>docker ps -a</code>  <strong>-</strong> exibe todos os containers, independente de estarem em execução ou não.</li></ul>
</li></ul>
<ul><li>Comandos relacionados à execução<ul><li><code>docker run NOME_DA_IMAGEM</code>  <strong>-</strong> cria um container com a respectiva imagem passada como parâmetro.</li><li><code>docker run -it NOME_DA_IMAGEM</code>  <strong>-</strong> conecta o terminal que estamos utilizando com o do container.</li><li><code>docker run -d -P --name NOME dockersamples/static-site</code>  <strong>-</strong> ao executar, dá um nome ao container.</li><li><code>docker run -d -p 12345:80 dockersamples/static-site</code>  <strong>-</strong> define uma porta específica para ser atribuída à porta 80 do container, neste caso 12345.</li><li><code>docker run -v &#34;CAMINHO_VOLUME&#34; NOME_DA_IMAGEM</code>  <strong>-</strong> cria um volume no respectivo caminho do container.</li><li><code>docker run -it --name NOME_CONTAINER --network NOME_DA_REDE NOME_IMAGEM</code>  <strong>-</strong> cria um container especificando seu nome e qual rede deverá ser usada.</li></ul>
</li></ul>
<ul><li>Comandos relacionados à inicialização/interrupção<ul><li><code>docker start ID_CONTAINER</code>  <strong>-</strong> inicia o container com id em questão.</li><li><code>docker start -a -i ID_CONTAINER</code>  <strong>-</strong> inicia o container com id em questão e integra os terminais, além de permitir interação entre ambos.</li><li><code>docker stop ID_CONTAINER</code>  <strong>-</strong> interrompe o container com id em questão.</li></ul>
</li></ul>
<ul><li>Comandos relacionados à remoção<ul><li><code>docker rm ID_CONTAINER</code>  <strong>-</strong> remove o container com id em questão.</li><li><code>docker container prune</code>  <strong>-</strong> remove todos os containers que estão parados.</li><li><code>docker rmi NOME_DA_IMAGEM</code>  <strong>-</strong> remove a imagem passada como parâmetro.</li></ul>
</li></ul>
<ul><li>Comandos relacionados à construção de Dockerfile<ul><li><code>docker build -f Dockerfile</code>  <strong>-</strong> cria uma imagem a partir de um Dockerfile.</li><li><code>docker build -f Dockerfile -t NOME_USUARIO/NOME_IMAGEM</code>  <strong>-</strong> constrói e nomeia uma imagem não-oficial.</li><li><code>docker build -f Dockerfile -t NOME_USUARIO/NOME_IMAGEM CAMINHO_DOCKERFILE</code>  <strong>-</strong> constrói e nomeia uma imagem não-oficial informando o caminho para o Dockerfile.</li></ul>
</li></ul>
<ul><li>Comandos relacionados ao Docker Hub<ul><li><code>docker login</code>  <strong>-</strong> inicia o processo de login no Docker Hub. </li><li><code>docker push NOME_USUARIO/NOME_IMAGEM</code>  <strong>-</strong> envia a imagem criada para o Docker Hub.</li><li><code>docker pull NOME_USUARIO/NOME_IMAGEM</code>  <strong>-</strong> baixa a imagem desejada do Docker Hub.</li></ul>
</li></ul>
<ul><li>Comandos relacionados à rede<ul><li><code>hostname -i</code>  <strong>-</strong> mostra o ip atribuído ao container pelo docker (funciona apenas dentro do container).</li><li><code>docker network create --driver bridge NOME_DA_REDE</code>  <strong>-</strong> cria uma rede especificando o driver desejado.</li></ul>
</li></ul>
<ul><li>Comandos relacionados ao docker-compose<ul><li><code>docker-compose up</code>  <strong>-</strong> sobe o arquivo compose.yml</li><li><code>docker-compose down</code>  <strong>-</strong> remove os containers do docker-compose</li><li><code>docker-compose restart</code>  <strong>-</strong> restarta os containers do docker-compose</li></ul>
</li></ul>
