# 📌 Feature 2: Dashboard Nutricionista
**Data de entrega:** 06/04/2025

## História de Usuário 1 - Pesquisa (leitura) de pacientes 
> **Como** nutricionista cadastrado na plataforma <br>
> **Quero** pesquisar pelo nome de um paciente no Dashboard <br>
> **Para** localizar rapidamente o paciente e gerenciar suas informações

### Critérios de Aceitação:
1. O nutricionista deve visualizar um campo de pesquisa de pacientes no **Dashboard**.
2. O nutricionista pode inserir o nome completo ou parte dele no campo de pesquisa.
3. Ao realizar a pesquisa, o sistema deve exibir pacientes que possuam o nome exato ou parcial.
4. Se o nome inserido não corresponder a nenhum paciente cadastrado, o sistema deve exibir a mensagem "Nenhum paciente encontrado".
5. O nome de cada paciente listado nos resultados de pesquisa deve ser clicável, redirecionando para a tela de detalhes do paciente.


<br>


## Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Pesquisar paciente com nome exato** 

**Dado** que o nutricionista está no dashboard <br>
**Quando** inserir no campo de pesquisa, o nome exato de um paciente já cadastrado  <br>
**Então** o sistema deve exibir o paciente correspondente na lista de resultados

<br>

✅ **Cenário 2: Pesquisar paciente com nome parcialmente correto** 

**Dado** que o nutricionista está no dashboard <br>
**Quando** inserir no campo de pesquisa, parte do nome de um paciente já cadastrado  <br>
**Então** o sistema deve exibir os pacientes cujos nomes contenham a parte inserida

<br>

❌ **Cenário 3: Pesquisar paciente com nome inexistente**

**Dado** que o nutricionista está no dashboard <br>
**Quando** inserir no campo de pesquisa, o nome incorreto ou com erro de digitação  <br>
**Então** o sistema deve exibir a mensagem "Nenhum paciente encontrado" <br>
**E** não exibir resultados de pacientes

