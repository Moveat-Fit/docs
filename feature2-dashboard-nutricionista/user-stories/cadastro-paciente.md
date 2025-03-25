# 📌 Feature 2: Dashboard Nutricionista
**Data de entrega:** 06/04/2025

## História de Usuário 1 - Cadastro de pacientes 
> **Como** nutricionista cadastrado na plataforma <br>
> **Quero** cadastrar um novo paciente preenchendo um formulário com suas informações <br>
> **Para** que eu possa visualizar, gerenciar e futuramente criar um plano alimentar para ele

### Critérios de Aceitação:
1. O nutricionista deve visualizar um formulário com campos obrigatórios (nome, data de nascimento, gênero, peso, altura, CPF, telefone e e-mail).
2. O CPF deve ser único e com formato correto; o e-mail deve ter um formato correto.
3. Ao cadastrar um paciente com sucesso, o sistema deve redirecionar para o **Dashboard** e exibir a mensagem "Paciente cadastrado!".


<br>


## Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Cadastrar paciente com sucesso** 

**Dado** que o nutricionista está no dashboard <br>
**Quando** clicar em "Cadastrar paciente" <br>
**E** preencher todos os campos obrigatórios corretamente <br>
**Então** o sistema deve exibir a mensagem "Paciente cadastrado!" <br>
**E** redirecionar para o Dashboard <br>
**E** exibir o paciente na lista de pacientes

<br>

❌ **Cenário 2: Tentar cadastrar paciente com CPF inválido** 

**Dado** que o nutricionista está na tela de cadastro de paciente <br>
**Quando** inserir um CPF inválido <br>
**Então** o sistema deve exibir a mensagem de erro "CPF inválido" <br>
**E** não cadastrar o paciente

<br>

❌ **Cenário 3: Tentar cadastrar paciente com e-mail inválido**

**Dado** que o nutricionista está na tela de cadastro do paciente <br>
**Quando** inserir um e-mail inválido <br>
**Então** o sistema deve exibir a mensagem de erro "E-mail inválido" <br>
**E** não cadastrar o paciente

<br>

❌ **Cenário 4: Tentar cadastrar paciente com campos obrigatórios vazios** <br>

**Dado** que o nutricionista está na tela de cadastro do paciente <br>
**Quando** deixar um ou mais campos obrigatórios vazios <br>
**Então** o sistema deve exibir uma mensagem de erro indicando os campos obrigatórios
