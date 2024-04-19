
# Estrutura Onion (Camadas Aninhadas):

A estrutura Onion, também conhecida como "Camadas Aninhadas" ou "Clean Architecture", propõe uma organização em camadas concêntricas, com o núcleo da aplicação independente de frameworks e tecnologias externas. Essa estrutura visa princípios de alto acoplamento e baixa dependência.

## Uso/Exemplos

```
src/main/java
├── com.example.projeto
│   ├── core
│   │   ├── application
│   │   │   └── service
│   │   │       └── ProdutoService.java
│   │   ├── domain
│   │   │   ├── entity
│   │   │   │   └── Produto.java
│   │   │   └── repository
│   │   │       └── ProdutoRepository.java
│   │   └── port
│   │       ├── input
│   │       │   └── CriarProdutoPort.java
│   │       └── output
│   │           └── ObterProdutoPort.java
│   ├── adapter
│   │   ├── controller
│   │   │   └── ProdutoController.java
│   │   └── repository
│   │       └── ProdutoRepositoryImpl.java
│   └── web
│       └── ProdutoControllerAdapter.java
└── test
    ├── java
    │   └── com.example.projeto
    │       ├── core
    │       │   └── application
    │       │       └── service
    │       │           └── ProdutoServiceTest.java
    │       └── domain
    │           └── entity
    │               └── ProdutoTest.java
    └── resources
        └── application.properties

```

## Organização:
- core: Classes do núcleo da aplicação, independentes de frameworks e tecnologias.
- domain: Entidades e regras de negócio.
- application: Casos de uso e serviços da aplicação.
- adapter: Adaptadores para frameworks e tecnologias externas.
- web: Adaptadores para frameworks web (Spring MVC, etc.).
- persistence: Adaptadores para bancos de dados (JPA, Hibernate, etc.).

##  Vantagens:

Baixo acoplamento: O núcleo da aplicação é independente de tecnologias externas.
Alta testabilidade: Fácil testabilidade de unidades no núcleo da aplicação.
Flexibilidade para mudanças: Facilita a adaptação a novas tecnologias e frameworks.

##  Desvantagens:
Maior curva de aprendizado: Requer um bom entendimento de conceitos como Clean Architecture e DDD.
Complexidade em projetos simples: Pode ser desnecessária para projetos pequenos.
Aumento da verbosidade: Nomes de pastas como "core" e "adapter" podem ser menos intuitivos.