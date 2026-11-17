# AKIN // Portfólio de Engenharia de Software & AI Builder

Portfólio técnico de **Lohan Akin Sampaio Silva** — formado em Jogos Digitais pela UNEB (julho de 2026), Embaixador Estudantil Google e residente em Games pelo CEPEDI.

- **Portfólio Publicado:** [https://akin-portfolio-seven.vercel.app/](https://akin-portfolio-seven.vercel.app/)
- **Demo Interativa ROTAS + PARTS:** [`/rotas-parts.html`](./rotas-parts.html)

---

## Estrutura do Portfólio

1. **Taxonomia Transparente de IA:**
   - Diferenciação explícita entre **Produtos com IA Integrada em Execução** (`Personal Hub` via rota server-side `/api/ai/weekly-plan`, `JARVIS`, `Editor de Vídeo com IA`) e **Projetos Construídos com Apoio de IA no Desenvolvimento** (`ROTAS + PARTS`, `Walkie`).
2. **Projetos Documentados com Evidências e Limitações Reais:**
   - **01 // Personal Hub (Projeto Principal):** Hub financeiro e de agenda com Planejador Semanal com IA, detecção de conflitos, revisão humana antes de salvar e isolamento de `GEMINI_API_KEY` no servidor (diferenciando `LIVE_GEMINI` de `SIMULATED_FALLBACK`).
   - **02 // ROTAS + PARTS (`rotas-parts.html`):** Minijogo e laboratório interativo sobre organização dos estudos (**ROTAS**: Compreender, Experimentar, Investigar, Construir) e engenharia de prompts (**PARTS**: Papel, Ação, Referências, Tom, Saída). Executa 100% no navegador sem chamadas de API de LLM em tempo de execução.
   - **03 // Walkie:** Comunicador PTT em tempo real (PeerJS WebRTC + LiveKit SFU). Documenta com transparência que a transmissão de áudio entre dois aparelhos físicos distintos em redes móveis ainda aguarda bateria de testes de campo.
   - **04 // JARVIS & 05 // Editor de Vídeo com IA:** Protótipos locais em Python documentados com seus estágios reais de desenvolvimento.
3. **Documentação de Automação (`#automacao`):**
   - Fluxo `Entrada de Tarefas → Organização com IA → Revisão Humana → Salvamento na Agenda`, detalhando payload de entrada, contrato JSON de saída, tratamento de erros e justificativa arquitetural (API Route nativa em vez de intermediários externos como n8n/Make).
4. **Evidências, Roteiros de 90s e Benchmark (`#evidencias`):**
   - Roteiros cronometrados de até 90 segundos para os 3 projetos principais.
   - Protocolo de teste comparativo reproduzível (Alocação Manual vs. Fluxo Assistido com Revisão Humana) com registro real de amostra única (`N=1`), sem invenção de usuários ou métricas de produção.

## Como Visualizar Localmente

Por ser construído em HTML5, CSS3 e JavaScript Vanilla sem dependências de bundler, basta abrir `index.html` ou `rotas-parts.html` no navegador ou servir o diretório com qualquer servidor estático:

```bash
npx serve .
```
