<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&height=175&color=0:0F172A,55:164E63,100:0891B2&text=ScreenMatch&fontColor=FFFFFF&fontSize=34&fontAlignY=38&desc=Filmes%2C%20s%C3%A9ries%20e%20Java&descAlignY=61&descSize=15" alt="Capa do projeto ScreenMatch" width="100%" />

![Tecnologias](https://img.shields.io/badge/Java%20e%20Gson-0F172A?style=flat-square) ![Idioma](https://img.shields.io/badge/documentação-pt--BR-0891B2?style=flat-square) ![Tipo](https://img.shields.io/badge/projeto-de%20estudo-334155?style=flat-square)

</div>

# ScreenMatch — Java, orientação a objetos e consumo de API

Projeto de console para praticar modelagem de filmes e séries, avaliações, cálculo de duração, coleções Java e consumo da API OMDb.

## O que o projeto demonstra

- Criar filmes, séries e episódios e exibir suas fichas técnicas;
- Registrar avaliações e calcular médias;
- Calcular o tempo total de uma seleção de títulos;
- Filtrar recomendações;
- Ordenar coleções e comparar títulos;
- Consultar filmes na OMDb, converter a resposta JSON para objetos Java e salvar os resultados em `filmes.json`.

Há três classes de entrada independentes:

| Classe | O que executa |
|---|---|
| `Principal` | Exemplos locais de filmes, séries, avaliações, duração e recomendação; não precisa de internet. |
| `PrincipalcomListas` | Exercícios de listas, ordenação e comparação de títulos. |
| `PrincipalcomBusca` | Busca títulos na OMDb e grava a lista consultada em `filmes.json`; precisa de internet e de uma chave da API. |

## Tecnologias

- Java 17 ou superior;
- API HTTP padrão do Java (`java.net.http`);
- Gson 2.10.1;
- IntelliJ IDEA (configuração do projeto).

O repositório não tem Maven ou Gradle. O arquivo `screenmatch.iml` referencia Gson em `Downloads/gson-2.10.1.jar` no diretório do usuário; em outra máquina, configure o caminho da dependência no IntelliJ.

## Como executar no IntelliJ IDEA

1. Instale um JDK 17 ou superior e abra o repositório no IntelliJ IDEA.
2. Baixe o Gson 2.10.1.
3. Se o IntelliJ não encontrar a biblioteca, abra **File → Project Structure → Modules → Dependencies** e adicione o arquivo `.jar` em **+ → JARs or Directories**.
4. Abra uma das classes de entrada em `src/br/com/alura/screenmatch/principal/`.
5. Execute a classe desejada pelo botão **Run** ao lado do método `main`.

Para começar sem configurar uma API, execute `Principal`. Para usar `PrincipalcomBusca`, siga também a seção abaixo.

## Busca na OMDb

A classe `PrincipalcomBusca` pergunta o nome de um filme, consulta a OMDb e salva os títulos encontrados em `filmes.json`. Digite `sair` para finalizar a busca e gravar o arquivo.

A OMDb exige uma chave de API própria. **A versão atual do código contém uma chave diretamente em `PrincipalcomBusca.java`.** Se ela for válida, considere-a exposta: revogue-a e gere outra. Não publique chaves no código nem em commits; configure a sua localmente antes de executar essa classe.

## Organização

```text
.
├── src/br/com/alura/screenmatch/
│   ├── calculos/       # cálculo de tempo e filtros de recomendação
│   ├── excecao/        # exceções personalizadas
│   ├── modelos/        # filmes, séries, episódios e títulos OMDb
│   └── principal/      # classes com métodos main
├── filmes.json
└── screenmatch.iml
```

## Cursos

Projeto desenvolvido durante os cursos da Alura sobre orientação a objetos, coleções, consumo de API, gravação de arquivos e tratamento de erros.
