# Screenmatch

**Screenmatch** é uma aplicação Java desenvolvida com o Spring Boot que permite a busca e análise de informações sobre séries de TV. O projeto demonstra a integração com APIs externas, processamento de dados JSON e a apresentação de informações ao usuário.

## Funcionalidades

- **Busca de Séries:** Permite ao usuário buscar séries pelo nome e exibe informações como título, número total de temporadas e avaliação geral.
- **Listagem de Temporadas e Episódios:** Mostra todas as temporadas e episódios da série, detalhando título, número do episódio, avaliação e data de lançamento.
- **Cálculo de Estatísticas:** Calcula e exibe estatísticas sobre as avaliações dos episódios, incluindo média, melhor e pior episódio.

## Estrutura do Projeto

### `br.com.alura.screenmatch`

- **`ScreenmatchApplication`**: Classe principal que configura e inicia a aplicação Spring Boot.

### `br.com.alura.screenmatch.principal`

- **`Principal`**: Contém a lógica para interação com o usuário, incluindo a exibição do menu, busca de dados e processamento das informações obtidas da API.

### `br.com.alura.screenmatch.service`

- **`ConsumoApi`**: Classe responsável por consumir a API externa e obter dados no formato JSON.
- **`ConverteDados`**: Implementa a interface `IConverteDados` para converter JSON em objetos Java usando a biblioteca Jackson.
- **`IConverteDados`**: Interface para conversão de dados JSON.

### `br.com.alura.screenmatch.model`

- **`Episodio`**: Representa um episódio de uma série com detalhes como temporada, título, número do episódio, avaliação e data de lançamento.
- **`DadosTemporada`**: Representa os dados de uma temporada, incluindo o número da temporada e a lista de episódios.
- **`DadosSerie`**: Representa os dados gerais de uma série, como título, número total de temporadas e avaliação.
- **`DadosEpisodio`**: Representa os dados de um episódio individual, incluindo título, número do episódio, avaliação e data de lançamento.

## Tecnologias Utilizadas

- **Java 17+**: Linguagem de programação utilizada para o desenvolvimento.
- **Spring Boot**: Framework para criação de aplicações Java baseadas em Spring.
- **Jackson**: Biblioteca para processamento de JSON.
- **API OMDB**: Fonte de dados para séries e episódios de TV.

## Contribuições
**Contribuições são bem-vindas! Se você tiver sugestões, correções ou melhorias, sinta-se à vontade para abrir uma issue ou um pull request.**

## Autor

Kaio Vitor - [GitHub](https://github.com/Kaio-0708)

