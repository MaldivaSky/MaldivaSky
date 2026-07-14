<div align="center">

<img src="https://avatars.githubusercontent.com/u/60511607?v=4" width="110" style="border-radius:50%" alt="Rafael Maldivas"/>

# Rafael Paiva · `MaldivaSky`

### Desenvolvedor Fullstack · Análise de Dados & BI

**Transformo problemas reais de negócio em software que roda em produção.**

Fullstack (Python · TypeScript · React) com background de +10 anos em vendas e inteligência de mercado.
Uno engenharia de software, análise de dados e visão de negócio — código que gera decisão, não só telas.

[![Portfólio](https://img.shields.io/badge/Portfólio-rafael--maldivas.vercel.app-6D28D9?style=for-the-badge&logo=vercel&logoColor=white)](https://rafael-maldivas.vercel.app)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rafael_Paiva_Dias-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rafael-paiva-dias-da-silva-022b17122/)
[![Email](https://img.shields.io/badge/Email-rafaelmaldivas@gmail.com-C9A84C?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rafaelmaldivas@gmail.com)

</div>

---

## 👋 Sobre

Sou **Rafael Maldivas**, graduado em Análise e Desenvolvimento de Sistemas (IFSP). Construo **plataformas SaaS multi-tenant, ERPs com emissão fiscal e apps com IA — em produção.**

Antes de escrever uma linha de código, entendo o problema: o fluxo do negócio, o que trava o cliente, o que faz ele perder dinheiro. Depois entrego a solução certa — sem over-engineering, sem enrolação. A tecnologia é consequência do problema, não vitrine.

- 🎯 **Arquitetura multi-tenant** com isolamento *fail-closed* no ORM, RLS e resiliência transacional
- - 🧾 **Integração fiscal real** — NFC-e/NF-e via SEFAZ, PIX com webhook, conformidade tributária (NCM/CEST/CFOP)
  - - 📊 **Análise de dados aplicada** — Curva ABC, RFM, DRE, previsão de ruptura, Power BI
    - - 🧩 **Do banco ao deploy** — backend, frontend, PostgreSQL, Docker e CI/CD
      - - 🌍 São Paulo · Brasil · **Remoto** · Aberto a novas oportunidades
       
        - ---

        ## 🛠️ Stack

        **Backend & Dados**

        ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
        ![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
        ![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
        ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
        ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
        ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
        ![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
        ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black)
        ![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)

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

        ## ⭐ Carro-chefe — MercadinhoSys `v5.0 Enterprise`

        > **Plataforma SaaS multi-tenant de gestão comercial e e-commerce.** ERP, PDV fiscal, recebimentos e Business Intelligence numa única plataforma na nuvem — *production ready*.
        >
        > 🔗 **Repositório:** [github.com/MaldivaSky/mercadinhosys](https://github.com/MaldivaSky/mercadinhosys) · 🚀 **Demo:** [mercadinhosys.vercel.app](https://mercadinhosys.vercel.app)
        >
        > **Engenharia que faz a diferença:**
        >
        > - 🏢 **Multi-tenancy isolado (fail-closed):** toda query é blindada pelo `TenantQuery` no ORM — um lojista nunca acessa dado de outro, nem por injection; rotas sem tenant resolvido recebem `403`.
        > - - 🛡️ **Resiliência transacional:** *savepoints* aninhados (`begin_nested` / psycopg2) isolam falhas pontuais (ex.: schema drift) para que o fechamento de venda no PDV **nunca aborte** a transação principal — zero-downtime.
        >   - - 🧾 **Motor fiscal NFC-e/NF-e:** emissão nativa via **Focus NFe → SEFAZ**, tratativa de rejeições, DANFE com QR Code e **travas de conformidade** (bloqueia emissão sem NCM/CEST/CFOP válido).
        >     - - 📦 **Catálogo inteligente:** *harvester* por código de barras (**API Cosmos/Bluesoft**) com **cache negativo TTL 7 dias** p/ preservar quota + **importação de XML** de nota de entrada (EAN, NCM, lotes, custos).
        >       - - 📊 **BI científico:** dashboards em tempo real, **Curva ABC (Pareto)**, **RFM de clientes**, previsão de ruptura de estoque e **DRE** automática (despesas × faturamento líquido).
        >         - - 📱 **PWA mobile-first:** painel SaaS, seletor de tenant e auditoria na palma da mão; impersonação de lojista em 1 clique para suporte.
        >           - - 🧪 **Qualidade & deploy:** **41 testes pytest** nos pontos críticos, CI no **GitHub Actions** (typecheck + build + testes), deploy automático **Vercel + Render** e migrações seguras com Flask-Migrate.
        >            
        >             - `React 18` `TypeScript` `Flask` `SQLAlchemy` `PostgreSQL` `Docker` `Focus NFe` `API Cosmos` `CI/CD`
        >            
        >             - ---
        >
        > ## 🚀 Outros projetos em produção
        >
        > ### 🍔 [MiseOn](https://github.com/MaldivaSky/MiseOn) · SaaS multi-tenant para food service
        > Uma instância, várias lojas (`/sua-loja`). **PIX na plataforma (Efí Bank) com confirmação por webhook**, painel PWA com pedidos em tempo real (WebSocket) e comanda térmica, e **estoque como ledger** com baixa automática por ficha técnica. Multi-tenant com RLS e **Edge Functions (Deno)**.
        > `React` `TypeScript` `Supabase/RLS` `Deno` `Docker` `CI/CD` · [Código](https://github.com/MaldivaSky/MiseOn)
        >
        > ### 🛒 [MySuperStore](https://github.com/MaldivaSky/MySuperStore) · Marketplace multi-vendedor
        > Marketplace headless com **PIX e cartão, split automático entre lojas (Efí Bank)**, frete em tempo real (Melhor Envio), filas com Celery e Redis.
        > `Django REST` `Next.js 15` `PostgreSQL` `Redis` `Celery` · [Demo](https://mysuperstore-lime.vercel.app) · [Código](https://github.com/MaldivaSky/MySuperStore)
        >
        > ### 🏛️ [Conecta Figueiredo](https://github.com/MaldivaSky/conecta-figueiredo) · Emancipação digital (setor público)
        > Plataforma para a **Secretaria de Saúde de Presidente Figueiredo (SEMS)** — inclusão digital: cidadania (Gov.br), identidade online, empregabilidade, segurança contra golpes e IA.
        > `React 19` `Tailwind` `Vite` · [Código](https://github.com/MaldivaSky/conecta-figueiredo)
        >
        > ### 🍸 [Lagoon Gastrobar](https://github.com/MaldivaSky/gastrobar-web) · Site premium + reservas
        > Reservas em tempo real, **mapa interativo do salão em SVG**, painel admin e tour 360°. Backend serverless com Supabase e RLS.
        > `JavaScript` `Supabase` `PostgreSQL/RLS` · [Demo](https://maldivasky.github.io/gastrobar-web/) · [Código](https://github.com/MaldivaSky/gastrobar-web)

        ---

        ## 📊 Dados & BI

        ### 📈 [Animaz DataAnalisys](https://github.com/MaldivaSky/Animaz-DataAnalisys)
        Análise de dados em Python para e-commerce: tratamento, exploração e visualização que orientam decisão do time. `Python` `Pandas`

        ### 💰 [iContas](https://github.com/MaldivaSky/iContas)
        Controle financeiro com categorização automática de gastos, análise por período e visualização de dados. `Python`

        ---

        ## 🧭 Como eu trabalho

        ```
        Problema do cliente → Diagnóstico → Solução sob medida → Entrega → Suporte
        ```

        Não entrego template. Entrego o que resolve. Cada projeto começa com perguntas sobre o **negócio**, não sobre tecnologia.

        ---

        <div align="center">

        ### 📊 GitHub em números

        ![Stats](https://github-readme-stats.vercel.app/api?username=MaldivaSky&show_icons=true&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=C9A84C&icon_color=C9A84C&text_color=F0EBE1)
        ![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=MaldivaSky&layout=compact&theme=midnight-purple&hide_border=true&bg_color=0D1117&title_color=C9A84C&text_color=F0EBE1)

        ---

        **🟢 Aberto a oportunidades** — Desenvolvedor Fullstack Pleno · Analista de Dados · Consultor de Soluções

        📬 [rafaelmaldivas@gmail.com](mailto:rafaelmaldivas@gmail.com) · 🌐 [Portfólio](https://rafael-maldivas.vercel.app) · 💼 [LinkedIn](https://www.linkedin.com/in/rafael-paiva-dias-da-silva-022b17122/)

        *"A melhor tecnologia é a que o cliente nem percebe — só sente o resultado."*

        </div>
        
