## Validação de API para Marcar/Desmarcar Conteudo como favorito

### Demonstração
Para acessar a demonstração do projeto <a href="https://learningcourse.netlify.app/" target="_blank">Clique aqui</a>

![GitHub Logo](/src/assets/img/thumb_1.jpg)

### Introdução:
Este portfolio apresenta a validação da API para a funcionalidade de marcar/desmarcar um curso como favorito. A validação foi realizada utilizando a ferramenta Postman, permitindo garantir a qualidade e confiabilidade da API antes de sua implementação em produção.

### Objetivo:
O objetivo principal do projeto era verificar se a API funcionava de acordo com os requisitos especificados e atendia às expectativas dos usuários. Para isso, foram criados quatro cenários de teste que abrangem as principais funcionalidades da API:
Cenários de Teste

1. Favoritar um Curso:
Objetivo: Testar se a API consegue marcar um curso como favorito para um usuário que ainda não o tenha favoritado.
Passo a Passo:
Entrada:
•	Informe o ID do curso que você deseja favoritar.
•	Informe o ID do usuário.
Saída Esperada:
•	A API retorna o código de status 200 OK, indicando que o curso foi favoritado com sucesso.
•	Uma mensagem de sucesso é exibida, confirmando que o curso foi favoritado.

2. Favoritar um Curso Já Favoritado:
Objetivo: Testar se a API retorna um erro ao tentar favoritar um curso que já está favoritado.
Passo a Passo:
Entrada:
•	Informe o ID do curso que você deseja favoritar (que já está favoritado).
•	Insira o token de autenticação da sua conta (que já tenha favoritado o curso).
Saída Esperada:
•	A API retorna o código de status 400 Bad Request, indicando que a requisição é inválida.
•	Uma mensagem de erro é exibida, informando que o curso já está favoritado.

3. Desfavoritar um Curso Favoritado:
Objetivo: Testar se a API consegue desmarcar um curso como favorito para um usuário que o tenha favoritado.
Passo a Passo:
Entrada:
•	Informe o ID do curso que você deseja desfavoritar (que está favoritado).
•	Insira o token de autenticação da sua conta (que tenha favoritado o curso).
Saída Esperada:
•	A API retorna o código de status 200 OK, indicando que o curso foi desfavoritado com sucesso.
•	Uma mensagem de sucesso é exibida, confirmando que o curso foi desfavoritado.

4. Desfavoritar um Curso Não Favoritado:
Objetivo: Testar se a API retorna um erro ao tentar desfavoritar um curso que não está favoritado.
Passo a Passo:
Entrada:
•	Informe o ID do curso que você deseja desfavoritar (que não está favoritado).
•	Insira o token de autenticação da sua conta (que não tenha favoritado o curso).
Saída Esperada:
•	A API retorna o código de status 400 Bad Request, indicando que a requisição é inválida.
•	Uma mensagem de erro é exibida, informando que o curso não está favoritado.

5. Favoritar uma Trilha:
Objetivo: Testar se a API consegue marcar uma trilha como favorita para um usuário que ainda não a tenha favoritado.
Passo a Passo:
Entrada:
•	Informe o ID da trilha que você deseja favoritar.
•	Informe o ID do usuário.
Saída Esperada:
•	A API retorna o código de status 200 OK, indicando que a trilha foi favoritada com sucesso.
•	Uma mensagem de sucesso é exibida, confirmando que a trilha foi favoritada.

6. Favoritar uma Trilha Já Favoritada:
Objetivo: Testar se a API retorna um erro ao tentar favoritar um trilha que já está favoritada.
Passo a Passo:
Entrada:
•	Informe o ID do trilha que você deseja favoritar (que já está favoritado).
•	Informe o ID do usuário.
Saída Esperada:
•	A API retorna o código de status 400 Bad Request, indicando que a requisição é inválida.
•	Uma mensagem de erro é exibida, informando que a trilha já está favoritada.

7. Desfavoritar uma Trilha Favoritada:
Objetivo: Testar se a API consegue desmarcar uma trilha como favorita para um usuário que a tenha favoritada.
Passo a Passo:
Entrada:
•	Informe o ID da trilha que você deseja desfavoritar (que está favoritado).
•	Informe o ID do usuário.
Saída Esperada:
•	A API retorna o código de status 200 OK, indicando que a trilha foi desfavoritada com sucesso.
•	Uma mensagem de sucesso é exibida, confirmando que a trilha foi desfavoritada.

8. Desfavoritar uma Trilha Não Favoritada:
Objetivo: Testar se a API retorna um erro ao tentar desfavoritar uma trilha que não está favoritado.
Passo a Passo:
Entrada:
•	Informe o ID da trilha que você deseja desfavoritar (que não está favoritado).
•	Informe o ID do usuário.
Saída Esperada:
•	A API retorna o código de status 400 Bad Request, indicando que a requisição é inválida.
•	Uma mensagem de erro é exibida, informando que o trilha não está favoritado.

### Resultados:
Todos os cenários de teste foram executados com sucesso, confirmando que a API funciona de acordo com os requisitos especificados. A validação identificou alguns pontos de melhoria, como a necessidade de mensagens de erro mais específicas, que foram documentados para posterior correção
