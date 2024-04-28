# LAWFLOW - Docker-compose


Para fins de facilidade na criação dos containers, criei este arquivo que deverá ficar em uma pasta própria em seu computador onde os repositórios [**LawFlow---Frontend-Sprint-2**](https://github.com/HugoLeoNunes/LawFlow---Frontend-Sprint-2) e [**LawFlow---Backend-Sprint-2**](https://github.com/HugoLeoNunes/LawFlow---Backend-Sprint-2), deverão ser clonados.

Desta forma, na pasta criada ficará apenas o arquivo docker-compose.yml e as pastas LawFlow---Backend-Sprint-2 e LawFlow---Frontend-Sprint-2.

*Explicação do Docker Compose*

O arquivo docker-compose.yml é usado pelo Docker Compose para definir e gerenciar múltiplos containers Docker como um único serviço. Aqui está o que cada parte do seu arquivo faz:

version: '3': Esta linha especifica a versão da sintaxe do Docker Compose que está sendo usada. A versão '3' é a mais recente e suporta todos os recursos do Docker Compose.

services:: Esta linha inicia a definição dos serviços que compõem a sua aplicação. Cada serviço corresponde a um container Docker.

backend: e frontend:: Estas linhas definem dois serviços, backend e frontend. Cada serviço terá seu próprio container Docker.

build: ./LFBackAvancado e build: ./LFFrontBasico: Estas linhas especificam o caminho para o Dockerfile que será usado para construir a imagem Docker para cada serviço. O Docker Compose irá procurar um arquivo chamado Dockerfile nesses diretórios e usá-lo para construir a imagem.

ports:: Esta linha inicia a definição das portas que serão expostas pelo container.

- "5000:5000" e - "80:80": Estas linhas mapeiam as portas do container para as portas do host. O formato é porta_do_host:porta_do_container. Portanto, a aplicação backend estará acessível na porta 5000 do host e a aplicação frontend estará acessível na porta 80 do host.

Em resumo, este arquivo docker-compose.yml define uma aplicação composta por dois serviços, backend e frontend. Cada serviço é construído a partir de seu próprio Dockerfile e expõe uma porta para o host.

[**Dr. Hugo Leonardo Nunes.**](https://www.linkedin.com/in/hugo-leonardo-nunes-474152246/) 
