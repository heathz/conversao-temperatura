# Conversao de Temperatura
Repositório criado para o Desafio Docker da Formação Kubedev - Kubedev.io

A aplicação roda em cima do NodeJS e faz a conversão de temperatura entre graus Célsius e Fahrenheit.
Para o desafio, foi criado o arquivo Dockerfile para o build da imagem que está disponível no Docker Hub em

    https://hub.docker.com/repository/docker/timeuz/conversao-temperatura/

No Dockerfile pode ser observado que a imagem utiliza a versão 14.17.5 da imagem do node presente do Docker Hub.

O diretório de instalação da aplicação está setado para /usr/share/temperatura

Inicialmente os arquivos package.json e package-lock.json são copiados para pasta raiz da aplicação e em seguida é feito o npm install para a instalação das dependências do projeto. Despois da instalação os demais arquivos são copiados para a pasta da aplicação.

Em seguida a porta 8080 é exposta e o comando node server.js é executado para inicialização da aplicação.

Para utilização da imagem:

    docker run -d timeuz/conversao-temperatura

Em seguida acessar no navegador:

    http://localhost:8080
    
