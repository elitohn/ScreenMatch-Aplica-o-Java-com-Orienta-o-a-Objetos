# ScreenMatch – Java, Orientação a Objetos e Consumo de API

Este projeto é uma aplicação em Java desenvolvida com o objetivo de praticar e consolidar os principais conceitos da Programação Orientada a Objetos (POO), manipulação de coleções de dados e integração com APIs externas.

A aplicação começou como um sistema simples de streaming, permitindo trabalhar com filmes, séries e episódios, calcular tempo total de duração e gerar recomendações.

Com a evolução do projeto, foi implementada a integração com a API do OMDb, permitindo buscar informações reais de filmes via requisições HTTP e converter os dados JSON para objetos Java.

---

## 🚀 Funcionalidades

### 🎬 Sistema de Streaming
- Cadastro de filmes e séries  
- Exibição de ficha técnica  
- Sistema de avaliações e cálculo de média  
- Cálculo do tempo total para maratonar conteúdos  
- Filtro de recomendação baseado em classificações  
- Manipulação de listas com `ArrayList`  
- Percorrer coleções com `forEach`  
- Ordenação de objetos personalizados  
- Critérios de ordenação customizados  

### 🌐 Integração com API
- Consumo da API do OMDb  
- Construção de requisições HTTP com `HttpClient`  
- Uso de `HttpRequest` e `HttpResponse`  
- Conversão de JSON para objeto Java utilizando Gson  
- Validação de erros retornados pela API  
- Tratamento de diferentes tipos de exceptions  
- Criação de exception personalizada  
- Lançamento de exceptions com `throw`  

---

## 🧠 Conceitos Aplicados

### 🔹 Programação Orientada a Objetos
- Encapsulamento  
- Herança  
- Polimorfismo  
- Sobrescrita de métodos (`toString`)  
- Uso de `super` para chamada do construtor da classe mãe  
- Uso de interfaces  
- Implementação da interface `Comparable`  

### 🔹 Construtores
- Construtor padrão (default)  
- Construtores com parâmetros  
- Encadeamento de construtores  

### 🔹 Coleções e Listas
- Interface `List`  
- Classe `ArrayList`  
- Classe `LinkedList`  
- Métodos `add()`, `get()`, `size()`  
- Uso de `foreach`  
- Casting de objetos  
- Uso de `instanceof`  

### 🔹 Ordenação
- Uso de `Collections.sort()`  
- Implementação do método `compareTo()`  
- Ordenação personalizada com `List.sort()` e `Comparator`  

### 🔹 Consumo de API
- Conceito de API REST  
- Funcionamento básico de requisições HTTP  
- Integração com API externa  
- Uso das classes:
  - `HttpClient`
  - `HttpRequest`
  - `HttpResponse`

### 🔹 Tratamento de Erros
- Uso de `try/catch`  
- Tratamento de `IOException`  
- Tratamento de `InterruptedException`  
- Criação de exception personalizada  
- Validação de dados antes da conversão  

### 🔹 Manipulação de JSON
- Instalação manual de biblioteca externa (.jar)  
- Uso da biblioteca Gson  
- Conversão de JSON para objeto Java (`fromJson`)  
- Uso de `@SerializedName`  

---

## 🛠️ Tecnologias Utilizadas

- Java  
- API de Collections do Java  
- API HTTP do Java (`java.net.http`)  
- Biblioteca Gson  
- Paradigma Orientado a Objetos  

---

## 📂 Estrutura do Projeto

- `modelos` → Classes principais do domínio (Filme, Série, Episódio, Título)  
- `calculos` → Regras de negócio como cálculo de tempo e filtro de recomendação  
- `service` → Classe responsável pelo consumo da API  
- `exception` → Exception personalizada criada para tratamento de erros  
- `Principal` → Classe responsável por executar e testar a aplicação  
- `listas` (ou classe equivalente criada no curso) → Manipulação e testes com coleções  

---

## 🎯 Evolução do Projeto

Este projeto começou aplicando os fundamentos da Orientação a Objetos e evoluiu para incluir:

- Manipulação de coleções  
- Ordenação de objetos personalizados  
- Uso de interfaces para ganho de flexibilidade  
- Aplicação prática de polimorfismo com listas  
- Consumo de API externa  
- Conversão de JSON para objetos Java  
- Tratamento estruturado de exceptions  

Representando um avanço importante na minha jornada com Java, saindo de fundamentos de POO para aplicações mais próximas do mercado, envolvendo integração com serviços externos e maior robustez no tratamento de falhas.

---

## 📚 Cursos

Projeto desenvolvido durante os cursos:

- **Java: aplicando a Orientação a Objetos**  
- **Java: trabalhando com listas e coleções de dados**  
- **Java: consumindo API, gravando arquivos e lidando com erros**  

Da plataforma Alura.
