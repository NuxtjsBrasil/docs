---
title: Instalação
description: Começar com o Nuxt.js é realmente muito fácil. Um projeto simples apenas precisa de uma dependência `nuxt`.
---

> Começar com o Nuxt.js é bastante simples. Um projeto simples apenas precisa de uma dependência `nuxt`.

## Utilizando o template inicial do Nuxt.js

Para começar rápido, o time do Nuxt.js criou um [template inicial](https://github.com/nuxt-community/starter-template).

[Baixe o .zip](https://github.com/nuxt-community/starter-template/archive/master.zip) do template inicial ou instale o com o vue-cli:

```bash
$ vue init nuxt-community/starter-template <nome-do-projeto>
```

> Se o [vue-cli](https://github.com/vuejs/vue-cli) não está instalado, por favor instale-o com `npm install -g vue-cli`

logo após instale as dependências:

```bash
$ cd <nome-do-projeto>
$ npm install
```

e inicie o projeto com:

```bash
$ npm run dev
```

A aplicação estará disponível em http://localhost:3000.

<p class="Alert">O Nuxt.js irá ouvir por mudanças nos arquivos dentro do diretório <code>pages</code>, então não há necessidade de reiniciar a aplicação quando adicionado novas páginas.</p>

Para descobrir mais sobre a estrutura do projeto: [Documentação sobre Estrutura de Diretório](/guide/directory-structure).

## Começando do zero

Criar uma aplicação Nuxt.js do zero também é bastante simples, apenas é necessário *1 arquivo e 1 diretório*. Vamos criar um diretório vazio para começar a trabalhar na aplicação:

```bash
$ mkdir <nome-do-projeto>
$ cd <nome-do-projeto>
```

<p class="Alert Alert--nuxt-green"><b>Informações:</b> substítua <code>&lt;nome-do-projeto&gt;</nom-du-projet></code> pelo nome do projeto.</p>

### O package.json

O projeto precisa de um arquivo `package.json` para especificar como iniciar o `nuxt`:

```json
{
  "name": "meu-app",
  "scripts": {
    "dev": "nuxt"
  }
}
```

`scripts` irão iniciar o Nuxt.js através de `npm run dev`.

### Instalando o `nuxt`

Uma vez que o `package.json` foi criado, então adicione o `nuxt` ao projeto através do npm:

```bash
npm install --save nuxt
```

### O diretório `pages`

O Nuxt.js irá transformar cada arquivo `*.vue`  dentro do diretório `pages` como uma rota da sua aplicação.

Crie o diretório `pages`:

```bash
$ mkdir pages
```

logo após crie a primeira página em `pages/index.vue`:

```html
<template>
  <h1>Olá mundo!</h1>
</template>
```

logo após inicie o projeto com:

```bash
$ npm run dev
```

A aplicação estará disponível em http://localhost:3000.

<p class="Alert">O Nuxt.js irá ouvir por mudanças nos arquivos dentro do diretório <code>pages</code>, então não há necessidade de reiniciar a aplicação quando adicionado novas páginas.</p>

Para descobrir mais sobre a estrutura do projeto: [Documentação sobre Estrutura de Diretório](/guide/directory-structure).
