# 📌 Feature 1: Acesso à Plataforma
**Data de entrega:** 09/03/2025

## História de Usuário 1 - Login Usuário
> **Como** um usuário cadastrado <br>
> **Quero** logar na plataforma <br>
> **Para** que eu possa acessar minha conta

### Critérios de Aceitação:
1. O sistema deve permitir login com **e-mail e senha** corretos.
2. Se a senha ou e-mail estiverem incorretos, deve exibir uma mensagem de erro.


<br>


### Cenários de Teste
**Contexto:** Usuário já cadastrado na plataforma

✅ **Cenário 1: Login com credenciais válidas** 

**Dado** que o usuário acesse a tela de login <br>
**Quando** preencher e-mail e senha corretamente <br>
**Então** o sistema deverá redirecioná-lo para a página principal

<br>

✅ **Cenário 2: Redefinição de senha bem-sucedida** 

**Dado** que o usuário acesse a tela de login <br>
**E** clique na opção "Esqueci minha senha" <br>
**Quando** preencher um e-mail válido <br>
**Então** o sistema deverá exibir a mensagem "Um link de redefinição de senha foi enviado para o seu e-mail"

<br>

❌ **Cenário 3: Tentativa de redefinição com e-mail não cadastrado** 

**Dado** que o usuário acesse a tela de login <br>
**E** clique na opção "Esqueci minha senha" <br>
**Quando** preencher um e-mail inválido <br>
**Então** o sistema deverá exibir a mensagem "E-mail não encontrado. Verifique e tente novamente"

<br>

❌ **Cenário 4: Tentativa de login com e-mail errado** <br>

**Dado** que o usuário acesse a tela de login <br>
**Quando** preencher uma senha correta <br>
**Mas** um e-mail incorreto <br>
**Então** o sistema deverá exibir uma mensagem de erro "E-mail e/ou senha inválidos." 

<br>

❌ **Cenário 5: Tentativa de login com senha errada** <br>

**Dado** que o usuário acesse a tela de login <br>
**Quando** preencher uma e-mail correto <br>
**Mas** uma senha incorreta <br>
**Então** o sistema deverá exibir uma mensagem de erro "E-mail e/ou senha inválidos." 
