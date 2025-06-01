# 📌 Feature 4: Plano Alimentar | Dashboard Paciente
**Data de entrega:** 08/06/2025

## História de Usuário 1 - Criar plano alimentar de um paciente
> **Como** nutricionista logado na plataforma  
> **Quero** criar um plano alimentar para um paciente já cadastrado  
> **Para** que ele possa seguir uma alimentação personalizada  

### Critérios de Aceitação:
1. Todos os campos obrigatórios devem ser preenchidos, exceto o campo de observações.
2. O plano deve estar vinculado ao paciente correto.
3. Após o cadastro, o sistema deve exibir a mensagem "Plano alimentar criado com sucesso!" e retornar ao dashboard.

### Cenários de Teste
**Contexto:** Nutricionista logado na plataforma e paciente cadastrado

✅ **Cenário 1: Criar plano alimentar com sucesso**  
**Dado** que o nutricionista está na página de criação de plano  
**Quando** preencher todos os campos obrigatórios  
**E** clicar em "Salvar"  
**Então** o sistema deve exibir a mensagem "Plano alimentar criado com sucesso!"  
**E** redirecionar ao dashboard do nutricionista  

❌ **Cenário 2: Tentar criar plano sem preencher campos obrigatórios**  
**Dado** que o nutricionista está criando o plano alimentar  
**Quando** deixar campos obrigatórios em branco  
**E** tentar salvar  
**Então** o sistema deve exibir mensagens de erro indicando os campos obrigatórios não preenchidos  
**E** não deve criar o plano  

❌ **Cenário 3: Tentar criar plano sem adicionar refeições**  
**Dado** que o nutricionista está criando o plano alimentar  
**Quando** não adicionar nenhuma refeição   
**E** tentar salvar  
**Então** o sistema deve exibir uma mensagem de erro  
**E** não deve criar o plano  

❌ **Cenário 4: Tentar criar plano sem adicionar os alimentos**  
**Dado** que o nutricionista está criando o plano alimentar  
**Quando** não adicionar nenhum alimento em uma refeição     
**E** tentar salvar  
**Então** o sistema deve exibir uma mensagem de erro  
**E** não deve criar o plano  