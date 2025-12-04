Testes Automatizados – Fire Alert (Cypress)

Este projeto reúne testes end-to-end feitos com Cypress para validar os formulários de Cadastro e Denúncia da aplicação Fire Alert.

Instalação do Cypress

Pré-requisitos

Node.js instalado

Projeto já configurado com pastas do front-end

 O passo a passo

bash
# Inicializar o projeto
npm init -y

# Instalar o Cypress
npm install cypress --save-dev

# Abrir o Cypress pela primeira vez
npx cypress open

# Executar testes em modo headless
npx cypress run
Os testes devem ser criados dentro da pasta:
Código
cypress/e2e/

📘 Testes de Cadastro

Validações implementadas:

Campos obrigatórios → alerta “Preencha todos os campos!”

Senhas diferentes → alerta “As senhas não coincidem!”

Senha fraca → alerta “Senha fraca!”

E-mail inválido → alerta “E-mail inválido!”

Cadastro bem-sucedido → alerta de sucesso e redirecionamento para login.html

📘 Testes de Denúncia

Validações implementadas:

Campos obrigatórios → alerta “Por favor, preencha todos os campos!”

Upload com pré-visualização → imagem aparece corretamente

Envio com sucesso → alerta de sucesso, limpa campos e preview

Upload inválido → envio de .txt mostra “Arquivo inválido”

Reset → preview removido após envio

Navegação → link Denúncia presente na interface
