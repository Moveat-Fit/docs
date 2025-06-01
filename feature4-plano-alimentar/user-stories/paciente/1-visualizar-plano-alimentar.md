# 📌 Feature 4: Plano Alimentar | Dashboard Paciente
**Data de entrega:** 08/06/2025

## História de Usuário 1 - Visualizar plano alimentar
> **Como** paciente cadastrado na plataforma  
> **Quero** visualizar meu plano alimentar  
> **Para** que eu possa seguir as orientações do nutricionista  

### Critérios de Aceitação:
1. O plano deve estar visível apenas para o paciente associado.
2. O paciente não pode editar o plano, apenas visualizar.

### Cenários de Teste
**Contexto:** Paciente logado na plataforma

✅ **Cenário 1: Visualizar plano alimentar com sucesso**  
**Dado** que o paciente está logado  
**Quando** acessar a aba "Plano Alimentar"  
**Então** o sistema deve exibir o plano criado pelo nutricionista  

❌ **Cenário 2: Paciente tenta editar o plano**  
**Dado** que o paciente está visualizando o plano  
**Quando** tenta modificar algum campo  
**Então** o sistema não deve permitir a edição  
**E** os campos devem estar desabilitados  

❌ **Cenário 3: Paciente sem plano tenta acessar a aba**  
**Dado** que o paciente não tem plano alimentar cadastrado  
**Quando** acessar a aba "Plano Alimentar"  
**Então** o sistema deve exibir a mensagem "Nenhum plano alimentar disponível"  