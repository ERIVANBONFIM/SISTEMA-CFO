# SISTEMA-CFO
SISTEMA PARA FAZER ANALISE FINANCEIRA DA EMPRESA
# SISTEMA CFO

Dashboard de análise financeira para diretoria, com integração ao IXC Soft.

## Objetivo
Consolidar dados financeiros do provedor (clientes, contratos, contas a 
receber, recebimentos, inadimplência) em um painel visual que ajude a 
diretoria a tomar decisões.

## Stack
- Next.js 14 (App Router) + TypeScript
- Tailwind CSS + shadcn/ui
- Recharts (gráficos)
- Supabase (PostgreSQL)
- Integração com IXC Soft via webservice REST
- Deploy na Vercel

## KPIs do dashboard
- MRR (Monthly Recurring Revenue)
- Inadimplência total e por aging (30/60/90/120+ dias)
- Churn financeiro mensal
- Ticket médio
- Top 20 devedores
- Receita prevista vs realizada
- Recuperação de dívida (cobrança antiga recebida no mês)
- Aging de contas a receber

## Estrutura planejada
- `/app` — rotas do Next.js (páginas e API routes)
- `/components` — componentes reutilizáveis (cards de KPI, gráficos, tabelas)
- `/lib/ixc` — cliente da API do IXC e funções de busca
- `/lib/db` — acesso ao Supabase
- `/lib/kpis` — cálculo dos indicadores
- `/types` — tipos TypeScript dos dados do IXC

## Variáveis de ambiente
Veja `.env.example`. Nunca commite o `.env.local`.

## Status
Em construção.
