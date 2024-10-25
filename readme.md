## Desafio

Construir uma aplicação web para realizar o cadastro de itens.

A aplicação deverá ser composta por 2 páginas, sendo uma para cadastro e outra para listagem. Ambas as páginas devem possuir um menu lateral, localizado à esquerda, com links para as mesmas, além de um sistema de navegação estrutural.

Os dados devem ser persistidos no formato JSON, fazendo uso da LocalStorage, adicionando, removendo e editando itens do JSON em questão. Não é necessária a utilização de APIs externas.

Cada página será melhor descrita a seguir:

### 1- Formulário:
Deve ser criado um formulário com validação conforme os campos descritos a seguir para cadastro de itens. É necessário informar com clareza os campos que apresentem erro de validação ou obrigatoriedade.

| Campo | Tipo | Obrigatoriedade | Validação |
| --- | --- | --- | --- |
| Nome do item | Texto | Sim | Tamanho máximo de 70 caracteres  |
| Categoria | Enumeração | Sim | Automovel, caminhão, Avião |
| Quantidade | Numérico | Só é obrigatório caso o produto seja ativo |  - |
| Preço | Monetário | Só é obrigatório caso o produto seja ativo | Validações de campo monetário\*|
| Ativo | Checkbox booleano | Sim | - |



\* Validação de campo monetário incluí exibição do tipo de moeda no início do campo e limite de casas decimais utilizando máscara (preenchimento da direita para esquerda).

O formulário deverá possuir dois botões, um para salvar e outro para cancelar. Ao selecionar o botão de salvar, caso esteja editando um item, deve salvar essas alterações, do contrário um novo será adicionado. O botão de cancelar direciona o usuário para a tela de listagem.

### 2- Listagem:

A listagem deverá exibir uma tabela com os itens cadastrados, bem como um link para edição e exclusão de cada item, e um botão para adicionar um novo item. A busca dos itens para listagem deve ser realizada de forma assíncrona. Ao clicar em excluir o usuário deverá ser questionado se realmente deseja excluir o item em questão. Caso sim, o item deverá ser removido e exibida uma notificação de sucesso ou erro.

Ao clicar em editar, o usuário deverá ser redirecionado para o formulário, carregado com os dados do item em questão. O botão de adicionar apenas redirecionará para a página do formulário.

#### Tecnologias e conceitos que serão avaliados:

- Angular 2+ 
- HTML 5;
- CSS;
- TypeScript / JavaScript;
- Rotas;
- Utilização de LocalStorage;
- Recomenda-se a utilização da biblioteca NG ZORRO.

Critérios de avaliação da tela:

- Usabilidade e experiência de uso;
- Responsividade (deve ser ajustável a diferentes tamanhos de tela);
- Padrão visual;
- Cross-browser (deve ser utilizavel em ie 10 +, Edge, Chrome, FireFox)

Critério de avaliação do código:

- Qualidade;
- Clareza;
- Documentação;
- Reutilização (criação de componentes);

