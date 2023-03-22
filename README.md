# roteiros-teste

## Modelo

|Cenário|Caso de teste|Roteiro|Resultado Esperado|Resultado|
|---|---|---|---|---|
|Login de usuário|Login com sucesso|1. Acessar a URL de login (<host>:3000/login)|1. Exibir a tela de login||
|Login de usuário|Login com sucesso|2. Inserir email cadastrado|2. Campo para preenchimento do e-mail do usuário é mostrado||
|Login de usuário|Login com sucesso|3. Inserir codinome da clínica no qual há intenção de logar|3. Campo para preenchimento do codinome da clínica no qual se deseja logar é mostrado||
|Login de usuário|Login com sucesso|4. Colocar a senha de acesso|4. Campo para preenchimento da senha do usuário é mostrado||
|Login de usuário|Login com sucesso|5. Pressionar o botão "Login"|5. Requisição ao banco de dados com a validação das informações preenchidas e, se tudo estiver correto, o usuário terá conseguido realizar com sucesso seu login e acessará o sistema||
|Login de usuário|Usuário não cadastrado tentando login|1. Acessar a URL de login (<host>:3000/login)|1. Exibir a tela de login|||
|Login de usuário|Usuário não cadastrado tentando login|2. Inserir email cadastrado|2. Campo para preenchimento do e-mail do usuário é mostrado||
|Login de usuário|Usuário não cadastrado tentando login|3. Inserir codinome da clínica no qual há intenção de logar|3. Campo para preenchimento do codinome da clínica no qual se deseja logar é mostrado||
|Login de usuário|Usuário não cadastrado tentando login|4. Colocar alguma possível senha de acesso|4. Campo para preenchimento da senha do usuário é mostrado||
|Login de usuário|Usuário não cadastrado tentando login|5. Pressionar o botão "Login"|5. Requisição ao banco de dados com a validação das informações preenchidas e, visto a inexistência do usuário no banco de dados, aparecerá uma mensagem logo acima dos campos de preenchimento com a mensagem "Este e-mail não tem uma conta"||
|Login de usuário|Usuário tentando logar com codinome ou senha inválida|1. Acessar a URL de login (<host>:3000/login)|1. Exibir a tela de login||
|Login de usuário|Usuário tentando logar com codinome ou senha inválida|2. Inserir email cadastrado|2. Campo para preenchimento do e-mail do usuário é mostrado||
|Login de usuário|Usuário tentando logar com codinome ou senha inválida|3. Inserir codinome da clínica no qual há intenção de logar|3. Campo para preenchimento do codinome da clínica no qual se deseja logar é mostrado||
|Login de usuário|Usuário tentando logar com codinome ou senha inválida|4. Colocar a senha de acesso|4. Campo para preenchimento da senha do usuário é mostrado||
|Login de usuário|Usuário tentando logar com codinome ou senha inválida|5. Pressionar o botão "Login"|5. Requisição ao banco de dados com a validação das informações preenchidas e, visto que o codinome ou a senha está errada, então o usuário receberá uma mensagem logo em cima do campo de e-mail dizendo "O codinome ou a senha está errada" e o login não será feito||
|Login de usuário|Usuário cadastrado realizando reset da senha|1. Acessar a URL de login (<host>:3000/login)|1. Carregar a tela de login|||
|Login de usuário|Usuário cadastrado realizando reset da senha|2. Clicar no botão que fica logo abaixo do campo de senha "Redefinir minha senha"|2. Requisição será feita para ir para outra página onde se iniciará o processo de redefinição da senha||
|Login de usuário|Usuário cadastrado realizando reset da senha|3. Esperar a página de redefinir a senha ser carregada|3. Página inicial de redefinição de senha carregada||
|Login de usuário|Usuário cadastrado realizando reset da senha|4. Preencher o e-mail cadastrado no campo de e-mail que aparecerá|4. O sistema aqui esperará o cliente preencher o e-mail||
|Login de usuário|Usuário cadastrado realizando reset da senha|5. Clicar no botão "Próximo"|5. Requisição feita nesse momento irá primeiro verificar no banco de dados a existência de um usuário com esse login e, caso haja, enviará um e-mail a este usuário para dar continuidade ao processo de redefinição de senha||
|Login de usuário|Usuário cadastrado realizando reset da senha|6. Entrar no e-mail dele e clicar no botão de "Mudar a senha" no e-mail que foi enviado a ele|6. Quando o cliente clicar em "Mudar a senha", será feito uma requisição para abrir uma página de redefinição de senha||
|Login de usuário|Usuário cadastrado realizando reset da senha|7. Esperar a tela de mudança de senha ser exibida|7. Sistema carrega a página||
|Login de usuário|Usuário cadastrado realizando reset da senha|8. Inserir a senha de interesse|8. Aguarda o usuário colocar uma senha||
|Login de usuário|Usuário cadastrado realizando reset da senha|9. Clicar em salvar|9. Realiza uma atualização na senha daquele usuário||