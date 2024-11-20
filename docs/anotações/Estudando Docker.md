# Estudando Docker

Docker é uma plataforma de virtualização que facilita o desenvolvimento e o deploy de aplicações. Ele utiliza **containers** para empacotar aplicações junto com suas dependências e configurações, permitindo padronização e portabilidade.

---

## Docker Image vs Docker Container

### Docker Image: O Molde do Bolo
- É como uma receita ou modelo.
- Contém instruções e dependências para criar uma aplicação.
- Exemplo: Pode incluir o sistema operacional (ex.: Ubuntu), bibliotecas, dependências e código-fonte.

### Docker Container: O Bolo Assado
- É uma instância funcional criada a partir de uma imagem.
- Um container é "vivo", podendo ser executado e manipulado.
- Vários containers podem ser criados a partir da mesma imagem.

---

## Docker Hub
- O **Docker Hub** é um repositório público com diversas imagens prontas para uso.
- Algumas imagens são mantidas por especialistas do Docker, que colaboram com os desenvolvedores das ferramentas.

### Comandos úteis:
- `docker images`: Lista imagens armazenadas localmente.
- `docker ps`: Lista containers em execução.

### Exemplo de uso:
1. **Baixar uma imagem específica:**
   ```bash
   docker pull {nome}:{tag}
   # Exemplo:
   docker run nginx:1.26
   ```
Nota: Caso a imagem não exista localmente, o Docker irá baixá-la do Docker Hub antes de rodar.

## Modificadores no Comando docker run
### Rodar em modo "detached" (-d ou --detach)
Para evitar que o terminal fique bloqueado:
   ```bash
   docker run -d {nome}:{tag}
   # Exemplo:
   docker run -d nginx:1.26
   ```
### Expondo portas (Port Binding)
Por padrão, os containers são isolados em uma rede interna. Para acessá-los:

```bash
docker run -d -p {portaEscolha}:{portaContainer} {nome}:{tag}
# Exemplo:
docker run -d -p 9000:80 nginx:1.26
```
Agora, o container estará disponível em: http://localhost:9000

### Nomeando containers
Para evitar nomes aleatórios:

```bash
docker run --name {nomeContainer} -d -p {portaEscolha}:{portaContainer} {nome}:{tag}
# Exemplo:
docker run --name web-app -d -p 80:80 nginx:1.26
```
## Gerenciamento de Containers
Ver containers ativos:

```bash
docker ps
```

Ver todos os containers (ativos e parados):

```bash
docker ps -a
```
Iniciar um container parado:
```bash
docker start {nome ou id}
```
Parar um container ativo:

```bash
docker stop {nome ou id}
```
Parar múltiplos containers:

```bash
docker stop {nome1} {nome2}
```

## Registries Docker Privados
### Docker Hub e Registries Públicos
* Docker Hub é o registro público padrão.
* Ideal para projetos abertos ou comunitários.
### Registries Privados
* Empresas usam registros privados para proteger imagens internas e proprietárias.
### Analogia com GitHub:
* GitHub => Docker Registry
* Repositórios => Docker Repository
* Commits => Imagens e suas versões (tags).

## Dockerfile: Criando Imagens Personalizadas
Um Dockerfile define como construir uma imagem para a aplicação.

### Exemplo: Dockerização de uma aplicação Node.js
1. Definir a base da imagem:

```bash
FROM node:19-alpine
```
2. Copiar arquivos da aplicação:

```bash
COPY package.json /app/
COPY src /app/src
```
3. Definir o diretório de trabalho:

```bash
WORKDIR /app
```
4. Instalar dependências:

```bash
RUN npm install
```
5. Definir o comando para iniciar a aplicação:

```bash
CMD ["node", "server.js"]
```
### Construindo a Imagem
```bash
docker build -t node-app:1.0 .
```
* -t node-app:1.0: Nome e tag da imagem.
* (ponto) . : Diretório onde está o Dockerfile.

Para listar as imagens:

```bash
docker images
```
Executando o Container:
```bash
docker run -d -p 3000:3000 node-app:1.0
```
## Comandos Adicionais
Ver logs de um container:

```bash
docker logs {id}
```
Remover um container:

```bash
docker rm {id}
```
Remover uma imagem:

```bash
docker rmi {id}
```

## Referência

- https://www.youtube.com/watch?v=pg19Z8LL06w
- https://hub.docker.com/_/nginx
- https://hub.docker.com/
- https://gitlab.com/nanuchi/docker-in-1-hour