
# Estrutura Hexagonal (Ports & Adapters):

A estrutura Hexagonal, também conhecida como "Ports & Adapters", é similar à Onion Architecture, mas separa explicitamente as interfaces (ports) da implementação concreta (adapters). Essa abordagem reforça a independência do núcleo da aplicação.
## Uso/Exemplos

```
src/main/java
├── com.example.projeto
│   ├── application
│   │   ├── service
│   │   │   └── ProdutoService.java
│   │   └── usecase
│   │       ├── CriarProdutoUseCase.java
│   │       └── ObterProdutoUseCase.java
│   ├── domain
│   │   ├── entity
│   │   │   └── Produto.java
│   │   └── repository
│   │       └── ProdutoRepository.java
│   ├── port
│   │   ├── input
│   │   │   └── CriarProdutoPort.java
│   │   └── output
│   │       └── ObterProdutoPort.java
│   └── adapter
│       ├── controller
│       │   └── ProdutoController.java
│       ├── repository
│       │   └── ProdutoRepositoryImpl.java
│       └── web
│           └── ProdutoControllerAdapter.java
└── test
    ├── java
    │   └── com.example.projeto
    │       ├── application
    │       │   └── usecase
    │       │       ├── CriarProdutoUseCaseTest.java
    │       │       └── ObterProdutoUseCaseTest.java
    │       └── domain
    │           └── entity
    │               └── ProdutoTest.java
    └── resources
        └── application.properties

```

## Organização:
- application: Casos de uso e serviços da aplicação.
- domain: Entidades e regras de negócio.
- port: Interfaces que definem as portas de entrada e saída da aplicação.
- adapter: Adaptadores para frameworks e tecnologias externas.
- web: Adaptadores para frameworks web (Spring MVC, etc.).
- persistence: Adaptadores para bancos de dados (JPA, Hibernate, etc.).

##  Vantagens:

Independência ainda maior: O núcleo da aplicação depende apenas de interfaces, não de implementações concretas.
Clareza na separação de preocupações: Separação explícita entre ports e adapters.
Altamente testável: Facilidade para testes de unidade e integração.

##  Desvantagens:
Maior complexidade: Similar à Onion Architecture, requer maior conhecimento de conceitos avançados.
Overkill para projetos simples: Pode ser desnecessária para projetos pequenos.
Aumento da verbosidade: Nomes como "port" e "adapter" podem ser menos intuitivos.