# Awesome Persistência de Dados em React Native
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![React Native](https://img.shields.io/badge/React%20Native-blue?logo=react)

> Este repositório reúne conteúdos sobre persistência de dados no React Native.  
> Meu objetivo é que este conteúdo ajude outras pessoas que estão iniciando na área, assim como eu, a encontrar informações ricas e organizadas sobre este tema, que é uma base tão importante para o desenvolvimento.

---

## Índice

- [Conceitos Gerais](#conceitos-gerais)
- [AsyncStorage](#asyncstorage)
- [SQLite](#sqlite)
- [Realm Database](#realm-database)
- [MongoDB e Armazenamento Remoto](#mongodb-e-armazenamento-remoto)
- [Ferramentas e Utilitários](#ferramentas-e-utilitários)
- [Artigos de Comparação](#artigos-de-comparação)
- [Vídeos e Tutoriais em Português](#vídeos-e-tutoriais-em-português)
- [Extras](#extras)
- [Como Contribuir](#como-contribuir)

---

## Conceitos Gerais

Aborda os princípios básicos da persistência de dados, como serialização, diferença entre armazenamento local e remoto, e o padrão "Offline First".

- [Diferença entre armazenamento local e remoto (TechnologyAdvice)](https://technologyadvice.com/blog/information-technology/cloud-storage-vs-local-storage/)
- [O que é Serialização? JSON.stringify() (MDN Docs)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify)
- [Construindo Aplicações Offline-First com React Native (DEV Community)](https://dev.to/zidanegimiga/building-offline-first-applications-with-react-native-3626)
- [Modelo Offline First com React Native (Blog InnovationM)](https://www.innovationm.com/blog/react-native-offline-first-architecture-sqlite-local-database-guide/)

---

## AsyncStorage

Método simples e nativo do React Native para armazenar dados no formato chave-valor. É ideal para configurações, preferências e pequenas quantidades de informação local.

- [Repositório Oficial - @react-native-async-storage/async-storage](https://github.com/react-native-async-storage/async-storage)
- [Guia passo a passo – AsyncStorage com hooks](https://medium.com/@arsdev/persist-data-like-a-pro-in-react-native-67f2bd328a54)
- [Exemplo de CRUD com AsyncStorage](https://gist.github.com/pavlealeksic/3de9c6f3d6148e19b6ddee6b50ed5b94)

---

## SQLite

Banco de dados relacional leve e local, muito usado em aplicativos móveis. Permite criar tabelas, executar consultas SQL e armazenar dados de forma estruturada no dispositivo.
- [**Biblioteca para Expo:** `expo-sqlite` (Documentação Oficial)](https://docs.expo.dev/versions/latest/sdk/sqlite/)
- [**Biblioteca para React Native (Nativo):** `react-native-sqlite-storage` (GitHub)](https://github.com/andpor/react-native-sqlite-storage)
- [Tutorial: CRUD completo com SQLite no React Native](https://medium.com/@shivam.soni.webdev/how-to-implement-crud-in-react-native-with-sqlite-step-by-step-guide-843a8e1d7777)

---

## Realm Database

Banco de dados orientado a objetos que substitui o SQLite em muitos projetos. Tem boa performance, suporte a tipos complexos e integração direta com o React Native.

- [Documentação oficial do Realm React Native](https://www.mongodb.com/docs/atlas/device-sdks/sdk/react-native/)
- [Introdução ao Realm em React Native (DEV Community)](https://dev.to/ajmal_hasan/building-a-react-native-app-with-realm-database-4ab4)
- [Exemplo de CRUD com Realm](https://www.scaler.com/topics/realm-react-native/)

---

## MongoDB e Armazenamento Remoto

Focado em armazenamento remoto e integração com APIs. Mostra como usar o MongoDB e o Express para criar soluções que sincronizam dados entre o app e o servidor.

- [MongoDB Atlas (criar cluster gratuito)](https://www.mongodb.com/atlas/database)
- [Biblioteca Axios para conexão com APIs REST](https://github.com/axios/axios)
- [Tutorial: Conectando React Native ao MongoDB via Express API](https://medium.com/@ahsanshahzad16asb/building-a-full-stack-notes-app-with-react-native-mongodb-express-and-node-js-7a9218a9d874)

---

## Ferramentas e Utilitários

Bibliotecas que complementam as opções de armazenamento, adicionando recursos de segurança, cache e melhor desempenho.  
Essas ferramentas não aparecem no material didático original, mas são amplamente usadas em projetos modernos.

- [**`WatermelonDB`:** Banco de dados reativo de alta performance focado em "Offline-First". Construído sobre o SQLite. (GitHub)](https://github.com/Nozbe/WatermelonDB)
- [**`react-native-mmkv`:** Alternativa de alto desempenho (key-value) ao AsyncStorage.](https://github.com/mrousavy/react-native-mmkv)
- [**Expo SecureStore:** Armazenamento seguro de valores criptografados no dispositivo (ideal para tokens de autenticação).](https://docs.expo.dev/versions/latest/sdk/securestore/)
---

## Artigos de Comparação

- [Comparação: AsyncStorage vs SQLite vs MMKV](https://dev.to/cathylai/choosing-the-right-storage-solution-3log)
- [Realm vs SQLite: qual escolher?](https://www.cleveroad.com/blog/realm-vs-sqlite-what-is-the-best-database-for-android-app-development/)

---

## Vídeos e Tutoriais em Português

Conteúdos em vídeo que explicam de forma direta e acessível como aplicar os principais conceitos de persistência de dados no React Native.

- [SQLite (O Banco de Dados de Bolso) — Código Fonte TV](https://www.youtube.com/watch?v=xOODmm-NdUc)  
  Explica de maneira simples e descontraída o que é o SQLite e por que ele é tão usado em dispositivos móveis.

- [Como utilizar o SQLite no React Native com Expo — Rodrigo Gonçalves](https://www.youtube.com/watch?v=BJEACwKXWf8&t=446s)  
  Mostra na prática como configurar e usar o SQLite em um aplicativo criado com Expo.

- [React Native + Realm — Quebrando Paradigmas](https://youtube.com/playlist?list=PLT2gdUfk6jQTUAiwXTWai4rDo7pW_X7by&si=Hf0jQ4k4eOfrRgZu)  
  Playlist com vários vídeos sobre o uso do Realm no React Native. O conteúdo é bem estruturado e aborda conceitos aplicados a um projeto real.

- [Utilizando Async Storage no React Native — Gabriel Mello](https://www.youtube.com/watch?v=u4-GwottHfc)  
  Um passo a passo simples que ensina a salvar e recuperar dados com AsyncStorage.

---

## Extras

Links complementares para aprofundar o conhecimento sobre arquitetura, padrões de projeto e referências gerais do ecossistema React Native.

- [Lista oficial Awesome React Native](https://github.com/jondot/awesome-react-native)
- [React Native Architecture – padrões de projeto](https://reactnative.dev/docs/architecture-overview)

---

## Como Contribuir

Se você conhece algum artigo, vídeo ou ferramenta interessante sobre persistência de dados no React Native, pode sugerir abrindo uma **Issue** ou enviando um **Pull Request**.  
Toda contribuição é bem-vinda para tornar esta lista cada vez mais completa.





