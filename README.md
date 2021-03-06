<h2 align="center">Primeiro projeto Node && TypeScript</h2>

<p align="center">
<a href="https://insomnia.rest/run/?label=&uri=https%3A%2F%2Fgithub.com%2Fmiroswd%2FfirstProject%2Fblob%2Fmaster%2Fassets%2Froutes-gostack-gobarber.json" target="_blank"><img src="https://insomnia.rest/images/run.svg" alt="Run in Insomnia"></a>
</p>

<p align="center">Construindo o back end da aplicação 'GoBarber'.</p>

</br>

```bash
docker run --name gobarber -e POSTGRES_PASSWORD=suasenha -p 5432:5432 -d postgres # Caso a porta 5432 esteja ocupada, modificar de 5432:5432 para 5433:5432
```

- Criar uma database chamada <b>gostack_gobarber</b> 
- Rodar as migrations

```bash
yarn typeorm migration:run
```

- Inicializar o projeto

```bash
yarn dev:server
yarn test # para rodar os testes
```

* Model => Representação de como o dado é salvo
* Router => Recebe a requisição, chama outro arquivo e retorna uma resposta
* Repositories => Lida com os dados, CRUD


Padronizado com:
* EditorConfig
* ESLint
* Prettier

Libs utilizadas:
* uuidv4 => para gerar id
* typeorm => mapeamento dos objetos para o banco de dados
* date-fns => fazer a tratativa de datas/horários
* multer => Upload de arquivos
* tsyringe => Injeção de dependências
* Jest => Criação de testes automatizados
* Handlebars => Template Engine
