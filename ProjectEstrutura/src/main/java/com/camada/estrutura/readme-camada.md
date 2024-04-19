
# Estrutura em Camadas (Camadas Clássicas):

A estrutura em camadas, também conhecida como "Camadas Clássicas" ou "MVC (Model-View-Controller)", é uma das mais tradicionais e difundidas. Sua simplicidade e clareza a tornam uma escolha popular para projetos iniciantes ou de médio porte.


## Uso/Exemplos

```
src/main/java
├── com.camada.estrutura
│   ├── model
│   │   ├── produto
│   │   │   └── Produto.java
│   │   └── pedido
│   │       └── Pedido.java
│   ├── service
│   │   ├── produto
│   │   │   ├── ProdutoService.java
│   │   │   └── ProdutoServiceImpl.java
│   │   └── pedido
│   │       ├── PedidoService.java
│   │       └── PedidoServiceImpl.java
│   ├── controller
│   │   ├── produto
│   │   │   └── ProdutoController.java
│   │   └── pedido
│   │       └── PedidoController.java
│   ├── repository
│   │   ├── produto
│   │   │   └── ProdutoRepository.java
│   │   └── pedido
│   │       └── PedidoRepository.java  
│   ├── util
│   │   ├── Email
│   │       └── EmailUtil.java  
│   │   └── Cripto
│   │       └── CriptoUtil.java 
└── test
    ├── java
    │   └── com.example.api
    │       ├── model
    │       │   └── produto
    │       │       └── ProdutoTest.java
    │       └── service
    │           └── produto
    │               └── ProdutoServiceTest.java
    └──────────────────────────────────────────
```


## Organização:
- model: Classes que representam os dados da aplicação (entidades).
- service: Classes que implementam a lógica de negócio da aplicação.
- controller: Classes que controlam a interação com o usuário e gerenciam os endpoints da API.
- repository: Classes que acessam e manipulam dados em um banco de dados.
- util: Classes com funcionalidades auxiliares (validação, conversão de dados, etc.).

##  Vantagens:

Simplicidade: Fácil de entender e implementar, ideal para iniciantes.
Organização clara: Separa as responsabilidades em camadas bem definidas.
Fácil navegação: Encontrar classes e funcionalidades é intuitivo.
Desvantagens:

##  Desvantagens:
Falta de modularidade: Pode ser rígida para projetos maiores e complexos.
Dificuldade de testabilidade: Testar unidades em camadas interligadas pode ser desafiador.
Limitações em arquiteturas complexas: Menos flexível para microsserviços ou DDD (Design Orientado a Domínio).

