# 📌 Feature 3: Dashboard Nutricionista II
**Data de entrega:** 04/05/2025

## História de Usuário 1 - Deletar paciente
> **Como** nutricionista cadastrado na plataforma  
> **Quero** deletar um paciente da minha lista  
> **Para** que eu possa manter meu dashboard organizado e com pacientes ativos  

### Critérios de Aceitação:
1. O nutricionista deve visualizar um botão para deletar um paciente.
2. Ao clicar, o sistema deve exibir uma mensagem de confirmação: "Tem certeza que deseja deletar este paciente?" com opções "Sim" e "Cancelar".
3. Caso confirme, o paciente deve ser removido da lista e a mensagem "Paciente deletado com sucesso!" deve ser exibida.
4. Caso cancele, nenhuma ação deve ser realizada.

## Cenários de Teste
**Contexto:** Nutricionista logado na plataforma

✅ **Cenário 1: Deletar paciente com sucesso**  
**Dado** que o nutricionista está no dashboard  
**Quando** clicar em "Deletar" na linha de um paciente  
**E** confirmar a ação na mensagem de confirmação  
**Então** o sistema deve exibir a mensagem "Paciente deletado com sucesso!"  
**E** remover o paciente da lista  

❌ **Cenário 2: Cancelar exclusão de paciente**  
**Dado** que o nutricionista clicou em "Deletar"  
**Quando** clicar em "Cancelar" na mensagem de confirmação  
**Então** o sistema deve manter o paciente na lista  
**E** não exibir nenhuma mensagem de sucesso
