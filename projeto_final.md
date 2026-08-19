---
layout: default
title: Projeto Final
has_children: true
has_toc: true
prazo_form: Aguardando definição
prazo_proposta: Aguardando definição
prazo_final: Aguardando definição
nav_order: 15
---

# Projeto Final

* [Descrição](#descricão)
* [Objetivos](#objetivos)
- [Requisitos mínimos](#requisitos-mínimos)
* [Como funciona a entrega do projeto final](#fluxo)
  * [Formulário e repositório dai equipe](#formulario) **Prazo: {{ page.prazo_form }}**
  * [Envio da proposta](#envio-proposta) - **Prazo: {{ page.prazo_proposta }}**
  * [Desenvolvimento](#desenvolvimento)
  * [Entrega final](#envio-entrega) - **Prazo: {{ page.prazo_final }}**
* [Apresentação do trabalho ](#apresentação-do-trabalho-)

---

## Descrição

No projeto final, você deverá desenvolver um sistema completo **Fullstack** contendo:

- Um backend desenvolvido utilizando Node.js e Express que fornecer uma API REST
- Um frontend será construído em Vue.js utilizando a Composition API, Vue-Router e Pinia

## Objetivos
- Consolidar todo o conteúdo aprendido ao longo da disciplina.
- Exercitar integração entre frontend e backend.
- Trabalhar em um fluxo de desenvolvimento próximo ao mercado.

## Requisitos mínimos

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


{: .warning }
> - O código do projeto que vai ser desenvolvido deve ser hospedado no <a href="http://www.github.com" target="_blank">GitHub</a>.
> - Caso o trabalho seja feito em equipe, cada membro da equipe deve usar seu próprio usuário para escrever código.
> - Não serão aceitos trabalhos implementados em um único commit.
> - TODOS os membros da equipe devem se envolver em atividades de desenvolvido do frontend e do backend.

## Como funciona a entrega do projeto final <a name="fluxo"></a>

O projeto final não usa mais o GitHub Classroom. O fluxo passa por um
formulário, um repositório de equipe já pronto no GitHub, e duas
aprovações do professor via Pull Request: uma na proposta, outra na
entrega final.

### Formulário e repositório da equipe <a name="formulario"></a>

Preencha o formulário abaixo — uma resposta por equipe (um integrante
preenche pelos demais):

<a href="https://forms.gle/xuZcYUVpqtrX4XDP8" class="btn" target="_blank">Formulário de equipes</a>

- Informe o tema do projeto e, para cada integrante, nome completo,
  matrícula e o **link do perfil do GitHub** (ex: `github.com/seu-usuario`).

{: .warning }
Confira o link do perfil do GitHub de cada integrante antes de enviar. 
Essa informação é essecial para que seja possível adicionar os membros da equipe
como colaboradores do repositório da equipe — um link errado significa que a pessoa errada (ou ninguém)
recebe acesso.

Depois disso, após  processar as respostas, cada integrante recebe um
**convite de colaborador** (por e-mail, ou em
<a href="https://github.com/notifications" target="_blank">github.com/notifications</a>)
para o repositório da equipe, já criado a partir do template da
disciplina. **Aceite o convite** e clone o repositório:

```bash
git clone https://github.com/profBruno-UFC-Qx/<nome-do-repositorio>.git
```

<hr>

### Envio da proposta <a name="envio-proposta"></a>

No repositório da equipe, crie uma branch e edite o arquivo
**`PROPOSTA.md`**, preenchendo todas as seções (objetivo, público-alvo,
funcionalidades, entidades...):

```bash
git checkout -b proposta
# edite PROPOSTA.md
git add PROPOSTA.md
git commit -m "Proposta do projeto"
git push origin proposta
```

Abra um **Pull Request** da branch `proposta` para `main` no GitHub. Um
check automático confere se todas as seções foram preenchidas (sem o
texto de exemplo).  Passando nessa primeira validação, a proposta terá seu conteúdo revisado. 
Qualquer ajuste necessário será informado diretamente no PR — **o desenvolvimento só está oficialmente
liberado depois do merge**.

{: .warning }
> Os temas devem ser distintos entre as equipes da disciplina. A ordem de
> envio determina a prioridade sobre um tema — se já tiver sido escolhido
> por outra equipe, proponha um novo.

<hr>

### Desenvolvimento <a name="desenvolvimento"></a>

Depois da proposta aprovada, desenvolva o projeto livremente em uma ou
mais branches, sem precisar de aprovação do professor a cada commit ou PR
intermediário. A branch `main` só recebe o merge da proposta e, mais
adiante, o merge da entrega final — todo o código da equipe deve estar
incluído na branch usada na entrega.

{: .warning }
TODOS os membros da equipe devem se envolver na escrita de código.

<hr>

### Entrega final <a name="envio-entrega"></a>

Próximo ao prazo final, garanta que todo o código do projeto está na
branch, crie/atualize uma branch e edite o arquivo **`ENTREGA.md`**
preenchendo: como executar o projeto, credenciais de acesso para teste,
uso de ferramentas de Inteligência Artificial e as maiores dificuldades
encontradas.

```bash
git checkout -b entrega-final
# edite ENTREGA.md
git add ENTREGA.md
git commit -m "Entrega final"
git push origin entrega-final
```

Abra um Pull Request da branch `entrega-final` para `main`. Um check
automático confere se as seções obrigatórias de `ENTREGA.md` foram
preenchidas. **O merge desse PR é a
confirmação formal da entrega**.

{: .warning }
> Na data final, todo o código deve estar disponível no GitHub. Não serão
> aceitos trabalhos enviados em formato compactado (zip, rar etc.) nem
> implementados em um único commit.
>
> Caso o trabalho seja feito em equipe, cada membro deve usar o próprio
> usuário do GitHub para escrever código.

## Apresentação do trabalho <a name="apresentacao"></a>

O trabalho também deverá necessariamente ser apresentado conforme cronograma da disciplina..
