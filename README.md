# 🏎️ Porsche Sales — Data Intelligence Dashboard

![Status](https://img.shields.io/badge/Status-Online-c7ff3d?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-Single_File-21e6ff?style=for-the-badge&logo=html5&logoColor=080c12)
![CSS3](https://img.shields.io/badge/CSS3-Responsive_Dark_UI-a78bfa?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla_Interactive-f1f6fb?style=for-the-badge&logo=javascript&logoColor=080c12)

> **Dashboard interativa de inteligência comercial** construída a partir de uma base sanitizada de 100 vendas da Porsche, publicada na web em arquivo único (`index.html`) — eliminando as limitações estáticas de planilhas tradicionais.

🔗 **[Acesse a Dashboard Online (GitHub Pages)]([(https://mateusuchoa.github.io/DESAFIO_DIO_Dashboard_Porsche/))]**

---

## 📸 Preview da Aplicação

### Visão Geral (Sem filtros)
![Preview Geral da Dashboard](<img width="1328" height="595" alt="semFiltros" src="https://github.com/user-attachments/assets/e849809f-c2c7-475a-8025-f3e1abf992cf" />)

### Exemplo com Filtro Aplicado
> Recorte aplicado: `[Ex: Modelo 911 | Pagamento: Financiamento | Ano: 2024]`
![Preview com Filtro Aplicado](<img width="1322" height="598" alt="comFiltros" src="https://github.com/user-attachments/assets/c2582aba-33cf-4699-84a9-cc93bfe25610" />)

---

## 🎯 Perguntas de Negócio Respondidas

Em vez de apenas empilhar gráficos, a dashboard foi desenhada para responder diretamente a **três perguntas estratégicas** sobre a operação comercial:

1. **[Pergunta 1 — Ex: Quais modelos e anos concentram o maior volume de vendas?]**
   * **Por que importa:** Direciona a alocação de estoque e campanhas de marketing para o mix de produtos com maior giro.
   * **Como é respondida:** Gráfico de barras horizontais comparativo e ranking de combinações (modelo + ano).

2. **[Pergunta 2 — Ex: Qual é o perfil predominante de pagamento dos clientes?]**
   * **Por que importa:** Ajuda a área financeira a calibrar parcerias de crédito, taxas e condições comerciais.
   * **Como é respondida:** Gráfico de rosca (donut) dinâmico com distribuição percentual e absoluta por método de pagamento.

3. **[Pergunta 3 — Ex: Como as vendas se distribuem geograficamente por estado/cidade?]**
   * **Por que importa:** Identifica praças com maior demanda e regiões subexploradas para expansão de concessionárias.
   * **Como é respondida:** Tabela interativa segmentada por UF/cidade com detalhamento de modelos e volume.

---

## ✨ Funcionalidades e Arquitetura

* **KPIs Executivos:** Indicadores de topo atualizados em tempo real conforme os filtros aplicados (volume de vendas, receita e métricas-chave).
* **Filtros Combinados:** Barra de controle com 4 seletores interativos e botão de reset para recortes rápidos sem recarregar a página.
* **Insights Dinâmicos:** 3 cards de leitura rápida que sintetizam os principais destaques do recorte atual.
* **Design System Próprio:** Interface *Dark Mode* inspirada em painéis de telemetria automotiva (`#080c12` com acentos em ciano `#21e6ff`, lima `#c7ff3d` e violeta `#a78bfa`), tipografia tabular para números e layout 100% responsivo (desktop, mobile e impressão).
* **Zero Dependências Externas:** Toda a lógica, estilização e dados sanitizados rodam em um único arquivo `index.html`, garantindo carregamento instantâneo no GitHub Pages.

---

## 🧹 Tratamento de Dados (Data Prep)

Antes de enviar a base para a IA, foi realizado o preparo rigoroso dos 100 registros de vendas:

1. **Remoção de colunas brutas:** Mantidas apenas as colunas sanitizadas geradas na etapa de tratamento de dados.
2. **Tipagem numérica:** Conversão explícita de campos de **preço** e **ano** para formato numérico puro.
3. **Limpeza de fórmulas:** Cópia e colagem como valores (*Paste Values*) para evitar referências quebradas na exportação.
4. **Privacidade e Segurança:** Verificação completa para garantir que nenhum dado sensível ou PII (informação pessoal identificável) fosse embutido no HTML público.

---

## 🤖 Processo com IA e Evolução do Prompt

* **Ferramenta utilizada:** `[Ex: ChatGPT com recurso Canvas / Agente personalizado com Skill de Dashboard / Ambos]`

### Prompt Inicial
```text
[utilizando o canva faça um dashboad em html com os dados da planilha em anexo.

\#Filtros
-City
-Modelo da Porsche
-Model Year
-Pay Method

\#Perguntas de negocio e Kpi's
-quais os modelos de carros mais vendidos por estado
-Quais os anos dos modelos que mais venderam
-Ranking de modelos mais vendidos&#x20;
-Grafico de barras mostrando qual o metodo de pagamento mais usado

\#ux/design use de referência o site da porsche brasil

[https://www.porsche.com/brazil/pt/models/cayenne/cayenne-models/cayenne-e-hybrid/?utm_source=google&utm_medium=paid+search&utm_campaign=cid%3A20098139_ca%3Actgcayenne&utm_id=gad%7C23999061292%7C&utm_content=pn%3A20438681%7Ecn%3Acayenne+e3ii+suv+br%7Emo%3Acay_cay%7Eco%3Abr%7Eln%3Amx&gad_source=1&gad_campaignid=23989557258&gclid=CjwKCAiAq5rYBhB-EiwAhj1Rdk7s3NjsT5M5tvAaRmK9ZPEtx3CdYIe8IEm6lceQ5cZFOgN61ii9aBoCrBUQAvD_BwE](https://www.porsche.com/brazil/pt/models/cayenne/cayenne-models/cayenne-e-hybrid/?utm_source=google\&utm_medium=paid+search\&utm_campaign=cid%3A20098139_ca%3Actgcayenne\&utm_id=gad%7C23999061292%7C\&utm_content=pn%3A20438681%7Ecn%3Acayenne+e3ii+suv+br%7Emo%3Acay_cay%7Eco%3Abr%7Eln%3Amx\&gad_source=1\&gad_campaignid=23989557258\&gclid=CjwKCAiAq5rYBhB-EiwAhj1Rdk7s3NjsT5M5tvAaRmK9ZPEtx3CdYIe8IEm6lceQ5cZFOgN61ii9aBoCrBUQAvD_BwE)

tenha um estilo moderno, chamativo porem não muito extravagante.

obs se houver necessidade faça mais gráfico e coloque insights para enriquecer a analise de dados do dashboard]
