# 📌 Feature 4: Plano Alimentar | Dashboard Paciente
**Data de entrega:** 08/06/2025

## História de Usuário 3 - Editar plano alimentar de um paciente
> **Como** nutricionista logado na plataforma  
> **Quero** editar um plano alimentar existente  
> **Para** que eu possa atualizá-lo conforme as necessidades do paciente  

### Critérios de Aceitação:
1. Os mesmos campos obrigatórios da criação devem ser validados.
2. Após a edição, o sistema deve exibir a mensagem "Plano alimentar atualizado com sucesso!" e retornar ao dashboard.

### Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Editar plano alimentar com sucesso**  
**Dado** que o nutricionista está na tela de edição do plano  
**Quando** modificar os dados e clicar em "Salvar"  
**Então** o sistema deve exibir "Plano alimentar atualizado com sucesso!"  
**E** retornar ao dashboard  

❌ **Cenário 2: Tentar salvar plano com campos obrigatórios vazios**  
**Dado** que o nutricionista está editando o plano  
**Quando** apagar campos obrigatórios  
**E** tentar salvar  
**Então** o sistema deve exibir mensagens de erro  
**E** não salvar as alterações  

❌ **Cenário 3: Tentar salvar plano com refeições vazias**  
**Dado** que o nutricionista está editando o plano  
**Quando** remover todas as refeições 
**E** tentar salvar  
**Então** o sistema deve exibir uma mensagem de erro  
**E** não salvar as alterações  

❌ **Cenário 4: Tentar salvar plano sem alimentos em uma refeição**  
**Dado** que o nutricionista está editando o plano  
**Quando** remover todos os alimentos de uma refeição  
**E** tentar salvar  
**Então** o sistema deve exibir uma mensagem de erro  
**E** não salvar as alterações  