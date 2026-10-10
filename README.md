# 🖥️ TechFlow

Aplicação front-end para gerenciar **projetos** e **equipes**, com cadastro por meio de modais, tema claro/escuro e layout responsivo para celulares, tablets, notebooks e desktops.

## Integrantes

| Nome | RM |
| --- | --- |
| [Lorenzo Mendes Pena](https://github.com/MendesPenaLorenzo) | 570036 |
| [Murillo Perez da Fonseca](https://github.com/MurilloFonseca) | 573674 |

## Tecnologias utilizadas

- **HTML5**: estrutura semântica das páginas, formulários e modais.
- **JavaScript (ES6+)**: toda a interatividade, em JavaScript puro, sem frameworks.
- **Tailwind CSS v4**: estilização por classes utilitárias, com cores e fontes próprias definidas em `@theme` e variante `dark` controlada pelo atributo `data-theme`.
- **Fontes Sansation e DM Mono**: carregadas localmente via `@font-face`.
- **Git e GitHub**: versionamento e hospedagem do código.

## Principais recursos implementados

**Projetos**
- Listagem em cards com nome, status (Pendente, Em andamento ou Concluída), responsável, categoria, prioridade, prazo e descrição.
- Modal para adicionar um novo projeto, acionado pelo botão `+`, com os campos nome, responsável, categoria, prioridade (dropdown com alta, média e baixa), prazo e descrição.
- Validação dos campos obrigatórios e do prazo, que não aceita datas passadas.
- O novo projeto aparece imediatamente no início da lista.

**Equipes**
- Listagem em cards com nome, responsável e membros.
- Modal para adicionar uma nova equipe, com nome, responsável e uma lista de membros.
- Os membros são adicionados com Enter ou com o botão **Adicionar**, aparecem como itens removíveis e não aceitam nomes repetidos. É necessário informar ao menos um membro.

**Interface**
- Tema **claro**, **escuro** ou **do sistema**, com a escolha salva no navegador.
- Barra lateral recolhível. No desktop a preferência é lembrada; em celulares e tablets ela vira um menu sobreposto.
- Layout responsivo: a grade de cards se ajusta à largura disponível, de 1 coluna no celular a várias no desktop.

**Qualidade e acessibilidade**
- Modais fecham com o botão de fechar, "Cancelar", clique no fundo ou tecla `Esc`, e devolvem o foco ao botão de origem.
- Rótulos acessíveis nos botões e nos campos, e atributos `aria` nos diálogos.
- O conteúdo digitado nos formulários é inserido como texto, o que impede a injeção de HTML nos cards.

> **Observação:** os projetos e as equipes cadastrados ficam apenas na memória da página e são perdidos ao recarregar. Ainda não há persistência de dados.

## Link do GitHub

<https://github.com/MurilloFonseca/techflow-dashboard>
