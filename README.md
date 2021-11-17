<h1 align="center">API 4º Semestre Banco de Dados</h1>

<h2>Descrição do projeto</h2> 
O projeto VEMPRACASA tem o objetivo de estimular o apredizado e desenvolvimento dos alunos atráves de uma parceria entre a Faculdade de Tecnologia de São Paulo e a Oracle Corporation. A proposta imposta pela empresa era de um software que realizasse o agendamento dos espaços da Casa Oracle, visando as regras de limite máximo de pessoas, priorização de agendamentos, aprovação de eventos pendentes e disponibilização de lista de convidados. O projeto teve o prazo estimulado em um semestre com apresentações a cada três semanas para o parceiro.
    <ol>
        <li> Requisitos 
             <ul><li> Utilização de metodologia agíl para planejamento e execução das sprints do projeto.</li></ul>
            <ul><li> Uso da linguagem de programação Java junto ao framework Spring Boot.</li></ul>
            <ul><li> Banco de dados Oracle para armazenamento das informações</li></ul>
            <ul><li> Deploy da aplicação em um ambiente de nuvem (de preferência Oracle Cloud)</li></ul>
        </li>
    </ol>

<h2> Tecnologias utilizadas</h2> 
Além das técnologias empregadas impostas pelo cliente parceiro, os alunos tambem tiveram a liberdade de analisar e utilizarem outras técnologias necessárias listadas abaixo:
<ol>
    <li>Desenvolvimento agíl
        <ul>
            <li>
                Jira
                </br>Utilizado para o gerenciamento do projeto, possibilitando realizar o planejo das sprints e distribuição das tarefas para cada integrante do grupo,                       podendo mapear e registrar o progresso da equipe e do projeto a cada etapa finalizada, desse modo, facilitando o desenvolvimento e previnindo a realização de retrabalho
            </li>
        </ul>
    </li>
    <li>
        Prototipação das telas
        <ul>
            <li>
                Figma
            </li>
            Figma foi utilizado para a aplicação dos conceitos de UX/UI, prototipação dos user stories, wireframes e construção dos MVPs
        </ul>
    </li>
     <li>Desenvolvimento Back-end
        <ul>
            <li>
                Java
                </br> Linguagem de programação orientada a objetos utilizada para o desenvolvimento back-end da aplicação com requisito técnico do cliente parceiro, junto ao framework Spring Boot para aumento de produtividade e configurações do projeto
            </li>
             <li>
                Spring Boot
                </br>Spring Boot é um framework open source para Java e Kotlin, utilizado para facilitar o desenvolvimento de aplicações,
                configurações e gerenciamento de um projeto, dessa forma melhorando a produtividade. 
            </li>
        </ul>
    </li> <li>Desenvolvimento Front-end
        <ul>
            <li>
                Angular 
                </br>O desenvolvimento front-end foi realizado com Angular uma plataforma para desenvolvimento de aplicações web com um código open source com base em TypeScript, foi escolhido pela equipe pela possibilidade de criação de páginas dinâmicas e otimização de trabalho e reinscrita de código. 
            </li>
             <li>
                MirageJS
                </br>Para a realização de testes(quando não havia conexão entre back-end e front-end) foi utilizado o MirageJS, ele funciona como uma API porém com dados mockados, dessa forma, tirando a dependência que o front tem sobre os endpoints do back-end durante o desenvolvimento.
            </li>
        </ul>
    </li> <li>Banco de dados
        <ul>
            <li>
                Oracle
                </br> Na parte de armazenamento de dados, foi utilizado o Oracle database em sua versão 12c, um SGBD relacional, escolhido por atender todas as necessidades do projeto e ser uma ferramenta da empresa parceira.
            </li>
            <li>
                SQL Developer
                </br> Um ambiente de desenvolvimento que possibilita a realização de scripts SQL em bancos de dados Oracle.
            </li>
        </ul>
    </li><li>Deploy
        <ul>
            <li>
                Oracle Cloud 
                </br> Infraestrura em nuvem para realização de deploy do banco de dados em produção, escolhido pela equipe por ser uma ferramenta da empresa parceira
            </li>
            <li>
                Heroku
                </br> Plataforma em nuvem como um serviço que suporta várias linguagens de programação, utilizado para realizar o deploy da aplicação web em ambiente de produção.
            </li>
        </ul>
    </li>
</ol>

<h2>Contribuições individuais</h2>
<h3>Contribuições desenvolvedor Backend</h3>.
<p>Entre as responsabilidade de um desenvolvedor back-end estão: Arquitetura do projeto, escolha de tecnologia, entendimento das regras de negócio e realização da lógia de programação.</br>
Como desenvolvedor participei ativamente em cada uma dessas partes.
O projeto foi gerado utilizando o Spring initializer, criando o esboço do projeto com as dependências necessárias para as primeiras linhas de código.
  <details>
  <summary>Spring initialize</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>
  </br>
Após ter o esboço do projeto em mãos, seguindo o conceito de boas práticas de programação a arquitetura do projeto foi definida em "Model","Controller", "Service", "Repository" separados por pacotes do Java.</p>
  <details>
  <summary>Arquitetura do Projeto</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>

<ul><li>Model: No pacote das models é onde está localizado as classes referentes as tabelas do banco de dados, ou seja cada classe referencia uma tabela, sendo cada variável uma coluna da tabela.</li>
  <details>
  <summary>Model</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>
<li>Controller: No pacote dos Controllers é onde estão as chamadas dos endpoints, foram criadas uma classe de controller para cada model. Sua função é indicar qual requesição deve ser realizada e qual seu endereço, porém não se deve realizar o desenvolvimento de regras de negócio nessas classes, para chamada dos metódos com a lógica e regras de negócio é necessário referenciar um service.</li>
      <details>
  <summary>Controller</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>
<li>Service: No pacote dos services estão as classes responsaveis por conter as regras de negócios e os metódos com as lógicas necessárias, porém caso algum metódo necessite realizar operações no banco de dados, deve se ser referenciado um repository.</li>
  <details>
  <summary>Service</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>
<li>Repository: No pacote dos repositorys é onde se encontra as interfaces responsáveis por realizar as operações no banco de dados, a interface extende a classe "JPARepository", esta classe otimiza o desenvolvimento pois todos os metódos para realização de uma operação no banco já estão prontos, necessitando apenas da sua chamada em sua classe repository.</li>
  <details>
  <summary>Repository</summary>
  <br>
   <img style="border-radius: 50%;" src="" width="800px;" alt=""/>
  </details>
</ul>

    

