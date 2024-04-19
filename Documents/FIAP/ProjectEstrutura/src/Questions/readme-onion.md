
# Perguntas Frequentes


## Pergunta:
1. Como você depura problemas de código?

 - Descrição: Essa pergunta avalia suas habilidades de análise e resolução de
problemas na identificação e correção de erros em código.
 - Resposta: Descreva seu processo de depuração de código de forma clara e
concisa. Mencione as ferramentas que você utiliza (debuggers, linters, etc.),
estratégias que você adota (análise de logs, testes unitários, etc.) e
metodologias que você segue para encontrar e corrigir erros de forma eficiente.

2. Explique os princípios de SOLID.

- Descrição: Essa pergunta verifica seu conhecimento sobre os princípios de SOLID,
considerados boas práticas de design de software orientado a objetos.

- Resposta: Apresente os cinco princípios do SOLID (Single Responsibility,
Open-Closed, Liskov Substitution, Interface Segregation e Dependency Inversion)
de forma clara e concisa. Explique como cada princípio funciona e como você os
aplica em seu trabalho para escrever código modular, reutilizável, fácil de
manter e testar.

3. Qual a diferença entre REST e SOAP?

- Descrição: Essa pergunta avalia seu conhecimento sobre as arquiteturas REST e
SOAP, utilizadas para implementar serviços web.
-
- Resposta: Diferencie as arquiteturas REST e SOAP em termos de princípios,
características, casos de uso e vantagens de cada uma. Enfatize os pontos
chave que as distinguem, como flexibilidade, escalabilidade, simplicidade e
padronização.
-
- REST - mensagens atráves de http e url
- SOAP - mensagens através de xml

4. O que você sabe sobre design de padrões?

- Descrição: Essa pergunta verifica seu conhecimento sobre design de padrões,
soluções reutilizáveis para problemas comuns de desenvolvimento de software.
-
- Resposta: Explique o conceito de design de padrões e cite alguns exemplos de
padrões comumente utilizados (Singleton, Factory Method, Observer, etc.).
Mencione como os padrões podem ajudar a escrever código mais eficiente,
flexível e reutilizável.

## Java:

- Encapsulamento: O encapsulamento é um dos princípios da programação orientada a objetos que visa ocultar a implementação interna de um objeto e expor apenas seus métodos e atributos públicos.
- Isso promove a modularidade, organização do código e reduz a dependência entre classes.
- 
- Ciclo de vida de um objeto Java:
-
- Criação: O objeto é instanciado usando o operador new.
- 
- Inicialização: O construtor da classe é executado para inicializar os atributos do objeto.
- 
- Uso: O objeto é utilizado em seu contexto de aplicação, interagindo com outros objetos e métodos.
-
- Coleta de lixo: Quando o objeto não é mais referenciado, a coleta de lixo o remove da memória.
- 
- Exceções checadas e não checadas:
-
- Exceções checadas: Compiladores obrigam o tratamento explícito. Relacionadas a erros de fluxo de programa (ex: FileNotFoundException).
- Exceções não checadas: Não exigem tratamento explícito. Relacionadas a erros lógicos ou de runtime (ex: NullPointerException).
- 
- Padrão de design Singleton: Garante que exista apenas uma instância de uma classe em todo o programa.
Implementado usando um atributo estático privado, um método de acesso público e sincronização.
- 
- Garbage collection: Mecanismo automático que gerencia a memória alocada para objetos Java.
Libera memória de objetos não utilizados, otimizando o uso da memória e evitando fragmentação.
- Thread-safety: Garante que um objeto possa ser acessado por várias threads sem causar problemas de consistência de dados.
Implementada usando mecanismos como sincronização, locks e atomicidade.
-
- Lambdas e streams: Lambdas fornecem uma forma concisa e expressiva de escrever código funcional.
Streams permitem processar coleções de dados de forma eficiente e elegante.

## SpringBoot:

- Simplificação do desenvolvimento:

- Autoconfiguration: simplifica a configuração da aplicação, detectando automaticamente beans e recursos.
- 
- Anotações Spring Boot: facilitam o desenvolvimento de aplicações web, RESTful APIs e serviços em geral.
- Processo de autoconfiguration: O Spring Boot verifica a classe @SpringBootApplication e o classpath para identificar beans e recursos.
Configura automaticamente beans com base em anotações e convenções.
Permite customização manual da configuração.
- 
- Anotações Spring Boot:
- @SpringBootApplication: marca a classe principal da aplicação, habilitando recursos do Spring Boot.
- @RestController: marca classes como controllers RESTful.
- @Autowired: injeta dependências automaticamente.
- @ConfigurationProperties: mapeia propriedades do arquivo application.properties para classes.
- 
- Integração com banco de dados:
- Spring Data JPA: fornece uma abstração simplificada para acesso a bancos de dados relacionais.
Anotações como @Entity, @Repository e @Transactional facilitam a persistência de dados.
-
- Segurança Spring Security:
- Autenticação: verifica a identidade do usuário.
- Autorização: controla o acesso a recursos da aplicação.
- Proteção contra ataques como CSRF, XSS e SQL Injection.
-
- Testes com Spring Boot:
- Spring Boot Test: fornece suporte para testes unitários e de integração.
- MockMvc: simula requisições HTTP para testar controllers RESTful.
- Testes de carga e desempenho também são possíveis.

## Docker:
- Benefícios dos containers:
- 
- Isolamento: cada container possui seu próprio sistema de arquivos e processo, tornando-os independentes e portáveis.
- Padronização: ambientes de desenvolvimento, testes e produção podem ser replicados com fidelidade.
- Agilidade: containers podem ser criados, inicializados e removidos rapidamente.
-
- Docker Compose: Ferramenta para definir e gerenciar multi-container applications.
Simplifica a configuração e o provisionamento de infraestrutura complexa.
Define os containers, seus volumes, redes e dependências em um único arquivo YAML.
-
- Dockerfiles: Instruções para construir imagens Docker.
Definem o sistema operacional base, instalam softwares, configuram o ambiente e definem o ponto de entrada da aplicação.
Padronizam a criação de imagens e garantem reprodutibilidade.
Melhores práticas para Docker em produção:
- 
- Versionamento de imagens: utilize tags para identificar diferentes versões da imagem.
- 
- Armazenamento em registro de imagens: armazene imagens

## TCP vs UDP:

- TCP: Conexão orientada, confiável, com controle de fluxo e entrega ordenada.
- 
- UDP: Sem conexão, não confiável, sem controle de fluxo ou entrega ordenada.

## Modelos de Serviço de Cloud Computing:
IaaS: Infraestrutura como Serviço (ex: Amazon EC2, Azure Virtual Machines).
PaaS: Plataforma como Serviço (ex: Google App Engine, Heroku).
SaaS: Software como Serviço (ex: Salesforce, Office 365).