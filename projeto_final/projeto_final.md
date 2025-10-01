---
layout: default
title: Projeto Final
has_children: true
has_toc: true
prazo_proposta: 15/10/2025
prazo_telas: A definir
prazo_front: A definir
prazo_crud: A definir
prazo_jwt: A definir
prazo_final: A definir
nav_order: 15
---

# Projeto Final

- [📝 Descrição](#descricão)
- [🎯 Objetivos](#objetivos)
- [📑 Requisitos mínimos](#requisitos-mínimos)
- [✅ Critérios de avaliação ](#criterios)
- [💾 Entregas](#entregas)
- [🎤 Apresentação do trabalho ](#apresentação-do-trabalho-)

---

## 📝Descrição

No projeto final, você deverá desenvolver um sistema completo **Fullstack** contendo:

- Um backend desenvolvido utilizando Node.js e Express que fornecer uma API REST
- Um frontend será construído em Vue.js utilizando a Composition API, Vue-Router e Pinia

{:  .new }
A temática do projeto deve possuir viés de extensão. Se você precisa de inspiração confira a página <a href="https://profbruno-ufc-qx.github.io/HubEx/" alt="Site com ideias de projetos relacionados com extensão" target="_blank">HubEx, que contém ideias de projetos de extensão.</a>


## 🎯Objetivos
- Consolidar todo o conteúdo aprendido ao longo da disciplina.
- Exercitar integração entre frontend e backend.
- Trabalhar em um fluxo de desenvolvimento próximo ao mercado.

## 📑Requisitos mínimos

1. **Backend** com Node.js, Express, TypeORM, SQLite e TypeScript.
2. **Frontend** com Vue 3, Composition API, Vue Router, Pinia e TypeScript.
3. **Autenticação JWT** (login, logout, rotas protegidas).
4. Diferentes papéis de usuário (Admin pode gerenciar todos os dados, usuário comum apenas os próprios).
5. Código organizado em **camadas** (services, controllers, routes, stores).

### Frontend

- O **frontend** deve ser uma **SPA – Single Page Application** e sua página principal deve exibida automaticamente ao acessar a raiz da aplicação (**/**).
- O fronted deve ser **modularizar os trechos de HTML usados em várias páginas**. 
    - Exemplo: Deixar cabeçalho e rodapé em arquivos separados e incluí-los nas páginas onde serão necessários.

{:  .warning }
> - Não serão aceitos trabalhos que usam a **Option API**.  Para mais detalhes  <a href="https://medium.com/@victor.souza2210/vue-js-composition-api-vs-options-api-qual-abordagem-escolher-a50a2f2f932b" target="_blank">leia este artigo</a>.
> - O **frontend** deve ser implementado fazendo **OBRIGATORIAMENTE** uso das bibiliotecas **VueRouter** e **Pinia**. 
> - As rotas do frontend **NÃO** podem ser todas públicas.
> - Não serão aceitos trabalhos implementados usando **VUEX**.

### Backend

- O **backend** deverá ter pelos um endpoint com paginação
- O **backend** deverá ter pelos um endpoint com opção de filtragem
- Os dados da aplição devem ser armezandos em um banco de dados **SQLITE**.
 
 
### Conjunto da obra
- A sua aplicação deve possuir pelo menos ***x* entidades (tabelas)**, onde :
<div>
\[x =
  \begin{cases}
    3       & \quad \text{quando o trabalho for individual }\\
   n + 1  & \quad \text{para trabalhos em equipe onde } n \text{ é o tamanho da equipe}
  \end{cases}
\]
</div>

- A aplicação deve implementar os CRUDs de pelo menos **DUAS** dessas tabelas.
  - **Uma das entidades deve ser dependende da outra**, os CRUDs não podem ser totalmente independentes 
  - Para trabalhos em equipe com **mais de dois membros**, as regras de negócio serão avaliada para verificar a elegibilidade do projeto.
- A aplicação deve possuir pelo menos **3 papéis de usuários** de forma que todos os **papéis** possuam permissões diferentes.
- A aplicação deve possuir uma **área pública com páginas/serviços acessíveis a todos; e uma área restrita com páginas/serviços acessíveis somente a usuários autenticados**.
  - A página de login e cadastro de usuários não é considerada uma área pública nessa contexto.


## ✅ Critérios de avaliação <a name="criterios"></a>

- Implementação correta e completa dos requisitos funcionais definidos
- Utlização adequada dos conceitos e tecnologias discutidos ao longo do curso
- Boas práticas de desenvolvimento, incluindo organização do código, padrões de nomenclatura, e legibilidade
- Funcionalidade e desempenho da aplicação
- Qualidade da apresentação do trabalho

{: .warning }
> - O código do projeto que vai ser desenvolvido deve ser hospedado no <a href="http://www.github.com" target="_blank">GitHub</a>.
> - Caso o trabalho seja feito em equipe, cada membro da equipe deve usar seu próprio usuário para escrever código.
> - Não serão aceitos trabalhos implementados em um único commit.
> - TODOS os membros da equipe devem se envolver em atividades de desenvolvido do frontend e do backend.



---

## 💾Entregas

### 🚩 Entrega 0 – Proposta do Projeto

O aluno deverá aceitar o [assingment do GitHub Classroom]() e preencher o README.md do repositório clonado.

Prazo: {{ page.prazo_proposta }}
{: .label .label-red }

### 🎨 Entrega 01 – Primeira versão das telas

- Criar o protótipo funcional das telas no Vue 3 com Vue Rouiter e Pinia.
- Os dados podem ser hardcoded no frontend ou fornecidos por meio de um JSON Server.
- O objetivo é estruturar os componentes, rotas e navegação.

Prazo: {{ page.prazo_telas }}
{: .label .label-red }


### 🖥️ Entrega 02 – Frontend totalmente funcional

- Finalizar o frontend com todos os formulários, validações básicas e rotas prontas.
- O backend pode ser simulado com Strapi ou ferramenta semelhante (MockAPI, JSON Server, etc.).
- Nesta entrega, o aluno deverá demonstrar que o frontend funciona independente da implementação do backend.

Prazo: {{ page.prazo_front }}
{: .label .label-red }


### ⚙️  Entrega 03 – Backend de Usuários

- Criar o backend com Node.js, Express e TypeORM.
- Implementar CRUD de usuários com todas as validações necessárias.
- O banco de dados pode ser SQLite (mais simples para início) ou PostgreSQL.

Prazo: {{ page.prazo_crud }}
{: .label .label-red }


### 🔐 Entrega 04 – Integração com autenticação JWT

- Integrar frontend e backend.
- Implementar login e cadastro de usuários.
- Usar JWT para autenticação e autorização.
- Restringir funcionalidades de acordo com o papel do usuário.

Prazo: {{ page.prazo_jwt }}
{: .label .label-red }


### 🚀 Entrega 05 – Versão final

- Entrega final do sistema, totalmente funcional.
- [Relato de experiência devidamente preenchido](https://forms.gle/Zp6DL3AKid8jtF3y9)

Prazo: {{ page.prazo_final }}
{: .label .label-red }


## 🎤 Apresentação do trabalho <a name="apresentacao"></a>

O trabalho também deverá necessariamente ser apresentado conforme cronograma da disciplina..
