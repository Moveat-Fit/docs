# 📌 Feature 1: Acesso à Plataforma
**Data de entrega:** 09/03/2025

## História de Usuário 1 - Cadastro Personal Trainer
> **Como** um novo usuário <br>
> **Quero** me cadastrar na plataforma <br>
> **Para** que eu possa montar a planilha de treino do meu aluno

### Critérios de Aceitação:
1. O personal deve preencher os campos obrigatórios **nome, e-mail, senha e número do CREF (Conselho Regional de Educação Física)** para se cadastrar.
2. O sistema deve validar se o e-mail é único.
3. O sistema deve validar se a senha tem no mínimo 8 caracteres.
4. O sistema deve validar se o número de cadastro no CREF é válido.

<br>

## História de Usuário 2 - Cadastro Nutricionista
> **Como** um novo usuário <br>
> **Quero** me cadastrar na plataforma <br>
> **Para** que eu possa montar o plano alimentar do meu paciente

### Critérios de Aceitação:
1. O nutricionista deve preencher os campos obrigatórios **nome, e-mail, senha e número do CRN (Conselho Regional de Nutrição)** para se cadastrar.
2. O sistema deve validar se o e-mail é único.
3. O sistema deve validar se a senha tem no mínimo 8 caracteres.
4. O sistema deve validar se o número de cadastro no CRN é válido.


<br>


### Cenários de Teste
✅ **Cenário 1: Cadastro com dados válidos** 

**Dado** que o usuário acesse a tela de cadastro <br>
**Quando** preencher os campos obrigatórios <br>
**Então** o sistema deverá criar a conta e redirecionar para o login 

<br>

❌ **Cenário 2: Tentativa de cadastro com e-mail já existente** <br>

**Dado** que já exista uma conta com determinado e-mail <br>
**Quando** o usuário tentar cadastrar com o mesmo e-mail <br>
**Então** o sistema deverá exibir uma mensagem de erro "Este e-mail já está cadastrado" 

<br>

❌ **Cenário 3: Tentativa de cadastro com dados em branco** <br>

**Dado** que o usuário acesse a tela de cadastro <br>
**Quando** preencher os dados <br>
**Mas** deixar de preencher qualquer campo obrigatório <br>
**Então** o sistema deverá exibir uma mensagem de erro "Preencha todos os campos obrigatórios"
