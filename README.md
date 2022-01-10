# SistemaDePonto
O projeto consiste em um sistema com 02 perfis, funcionário e administrador.<br/>
<br/>
No perfíl de funcionário, ao efetuar o login, este usuário poderá realizar sua marcação de ponto onde será capturada sua GeoLocalização. Além da tela de lançamento dos horários de início de trabalho/almoço e término de trabalho/almoço, este perfíl possui acesso à um relatório com suas marcações.<br/>
<br/>
Já no perfíl de administrador do sistema, será apresentado um relatório de todas as marcações de todos os funcionário que estão sobre o guarda-chuva de sua empresa, assim como a possibilidade de edição, em caso de alguma marcação incorreta.

### Pontos importantes sobre o projeto:
* O projeto foi desenvolvido utilizando o Angular Material;
* Trabalhamos com decode do Base64;
* Para as datas/horas foi utilizada a API [Moment.js](https://momentjs.com/docs/);
* Foram criadas mascaras personalizadas para CPF e CNPJ;
* Foram criados validadores personalizados para CPF e CNPJ;
* Trabalhamos com GeoLocalização junto ao registro das marcações;
* Trabalhamos com paginação e ordenação nos relatórios de lançamento;
* Utilizamos pipes para uma melhor visualização das datas/horas e tipos de lançamento.

__________________________________________________________________________________________________________

### Angular CLI - version 13.0.0
Esse projeto foi desenvolvido em Angular, portanto para execução realize os seguintes passos:

1. Faça o clone do repositório para sua máquina;
* `git clone url-projeto`
3. Utilizando o prompt de comando, navegue até a pasta do projeto;
* `cd caminho-da-pasta`
5. Ainda no prompt de comando e já dentro da pasta do projeto, você precisará instalar todas as dependências do package.json, sendo assim execute o seguinte comando:
* `npm install`
6. Após finalização da instalação, ainda no prompt de comando, execute:
* `ng serve`
7. O projeto será executado em `http://localhost:4200/`

________________________________________________________________________________________________________________

### API utilizada no projeto
A API utilizada no projeto encontra-se [aqui](https://github.com/m4rciosouza/ponto-inteligente-api-curso-angular-v2) e foi desenvolvida com Java e Spring Boot. Para execução do projeto, a API precisa estar rodando junto ao projeto, conforme segue:

1. Realize o clone do repositório para sua máquina;
* `git clone url-api`
3. Utilizando prompt de comando, navegue até a pasta da API;
* `cd caminho-da-pasta`
5. Ainda no prompt de comando, digite:
* `mvnw spring-boot:run` (caso esteja executando no windows) ou
* `./mvnw spring-boot:run` (nos demais sistemas operacionais);
6. A API será executada em `http://localhost:8080`
