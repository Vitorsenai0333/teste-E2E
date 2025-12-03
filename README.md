TESTE DE FORMULÁRIO-README
Este projeto contém uma suíte de testes automatizados para validar o funcionamento do formulário de denúncias da aplicação Fire Alert. Os testes foram escritos em Cypress e garantem que o fluxo de denúncia funcione corretamente em diferentes cenários.
Validações implementadas:
1.	Campos obrigatórios:
Envia o formulário vazio e espera o alerta de “Por favor, preencha todos os campos!”.
Garante que não seja possível enviar o formulário sem preencher.
2.	Upload de imagem gera pré-visualização:
Faz um envio de imagem fake.
Verifica se aparece preview e confirma que o sistema mostra a pré-visualização da imagem.
3.	Envio com sucesso:
Vai preencher os campos obrigatórios, enviar o formulário e espera o alerta de sucesso no envio.
Após o envio, os campos e o preview ficam limpos e garante que o envio funciona e reseta o formulário.
4.	Upload de arquivo invalido:
Faz um upload de um arquivo texto “.txt”, verifica se aparece mensagem de erro de “arquivo inválido”.
Garante que apenas imagens sejam aceitas.
5.	Reset limpa preview:
Faz o upload de uma imagem e cria um pré visualização, preenche os campos obrigatórios e envia, espera o alerta de sucesso e confere que o preview foi apagado.
Mostra o sistema limpando tudo após envio.
6.	Navegação:
Verifica se existe o link está visível na interface.

TESTE DE CADASTRO-README
1.	Campos obrigatórios
Envia um formulário vazio, espera um alerta dizendo para preencher os campos e vai garantir que não seja possível fazer o cadastro sem o preenchimento dos dados.
2.	Senhas diferentes
Preenche os campos de nome, e-mail e senha, mas coloca uma confirmação de senha diferente, e espera um alerta de que as senham não coincidem.
Assim confirmando que o sistema bloqueia senhas divergentes.
3.	Senha fraca
     Preenche os campos com uma senha simples como “12345”, espera a mensagem de senha fraca, assim garantindo que o sistema não permita senhas fracas.
4.	E-mail inválido
Preenche os campos os campos com um e-mail sem “@” e domínio e espera um alerta de e-mail invalido, assim confirmando que o sistema valida corretamente o formato do e-mail.
5.	Cadastro bem sucedido 
Preenche todos os campos corretamente, e espera um alerta de confirmação de usuário com sucesso, após o cadastro, a pagina redireciona para o tela de login e garante que o fluxo de cadastro funcione corretamente








