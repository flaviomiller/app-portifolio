
# Aplicativo para apresentar portifólio, do Último Desafio proposto pelo Santander Bootcamp em parceria com a Dio <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/b8/Banco_Santander_Logotipo.svg/1280px-Banco_Santander_Logotipo.svg.png" width="100" height="30"> <img src="https://static.wixstatic.com/media/7a378f_5140deabd7d040378d740069cb692b87~mv2.png/v1/crop/x_0,y_10,w_1334,h_493/fill/w_568,h_208,al_c,q_85,usm_0.66_1.00_0.01,enc_auto/logo%20DIO.png" height="25px" width="60px"> 

## Navegue aqui :3

* [To do](#to-do)
* [Informações gerais](#informações-gerais)
* [Capturas de tela](#screenshots)
* [Tecnologias](#tecnologia)
* [Setup](#setup)
* [License](#license)

## Informações gerais

Projeto foi feito em kotlin, e tem objetivo central, criar um aplicativo nativo para visualização de projetos,
tal como dos seus criadores, sendo assim, uma espécie de portifólio. 

Antes de tudo, peço desculpas pela forma arquitetada de meu projeto,
 por estudar mais sobre requisições puras (isto é,
 sem o uso de bibliotecas de terceiros como Retrofit) acabei por não seguir exatamente a ordem e reconhecimento do padrão até então utilizado MVVM, por esse motivo,
 e ainda mantendo a melhor organização possivel, decidi ficar algo próximo do MVC.

De forma principal, ele consome duas API, a do [Github](https://docs.github.com/pt/rest/guides/getting-started-with-the-rest-api) para listagem dos perfis,
 para busca de melhores perfis, e para busca de projetos pelo nome, e também a API do [UI Avatars](https://ui-avatars.com/), que gerá imagens aleatórias porém customizada,
 mediante ao parámetro utilizado, no meu caso, o nome dos projetos.

Como decidi deixar nesse projeto o legado que eu mais aprendi durente esses ultimos meses e utilizar um pouco de tudo visto até aqui, então, fiz algumas várias mudanças na criação do aplicativo básico proposto.
 Desde a concepção inicial do aplicativo, que retêm na tela inicial um estudo na área de Ciência de Dados,
 pelos repositórios com mais seguidores do github, além de uma pesquisa por nome de qualquer pessoa ou usuário do github, até a listagem dinâmica e completa dos projetos e perfis detalhados.

## To do

- [ ] Splash Screen
- [x] Tela Inicial (Search) ✔
- [x] Tela do Perfil com os projeots ✔
- [x] Consumir API do github (perfil, projetos), requisição pura no kotlin ✔
- [x] Consumir API de pesquisa, requisição pura ✔
- [x] Consumir [API de imagens](https://ui-avatars.com/) randômicas. ✔
- [x] Adição de banco de dados, SQlite para guardar os perfis favoritos ✔
- [x] Adição de webview com JS para visualização da bio ✔
- [ ] Adição de tema escuro
- [ ] Substituição, Picasso por Coin para requisições svg na tela de repositório
- [ ] Remoção de bugs (deletar do banco e network connection)

## Screenshots
 <img src="images/gif.gif" width="200" />
<p float="left">
  <img src="images/home.jpeg" width="200" /> 
  <img src="images/search.jpeg" width="200" />
  <img src="images/bio.jpeg" width="200" />
  <img src="images/repo.jpeg" width="200" />
  <img src="images/save.jpeg" width="200" />
  <img src="images/remove.jpeg" width="200" />
</p>

## Tecnologia

#### Linguagens:

- Kotlin 
- Xml

#### Arquitetura usada:
- MVC

#### Libraries:

- Picasso(https://github.com/square/picasso)
- Room(https://developer.android.com/jetpack/androidx/releases/room)

## Setup

Para rodar esse projeto, instale-o baixando ou clonando o repositório.

#### Requisitos do sistema 

- Ter um computador
- Android Studio Chipmunk | 2021.2.1
- Minimum sdk v21
- Compile sdk v32

## Licença

```html
MIT Licence 

Copyright (c) 2022 Wanderley Filho

Permission is hereby granted, free of charge, to any person obtaining a copy of this software
and associated documentation files (the "Software"), to deal in the Software without restriction,
including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, 
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial 
portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE
AND NONINFRINGEMENT.IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE
OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```
