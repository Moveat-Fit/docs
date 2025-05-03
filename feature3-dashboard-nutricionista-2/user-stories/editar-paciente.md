# 📌 Feature 3: Dashboard Nutricionista II
**Data de entrega:** 04/05/2025

## História de Usuário 1 - Alterar dados cadastrais do paciente
> **Como** nutricionista cadastrado na plataforma  
> **Quero** editar as informações de um paciente  
> **Para** que eu possa manter os dados sempre atualizados  

### Critérios de Aceitação:
1. O nutricionista deve poder acessar os dados de um paciente e editá-los.
2. Os mesmos campos obrigatórios do cadastro devem ser validados.
3. Após a edição bem-sucedida, o sistema deve exibir a mensagem "Paciente atualizado com sucesso!" e retornar ao Dashboard.

## Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Atualizar informações de paciente com sucesso**  
**Dado** que o nutricionista está no dashboard  
**Quando** clicar em "Editar"  
**E** alterar os dados
**E** salvar as alterações  
**Então** o sistema deve exibir a mensagem "Paciente atualizado com sucesso!"  
**E** redirecionar para o Dashboard com os dados atualizados

❌ **Cenário 2: Tentar salvar dados com e-mail inválido**  
**Dado** que o nutricionista está editando os dados do paciente  
**Quando** inserir um e-mail inválido  
**E** tentar salvar  
**Então** o sistema deve exibir a mensagem de erro "E-mail inválido"  
**E** não salvar as alterações

❌ **Cenário 3: Tentar salvar dados com e-mail já cadastrado**  
**Dado** que o nutricionista está editando os dados do paciente  
**Quando** inserir um e-mail que já está em uso por outro paciente  
**E** tentar salvar  
**Então** o sistema deve exibir a mensagem de erro "E-mail já cadastrado"  
**E** não salvar as alterações  

❌ **Cenário 4: Tentar deixar campos obrigatórios vazios na edição**  
**Dado** que o nutricionista está editando os dados do paciente  
**Quando** não preencher um ou mais campos obrigatórios  
**Então** o sistema deve exibir mensagens de erro indicando os campos obrigatórios  
**E** não salvar as alterações
