# dieacetaria – Estrutura da organização

## Repositórios

Diferentes projetos dividem-se em múltiplos repositórios, contendo um repositório principal (este com o nome do projeto, sem adições) para criação de issues de design e business.

Outros repositórios criam-se utilizando o nome do projeto com adição de nome descritivo do propósito deste.

**Obs.: Repositórios não devem ter boards individuais.** 

> **Exemplo** – Projeto "Abacaxi" – Repositórios:
> - *abacaxi*: Repositório principal.
> - *abacaxi-frontend*: Repositório frontend do projeto abacaxi.
> - *abacaxi-notifications*: Repositório para o microsserviço de notificações do projeto abacaxi.
> - *abacaxi-android*: Repositório para a aplicação Android do projeto abacaxi.

## Projetos

Todos os projetos desenvolvidos são separados em dois projetos do Github.

*Cuidado para não confundir "projeto" desenvolvidos com "projetos" do Github. Projetos do Github são boards Kanban.*

> **Exemplo** – Projeto "Abacaxi" – Projetos (boards do Github):
> - *abacaxi-upstream*
> - *abacaxi-downstream*

##### Downstream
Board destinado às issues relacionadas ao desenvolvimento e à todas as outras issues que não se encaixem no Upstream.

##### Upstream
Board para validação de ideias. Todas as funcionalidades à serem desenvolvidas passam por este board antes.

## Issues

Issues podem ser divididas em quatro categorias:

##### Issues de desenvolvimento
Devem ser criadas no repositório específico e adicionadas ao board *downstream* do projeto.

##### Issues de blueprint
São relacionadas ao processo de validação de ideias (board *upstream*) mas requerem algum esforço técnico.

Devem ser criadas no repositório principal do projeto e adicionadas ao board *downstream* do projeto.

##### Issues de ideias
São as potenciais funcionalidades ou melhorias do projeto, passam pelo processo de *upstream*.

Devem ser criadas no repositório principal do projeto e adicionadas ao board *upstream* do projeto.

##### Issues gerais
São issues não possíveis de categorização nos outros grupos, relacionadas à criação de documentações, *pitchs*, formulários, etc.

Devem ser criadas no repositório principal do projeto e adicionadas ao board *downstream* do projeto.

### Da criação das issues...

Todas as issues criadas **obrigatoriamente** têm definidos:

- Título
- Descrição mínima para compreensão da tarefa
	- Caso seja uma issue de *desenvolvimento* ou *blueprint*, portanto advinda de outra issue de *ideia*, deve ter a issue de *ideia* relacionada em sua descrição: `Related to #[NumeroDaIssueDeIdeia]`
- Assignees
- Labels
- Projects
- Milestone
