# Vue Norte - Site 💻

Site da comunidade Vue Norte desenvolvido com Quasar Framework SSR

## Instalação
Para instalar localmente será necessário você ter o [npx](https://www.npmjs.com/package/npx) instalado globalmente em sua máquina, pois estamos criando com uma versão beta do Quasar Framework.

Após instalar o npx, crie um diretório no seu ambiente, por exemplo **quasar-beta**, acesse o diretório criado e crie um arquivo package.json com o comando:

```sh
npm init 
```
Após criar o arquivo, instale a versão beta do quasar-cli localmente neste diretório:
```sh
npm install --save @quasar/cli
```
Dessa forma evitamos qualquer problema com os projetos antigos construidos com o CLI anterior.

Agora clone esse projeto dentro do mesmo diretório:
```sh
git clone https://github.com/patrickmonteiro/vuenorte
```

Acesse o diretório vuenorte e instale as dependências:
```sh
npm install
```
e execute o seguinte comando para levantar seu ambiente de desenvolvimento com a nova versão do quasar:
```sh
npx quasar dev
```
Observe se no seu console o **pkg quasar** está **v1.0.0-beta.10** e **pkg @quasar/app - v1.0.0-beta-13** 

Pronto, agora você pode modificar e fazer seu pull request com novas ideias para nossa comunidade.