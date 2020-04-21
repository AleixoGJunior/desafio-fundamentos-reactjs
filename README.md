# Desafio 7 - Fundamentos do ReactJS

O objetivo do desafio é criar um aplicação para treinar os conhecimentos aprendidos sobre ReactJS.

## Sobre

Continuar desenvolvendo a aplicação de gestão de transações, a GoFinances. Agora você irá praticar o que você aprendeu até agora no React.js junto com TypeScript, utilizando rotas e envio de arquivos por formulário.

Essa será uma aplicação que irá se conectar ao seu backend do Desafio 06, e exibir as transações criadas e permitir a importação de um arquivo CSV para gerar novos registros no banco de dados.

### Funcionalidades da aplicação

- **`Listar os repositórios da sua API`**: Sua página `Dashboard` deve ser capaz de exibir uma listagem através de uma tabela, com o campo `title`, `value`, `type` e `category` de todas as transações que estão cadastradas na sua API.

**Dica**: Você pode utilizar a função [Intl](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/NumberFormat) para formatar os valores. Dentro da pasta `utils` no template você encontrará um código para te ajudar.

- **`Exibir o balance da sua API`**: Sua página `Dashboard`, você deve exibir o balance que é retornado do seu backend, contendo o total geral, junto ao total de entradas e saídas.

- **`Importar arquivos CSV`**: Na sua página `Import`, você deve permitir o envio de um arquivo no formato `csv` para o seu backend, que irá fazer a importação das transações para o seu banco de dados. O arquivo csv deve seguir o seguinte [modelo](https://github.com/Rocketseat/bootcamp-gostack-desafios/blob/master/desafio-database-upload/assets/file.csv).

### Específicação dos testes

Para esse desafio temos os seguintes testes:

- **`should be able to list the total balance inside the cards`**: Para que esse teste passe, sua aplicação deve permitir que seja exibido na sua Dashboard, cards contendo o total de `income`, `outcome` e o total da subtração de `income - outcome` que são retornados pelo balance do seu backend.

* **`should be able to list the transactions`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados dentro de uma tabela, toda as transações que são retornadas do seu backend.

**Dica**: Para a exibição dos valores na listagem de transações, as transações com tipo `income` devem exibir os valores no formado `R$ 5.500,00`. Transações do tipo `outcome` devem exibir os valores no formado `- R$ 5.500,00`.

- **`should be able to navigate to the import page`**: Para que esse teste passe, você deve permitir a troca de página através do Header, pelo botão que contém o nome `Importar`.

**Dica**: Utilize o componente `Link` que é exportado do `react-router-dom`, passando a propriedade `to` que leva para a página `/import`.

## Tecnologia

Este projeto foi desenvolvido utilizando as seguintes tecnologias:

- [ReactJS](https://pt-br.reactjs.org/)
- [Jest](https://jestjs.io/)

## Instalação e Execução

1. Faça a instalações dos pacotes executando o comando: 
```bash 
yarn
```

2. Execute a aplicação com o comando: 
```bash 
yarn start
```

3. Execute os testes com o Jest utilizando o comando: 
```bash
yarn test
```

## Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](https://github.com/AleixoGJunior/desafio-fundamentos-reactjs/blob/master/LICENSE) para mais detalhes.
