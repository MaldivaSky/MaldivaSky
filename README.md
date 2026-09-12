<div align="center">

<img src="https://avatars.githubusercontent.com/u/60511607?v=4" width="120" style="border-radius:50%" alt="Rafael Maldivas" />

# Rafael Paiva Dias da Silva

### Engenheiro de Software Fullstack · Dados & BI

**Transformo problema real de negócio em software que roda em produção.**

Fullstack (Python · TypeScript · React) com mais de 10 anos de bagagem em vendas e
inteligência de mercado. Uno engenharia, dados e leitura de negócio — software que
gera decisão, não só tela.

[![Portfólio](https://img.shields.io/badge/Portfólio-rafael--maldivas.vercel.app-6D28D9?style=for-the-badge&logo=vercel&logoColor=white)](https://rafael-maldivas.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rafael_Paiva_Dias-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-paiva-dias/)
[![E-mail](https://img.shields.io/badge/E--mail-rafaelmaldivas@gmail.com-C9A84C?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rafaelmaldivas@gmail.com)

</div>

---

## Sobre

Sou **Rafael Maldivas**, formado em Análise e Desenvolvimento de Sistemas (IFSP).
Construo **plataformas SaaS multi-tenant, ERPs com emissão fiscal e aplicações de dados
— em produção**.

Antes de escrever a primeira linha, entendo o problema: o fluxo do negócio, o que trava
o cliente, onde o dinheiro vaza. Depois entrego a solução certa — sem over-engineering.
A tecnologia é consequência do problema, não vitrine.

- **Arquitetura multi-tenant** com isolamento *fail-closed* no ORM, Row Level Security e resiliência transacional
- **Integração fiscal real** — NFC-e/NF-e via SEFAZ, PIX com webhook e travas de conformidade (NCM/CEST/CFOP)
- **Dados aplicados à decisão** — Curva ABC, RFM, DRE, previsão de ruptura e dashboards
- **Do banco ao deploy** — backend, frontend, PostgreSQL, Docker e CI/CD
- **São Paulo, Brasil** — atendimento local e remoto, aberto a novas oportunidades

---

## Stack

**Backend & Dados**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)

**Frontend**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)

**DevOps & Ferramentas**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat-square&logo=render&logoColor=black)

---

## Projetos em produção

### ERP multi-tenant com PDV fiscal — mercadinhosys

Plataforma de gestão comercial: ERP, PDV fiscal, recebimentos e Business Intelligence
na mesma base.

- **Multi-tenancy isolado (fail-closed):** toda consulta passa por um `TenantQuery` no ORM — um lojista nunca enxerga dado de outro, nem por injection; rota sem tenant resolvido recebe `403`.
- **Motor fiscal NFC-e/NF-e:** emissão via Focus NFe (SEFAZ), tratativa de rejeições, DANFE com QR Code e travas de conformidade que bloqueiam emissão sem NCM/CEST/CFOP válido.
- **Resiliência transacional:** *savepoints* aninhados isolam falhas pontuais para que o fechamento de venda no PDV não aborte a transação principal.
- **Catálogo inteligente:** *harvester* por código de barras com cache negativo e importação de XML de nota de entrada (EAN, NCM, lotes e custos).
- **BI:** Curva ABC (Pareto), RFM, previsão de ruptura e DRE automática.
- **Qualidade:** testes automatizados nos pontos críticos, CI com typecheck e build, deploy Vercel + Render.

`React` `TypeScript` `Flask` `SQLAlchemy` `PostgreSQL` `Docker` `Focus NFe` `CI/CD`

### MiseOn — SaaS multi-tenant para food service

Cardápio digital, pedidos em tempo real e gestão para restaurantes. Uma instância,
várias lojas, com **PIX na plataforma (Efí Bank) confirmado por webhook**, painel PWA
com pedidos ao vivo (WebSocket), comanda térmica e **estoque como ledger** com baixa
por ficha técnica.

`React 19` `TypeScript` `Supabase/RLS` `Deno` `Three.js` `PWA` `CI/CD`

### MySuperStore — marketplace multi-vendedor

Marketplace headless com **PIX e cartão e split automático de receita entre lojas
(Efí Bank)**, frete cotado em tempo real (Melhor Envio) e processamento assíncrono.

`Django REST` `Next.js 15` `PostgreSQL` `Redis` `Celery`

### SelectSys Jobs — ATS bilíngue (Brasil → Japão)

Sistema de recrutamento com cadastro bilíngue, leitura de documentos via OCR
(Tesseract.js / PDF.js), exportação para planilhas e permissões por empresa com RLS.

`React 19` `Tailwind` `Playwright` `OCR` `PostgreSQL/RLS`

---

## Dados & BI

### Animaz Pet Center — relatório analítico

Pipeline que ingere três bases do cliente e monta o relatório completo: **faturamento
contra meta**, **ruptura de estoque** e **funil de atendimento por vendedor**.

`Python` `Pandas` `Ingestão de dados`

### iContas — controle financeiro

Categorização automática de gastos, análise por período e visualização de dados.

`Python`

---

## Como eu trabalho

```
Problema do cliente → Diagnóstico → Solução sob medida → Entrega → Suporte
```

Não entrego template. Cada projeto começa com perguntas sobre o **negócio**, não sobre
tecnologia. A conversa vem antes do código.

---

<div align="center">

### GitHub em números

<img height="165" src="https://github-readme-stats.vercel.app/api?username=MaldivaSky&show_icons=true&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=C9A84C&icon_color=C9A84C&text_color=F0EBE1" alt="Estatísticas do GitHub" />
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MaldivaSky&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=C9A84C&text_color=F0EBE1" alt="Linguagens mais usadas" />

<br/>

<sub>Maldivas Tech · Rafael Paiva Dias da Silva Consultoria em Tecnologia da Informação LTDA</sub>

</div>
