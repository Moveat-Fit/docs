# 📌 Feature 4: Plano Alimentar | Dashboard Paciente
**Data de entrega:** 08/06/2025

## História de Usuário 2 - Remover plano alimentar de um paciente
> **Como** nutricionista logado na plataforma  
> **Quero** remover um plano alimentar existente  
> **Para** que eu possa atualizar ou excluir informações desnecessárias  

### Critérios de Aceitação:
1. O sistema deve solicitar uma confirmação antes de excluir.
2. Após a remoção, o sistema deve exibir a mensagem "Plano alimentar removido com sucesso!".  

### Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Remover plano alimentar com sucesso**  
**Dado** que o nutricionista está visualizando o plano alimentar de um paciente  
**Quando** clicar em "Remover"  
**E** confirmar a exclusão  
**Então** o sistema deve exibir a mensagem "Plano alimentar removido com sucesso!"  
**E** atualizar a lista de planos do paciente  

❌ **Cenário 2: Cancelar a remoção do plano**  
**Dado** que o nutricionista clicou em "Remover"  
**Quando** cancelar a ação na janela de confirmação  
**Então** o plano não deve ser excluído  
**E** o sistema deve continuar exibindo o plano  

❌ **Cenário 3: Tentar remover plano inexistente**  
**Dado** que o plano alimentar foi excluído em outra sessão  
**Quando** o nutricionista tentar removê-lo novamente  
**Então** o sistema deve exibir a mensagem de erro "Plano não encontrado"  