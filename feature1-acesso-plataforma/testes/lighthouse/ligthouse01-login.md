# Relatório Lighthouse: Página Login

## 1. Objetivo
Avaliar a aplicação utilizando a ferramenta Lighthouse para identificar problemas relacionados à desempenho, acessibilidade, melhores práticas e SEO (Search Engine Optimization).

## 2. Ambiente
- URL: [Moveat - Login](https://frontend-production-fdf3.up.railway.app/login)
- Navegador: Google Chrome (versão 133.0.6943.142)
- Sistema Operacional: Windows 11 Pro
- Data do teste: 04/03/2025

## 3. Resultados
| Categoria            | Pontuação | Observações                                |
|----------------------|-----------|--------------------------------------------|
| Desempenho           | 99%       | Página demora para ser renderizada; Imagem grande carrega lentamente          |
| Acessibilidade       | 81%       | Contraste, etiquetas/nomes e localização   |
| Melhores Práticas    | 100%      | -                                          |
| SEO                  | 82%       | Título e metadescrição                     |


---

## 4. Melhorias Encontradas
| ID da Melhoria       | Categoria            | Descrição                                                                                                  | Prioridade | Status |
|----------------------|----------------------|------------------------------------------------------------------------------------------------------------|------------|--------|
| [LIG-LOGIN-001](https://github.com/orgs/Moveat-Fit/projects/4?pane=issue&itemId=100370603&issue=Moveat-Fit%7Cfrontend%7C8) | Desempenho           | Recurso Google Fonts faz com que a página demore para ser renderizada; Imagem com atributo ``loading="lazy"`` atrasa a renderização da página  | Baixa      | Aberto |
| [LIG-LOGIN-002](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100374859&issue=Moveat-Fit%7Cfrontend%7C9)   | Desempenho   | JavaScript não utilizado (é carregado e executado, mas não é necessário para renderização naquele momento) | Baixa      | Aberto |
| [LIG-LOGIN-003](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100379765&issue=Moveat-Fit%7Cfrontend%7C10)  | Acessibilidade       | Cores com taxa de contraste insuficiente | Alta       | Aberto |
| [LIG-LOGIN-004](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100381181&issue=Moveat-Fit%7Cfrontend%7C11) | Acessibilidade e SEO | Documento sem elemento ``<title>``    | Alta       | Aberto |
| [LIG-LOGIN-005](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100382222&issue=Moveat-Fit%7Cfrontend%7C12) | Acessibilidade       | Logo do Google com atributo ``alt`` redundante (pode ser confuso para leitores de tela)  | Baixa      | Aberto |
| [LIG-LOGIN-006](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100383681&issue=Moveat-Fit%7Cfrontend%7C13) | Acessibilidade       | Elemento ``<html>`` sem atributo ``[lang]`` | Média      | Aberto |
| [LIG-LOGIN-007](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100385623&issue=Moveat-Fit%7Cfrontend%7C14) | Acessibilidade       | Áreas de toque não têm espaçamento suficiente                                                                | Média      | Aberto |
| [LIG-LOGIN-008](https://github.com/orgs/Moveat-Fit/projects/4/views/1?pane=issue&itemId=100386819&issue=Moveat-Fit%7Cfrontend%7C15) | SEO          | Documento não tem metadescrição   | Baixa      | Aberto |

---

## 5. Links Úteis
[Relatório gerado pelo Google Lighthouse](https://pagespeed.web.dev/analysis/https-frontend-production-fdf3-up-railway-app-login/tixklrbl1d?form_factor=desktop&category=performance&category=accessibility&category=best-practices&category=seo&hl=pt&utm_source=lh-chrome-ext)
