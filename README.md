# 👋 Opa! Eu sou o Leandro

Sou **Desenvolvedor C# focado em RPA** e automação de processos “de verdade”: robôs que rodam em produção, com **resiliência**, **observabilidade**, **retomada** e **integração** com sistemas web/legados.

Aqui no GitHub eu compartilho ideias, componentes e padrões que uso no dia a dia para criar automações confiáveis — sem expor projetos privados.

---

## 🚀 O que eu construo
- **Robôs Web** com **Selenium WebDriver** (fluxos longos, múltiplas janelas, uploads/downloads, tabelas, navegação dinâmica)
- **Automação híbrida UI + API** (quando API existe, acelera e estabiliza; quando não, a UI resolve)
- **Orquestração** com fila, controle de execução e estados (pendente → executando → sucesso/erro → reprocesso)
- **Evidências** (prints, HTML, logs detalhados, arquivos gerados) para auditoria e suporte
- **Tratamento de falhas e retomada** (retry com backoff, detecção de popups/alertas, validações fortes, timeout controlado)
- **Exportação e transformação de dados** (CSV/planilhas, validação, normalização e pipelines simples)

---

## 🧠 Ferramentas e bibliotecas que eu uso muito
**C# / .NET (Framework e moderno)**  
- `Selenium.WebDriver` + `Selenium.Support`  
- `SeleniumExtras.WaitHelpers` (esperas explícitas e condições)  
- `System.Text.Json` / `Newtonsoft.Json` (integrações e payloads)  
- `HttpClient` (APIs REST com políticas de retry e timeouts)  
- `Microsoft.Extensions.DependencyInjection` (DI)  
- `Microsoft.Extensions.Configuration` (appsettings, variáveis de ambiente)  
- `Serilog` (ou logging equivalente) + logs estruturados por correlação  
- `SqlClient` / procedures (auditoria, execução e trilha operacional)

## 🖥️ Automação Desktop / Legado (FlaUI)
Quando o cenário envolve aplicações **Windows/legadas** (WinForms/WPF e afins) eu uso **FlaUI** para automação via UI Automation, principalmente quando não dá pra resolver tudo por API ou web.

**Como eu aplico na prática:**
- **Attach por processo/janela** (encontrar a janela certa, inclusive quando existem sub-janelas/modal)
- Busca de elementos por **AutomationId/Name/ControlType** e navegação na árvore de automação
- **Sincronização real** (esperas por elemento existir/estar habilitado, evitando “sleep” desnecessário)
- Ações de interação: **click**, **set de texto**, **seleção**, **atalhos de teclado** e fluxos com **popups**
- Tratamento de casos chatos de produção: janela não focada, UI travada, modal inesperado, foco/teclado
- **Evidências** e logs do passo-a-passo para facilitar suporte e auditoria

> Eu gosto do FlaUI porque ele ajuda a levar automação desktop pra um padrão mais “engenharia”: previsível, rastreável e manutenível.

**Quando envolve desktop/legado (dependendo do cenário)**  
- UI Automation / wrappers (ex.: FlaUI) para telas antigas e controles difíceis
- Estratégias de attach por processo/janela, sincronização e ações de teclado

---

## 🧩 Padrões e “lógicas” que eu curto (porque seguram produção)
- **State machine** de execução (cada etapa valida antes de avançar)
- **Retries inteligentes** (não é retry cego: retry com critério, limites e fallback)
- **Esperas explícitas + validações** (menos “Thread.Sleep”, mais previsibilidade)
- **Idempotência** (rodou 2x não quebra nem duplica resultado)
- **Correlação de logs** por execução (um `correlationId` por item/fila)
- **Separação de camadas** (core de negócio ≠ automação de tela ≠ infra)
- **Factory/Strategy** para escolher “qual automação” executar conforme contexto
- **Captura de evidência no erro** (print + estado + último passo + dados do item)

---

## 🧪 Exemplos do que você pode ver por aqui
> Sem repositórios corporativos: foco em componentes reaproveitáveis e provas de conceito.
- helpers de Selenium (Waits, Actions, Selects, download handler)
- wrappers de `HttpClient` com retry/timeouts
- modelos de orquestração (fila + logs + estado)
- exportadores CSV/planilha com validação e normalização
- padrões de logging para RPA (execução auditável)

---

## 🛠️ Stack
**C# | .NET | Selenium | SQL Server | REST APIs | Windows Automation | Git**

---

## 📫 Contato
- LinkedIn: **linkedin.com/in/leandrodayrell**
- E-mail: **leandrodayrellsilva@hotmail.com**

<div align="center">
 <p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=leandrodayrell&theme=chartreuse-dark" alt="leandrodayrell" /></p>

<div style="display: inline_block"><br>
  <img align="center" alt="Leandro-Lua" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/lua/lua-original.svg">
  <img align="center" alt="Leandro-Csharp" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg">
  <img align="center" alt="Leandro-Python" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original-wordmark.svg">
  <img align="center" alt="Leandro-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Leandro-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Leandro-JavaScript" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg">
  <img align="center" alt="Leandro-SqlServer" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/microsoftsqlserver/microsoftsqlserver-plain-wordmark.svg">
  <img align="center" alt="Leandro-NodeJS" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/nodejs/nodejs-original-wordmark.svg">
</div>
  
