## Projeto Desenvolvendo Microsserviço em Java para Integração com IA Generativa

# DESCRIÇÃO
Esse projeto tem como objetivo desenvolver um microsserviço responsável por receber uma imagem de perfil e enviá-la para uma Inteligência Artificial Generativa (Stable Diffusion), criando assim variações criativas da imagem. O microsserviço será desenvolvido em Java, utilizando o framework Quarkus e tecnologias avançadas como Hibernate, MariaDB, JAX-RS, Reactive Programming, Mutiny, Docker e Testcontainers. Você entenderá na prática desde criação da Estrutura do Projeto e seus Domínios até a conexão com Banco de Dados e o consumo de um serviço de IA via REST Client. Os pré-requisitos para conseguir executar o projeto por completo são: conhecimentos intermediários em Java e Docker, bem como conhecimentos básicos em HTTP, MariaDB e AWS S3.


# avatar

Este projeto usa Quarkus, o Supersonic Subatomic Java Framework.

Se quiser saber mais sobre o Quarkus, visite o site: https://quarkus.io/ .

## Executando o aplicativo no modo dev

Você pode executar seu aplicativo no modo dev que permite a codificação ao vivo usando:
```script shell
./mvnw compila quarkus:dev
```

> **_NOTA:_** O Quarkus agora vem com uma IU Dev, que está disponível apenas no modo dev em http://localhost:8080/q/dev/.

## Empacotando e executando o aplicativo

O aplicativo pode ser empacotado usando:
```script shell
./mvnw pacote
```
Ele produz o arquivo `quarkus-run.jar` no diretório `target/quarkus-app/`.
Esteja ciente de que não é um _über-jar_ pois as dependências são copiadas para o diretório `target/quarkus-app/lib/`.

O aplicativo agora pode ser executado usando `java -jar target/quarkus-app/quarkus-run.jar`.

Se você deseja construir um _über-jar_, execute o seguinte comando:
```script shell
./mvnw pacote -Dquarkus.package.type=uber-jar
```

O aplicativo, empacotado como um _über-jar_, agora pode ser executado usando `java -jar target/*-runner.jar`.

## Criando um executável nativo

Você pode criar um executável nativo usando:
```script shell
./mvnw pacote -Pnative
```

Ou, se você não tiver o GraalVM instalado, pode executar o build executável nativo em um contêiner usando:
```script shell
./mvnw pacote -Pnative -Dquarkus.native.container-build=true
```

Você pode então executar seu executável nativo com: `./target/avatar-1.0.0-SNAPSHOT-runner`

Se você quiser saber mais sobre a criação de executáveis nativos, consulte https://quarkus.io/guides/maven-tooling.

## Roberto Trugilho Moreira<br> Em desenvolvimento...