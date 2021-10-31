## 💻 Sobre o desafio

<div align='center'>
    <h1>Desafio 02 - Trabalhando com middlewares</h1>
    <p>Esse é o segundo desafio da trilha de NodeJS do bootcamp Ignite da Rocketseat, nele vamos colocar os conhecimentos sobre middlewares.</p>
</div>

### 🧪 Tecnologias

- NodeJs (https://nodejs.org/)
- Express (https://expressjs.com/)
- Uuidv4 (https://www.npmjs.com/package/uuidv4)

### 🛠 Testes

- **Should be able to put user and todo in request when both exits**

  Para que esse teste passe, o middleware **checksTodoExists** deve receber o `username` de dentro do header e o `id` de um _todo_ de dentro de `request.params`. Você deve validar que o usuário exista, validar que o `id` seja um uuid e também validar que esse `id` pertence a um _todo_ do usuário informado.

  Com todas as validações passando, o _todo_ encontrado deve ser passado para o `request` assim como o usuário encontrado também e a função next deve ser chamada.

  É importante que você coloque dentro de `request.user` o usuário encontrado e dentro de `request.todo` o _todo_ encontrado.

- **Should not be able to put user and todo in request when user does not exists**

  Para que esse teste passe, no middleware **checksTodoExists** você deve retornar uma resposta com status `404` caso não exista um usuário com o `username` passado pelo header da requisição.

- **Should not be able to put user and todo in request when todo id is not uuid**

  Para que esse teste passe, no middleware **checksTodoExists** você deve retornar uma resposta com status `400` caso o `id` do _todo_ passado pelos parâmetros da requisição não seja um UUID válido (por exemplo `1234abcd`).

  - **Should not be able to put user and todo in request when todo does not exists**

  Para que esse teste passe, no middleware **checksTodoExists** você deve retornar uma resposta com status `404` caso o `id` do _todo_ passado pelos parâmetros da requisição não pertença a nenhum _todo_ do usuário encontrado.

  - **Should be able to find user by id route param and pass it to request.user**

  Para que esse teste passe, o middleware **findUserById** deve receber o `id` de um usuário de dentro do `request.params`. Você deve validar que o usuário exista, repassar ele para `request.user` e retornar a chamada da função next.

  - **Should not be able to pass user to request.user when it does not exists**

  Para que esse teste passe, no middleware **findUserById** você deve retornar uma resposta com status `404` caso o `id` do usuário \*\*passado pelos parâmetros da requisição não pertença a nenhum usuário cadastrado.

### 🚀 Meus Contatos

<h4>LinkedIn: <a href="https://www.linkedin.com/in/lbandeira/">www.linkedin.com/in/lbandeira/</a></h4>
<h4>Facebook: <a href="https://www.facebook.com/luiz.guilherme.58367/">https://www.facebook.com/luiz.guilherme.58367/</a></h4>
<h4>E-mail: <a href="mailto://arkanael@gmailcom/">arkanael@gmail.com</a></h4>
<h4>Currículo: <a href="https://arkanael.github.io/curriculo/">https://arkanael.github.io/curriculo/</a></h4>
<h4 align=center>Desenvolvido por Luiz Guilherme Bandeira</h4>
