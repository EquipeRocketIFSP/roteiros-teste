# roteiros-teste

## Modelo

|Cenário|Caso de teste|Roteiro|Resultado Esperado|Resultado|
|---|---|---|---|---|
|Login de usuário|Login com sucesso|1. Ao acessar a URL de login (<host>:3000/login)|1. Exibir a tela de login||
|Login de usuário|Login com sucesso|1.2 Inserir email: cartvet@gmail.com|1.2 devem existir campos para inserção de email||
|Login de usuário|Login com sucesso|1.3 Inserir codinome: peludos|1.3 codinome da clínica||
|Login de usuário|Login com sucesso|2. Prosseguir e adicionar a senha: 123456|2. direcionar para a página logada||
|Login de usuário|Desistência de login|1. Ao acessar a URL de login (<host>:3000/login)|1. Exibir a tela de login|||
|Login de usuário|Desistência de login|1.2 Inserir email: cartvet@gmail.com|1.2 devem existir campos para inserção de email||
|Login de usuário|Desistência de login|1.3. Inserir codinome: peludos|1.3 codinome da clínica||
|Login de usuário|Desistência de login|2. Selecionar o botão "Cancelar"|2. Ser redirecionado à página de login, sem dados de email ou clínica no formulário de login"||
|Login de usuário|Usuário não cadastrado tentando login|1. Ao acessar a URL de login (<host>:3000/login)|1. carregar a tela de login||
|Login de usuário|Usuário não cadastrado tentando login|1.2 Inserir um email qualquer|1.2 devem existir campos para inserção de email||
|Login de usuário|Usuário não cadastrado tentando login|1.3 Inserir um codinome qualquer|1.3 codinome da clínica||
|Login de usuário|Usuário não cadastrado tentando login|2. Inserir uma senha qualquer|2. Apresentar tela de dados de acesso não puderam ser validados.||
|Login de usuário|Usuário cadastrado realizando reset|1. Ao acessar a URL de login (<host>:3000/login)|1. carregar a tela de login|||
|Login de usuário|Usuário cadastrado realizando reset|1.2 Inserir email: cartvet@gmail.com|1.2 devem existir campos para inserção de email||
|Login de usuário|Usuário cadastrado realizando reset|1.3 Inserir codinome: peludos|1.3 codinome da clínica||
|Login de usuário|Usuário cadastrado realizando reset|2. Selecionar o botão "Esqueci minha senha"|2. Apresentar mensagem: "Instruções encaminhados para o email cadastrado"||
|Login de usuário|Usuário cadastrado realizando reset|2.1 Observar banner com mensagem de envio de email com instruções para reset|2.1 Verificar recebimento de email com instruções para executar o reset.||
|Login de usuário|Usuário cadastrado realizando reset|3. Abrir o link e definir uma nova senha|3. Observar exibição de banner verde com mensagem de alteração de senha com sucesso. A tela será redirecionada para a tela de login. Observar que o banner persiste sendo exibido.||
