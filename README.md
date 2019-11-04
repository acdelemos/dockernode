criar pasta do projeto
criar arquivo package.json com o comando:
npm init -y

criar arquivo index.js
criar o arquivo dockerfile

instalar o express com o comando:
npm install express

editar o arquivo index.js com os requires e rota
editar o arquivo dokerfile
criar o arquivo .dockerignore
editar o package.json incluindo a chave start com o comando node index.js
criar a image docker com o comando:
docker build -t acdelemos/dockernode .
rodar a imagem docker com o comando:
docker run -p 3000:3000 -d acdelemos/dockernode
verificar se o docker está rodando a imagem com o comando:
docker ps

criar arquvo docker-compose.yml
editar o arquivo docker-compose.yml

instalar o nodemon com o comando:
npm install --save-dev nodemon
alterar no package.json a chave start para o comando nodemon index.js
obs.: no meu caso só atualiza com o comando:
nodemon --legacy-watch index.js

pegar o container id da imagem com o comando:
docker ps
pode se utilizar o nome da imagem ou o container id para parar/remover
parar a imagem dockernode com o comando:
docker stop dockernode
remover a imagem dockernode com o comando:
docker rm dockernode

startar uma nova imagem com o comando:
docker-compose up --build

a partir da segunda vez que for executar o comando docker-compose up
não será mais necessário do --build

caso queira utilizar o docker em modo detach utilize o -d junto com o comando

deste ponto em diante as alterações no código serão refletidas no server.
