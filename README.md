# careapp

> ***System requirements***
##### IDEs: Netbeans, Intellij, Eclipse
##### Banco de dados: H2
##### Versão db : liquibase
##### Github: git bash
##### Server: Wildfly
##### Gerenciador de projeto: Maven

### Execution
- DB
- Iniciar seu banco de dados H2 com as seguintes configurações:
	(para iniciar, basta executar o jar localizado dentro dos arquivos do banco, geralmente em [por exemplo C:\Program Files (x86)\H2\bin\h2-1.4.200.jar <- pode variar de acordo com sua versão.])
* Saved Settings: `Generic H2 (Server)`
* JDBC URL: `jdbc:h2:tcp://localhost/C:/data/fileDb`
* User Name: `sa`
* Password: `sa`

- Server
 deve ser criado/instanciado um server wildfly
 Goals do server: `wildfly:deploy` (para fazer deploy do projeto) e `wildfly:run`
 Caso o server não start pelo wildfly:run, estartar manualmente pelos gerenciadores de servers da sua IDE de escolha.

### Com o Banco de dados e o server up:
	- Clear / build do projeto
	- `wildfly:deploy`
	- Run Project (pela ide escolhida)
	
	Ocorrendo tudo bem, você será levado a tela de login:
	Usuario: teste / password:123
	
	Ao Fazer login, estara disponivel o sistema para cadastro, exclusão, edição, execução de procedimentos e um relatorio simples.


Requisitos obrigatórios:
- [x] Utilizar Servlets e JSP para o cadastro e validação dos procedimentos de autorização;
- [x] Entregar a documentação necessária para compilar (colocar no readme do repositório);
- [x] Criar a estrutura de banco de dados proposta para o problema (pode-se utilizar banco de dados em memória – H2), também com instruções no readme;
- [x] Usar git para armazenar o fonte (usar um git publico e enviar a URL);
- [x] Usar o Maven para fazer o build;
 
