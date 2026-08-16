# Dashboard de Prospecção

Painel pessoal de prospecção e financeiro para venda de sites a clínicas e
consultórios de saúde/estética. Arquivo único (`dashboard-prospeccao.html`) —
abre direto no navegador, sem servidor, sem instalação, funciona offline.

## Como usar

1. Abra `dashboard-prospeccao.html` com dois cliques.
2. Digite o código de liberação.
3. Importe a planilha de leads (`.xlsx`, aba `Leads`) pelo botão **Importar planilha**.
4. Os dados ficam salvos no `localStorage` do navegador. Faça **Exportar JSON**
   regularmente como backup (em Ajustes).

## O que ele faz

- **Funil de follow-up** com régua automática (2 / 5 / 10 dias, configurável):
  mostra quem contatar hoje, ordenado pelo mais atrasado.
- **Envio via WhatsApp**: abre a conversa com a mensagem certa já preenchida.
  Nada é enviado automaticamente — você confirma cada envio.
- **Financeiro**: contratos por cliente (criação à vista/parcelada e/ou
  mensalidade), cobranças com vencimento, recebido/a receber/atrasado, MRR e
  gráfico de faturamento. Cobrança por links de pagamento (Asaas) colados em
  Ajustes — sem chave de API no arquivo.
- **Bloqueio por código** na abertura.

## Dados

A planilha de leads e os backups **não são versionados** (ver `.gitignore`) —
contêm telefones e dados de terceiros. O repositório carrega só o aplicativo.
