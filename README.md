# 🏎️ Porsche Sales — Data Intelligence Dashboard

![Status](https://img.shields.io/badge/Status-Online-c7ff3d?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-Single_File-21e6ff?style=for-the-badge&logo=html5&logoColor=080c12)
![CSS3](https://img.shields.io/badge/CSS3-Responsive_Dark_UI-a78bfa?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla_Interactive-f1f6fb?style=for-the-badge&logo=javascript&logoColor=080c12)

> **Dashboard interativa de inteligência comercial** desenvolvida a partir de uma base sanitizada de 100 vendas da Porsche e publicada em arquivo único (`index.html`), substituindo planilhas estáticas por uma experiência analítica responsiva na web.

🔗 **[Acesse a Dashboard Online (GitHub Pages)](https://mateusuchoa.github.io/DESAFIO_DIO_Dashboard_Porsche/)**

---

## 📸 Preview da Aplicação

### Visão Geral (Sem filtros)
![Visão Geral da Dashboard](https://github.com/user-attachments/assets/e849809f-c2c7-475a-8025-f3e1abf992cf)

### Visão Segmentada (Com filtros aplicados)
![Dashboard com Filtros Aplicados](https://github.com/user-attachments/assets/c2582aba-33cf-4699-84a9-cc93bfe25610)

---

## 🎯 Perguntas de Negócio Respondidas

A arquitetura visual foi planejada para responder diretamente às principais questões estratégicas da operação comercial:

1. **Qual é o ranking de modelos mais vendidos e quais anos concentram o maior volume?**
   * **Impacto no negócio:** Direciona a alocação de estoque e campanhas comerciais para o mix de produtos com maior giro.
   * **Visualização:** Ranking comparativo de modelos e distribuição por ano de fabricação (*Model Year*).

2. **Quais modelos lideram as vendas em cada estado/cidade?**
   * **Impacto no negócio:** Mapeia a demanda regional para orientar ações locais de concessionárias e expansão de praças.
   * **Visualização:** Tabela interativa segmentada por localidade com detalhamento de modelos e volume.

3. **Qual é o método de pagamento predominante entre os compradores?**
   * **Impacto no negócio:** Apoia a área financeira na calibragem de parcerias de crédito, taxas e condições comerciais.
   * **Visualização:** Gráfico dinâmico com a participação percentual e absoluta de cada forma de pagamento.

---

## ✨ Funcionalidades e Arquitetura

* **KPIs Executivos:** Indicadores de topo atualizados em tempo real conforme os recortes selecionados.
* **Filtros Combinados:** Barra interativa com 4 dimensões de análise (`City`, `Modelo da Porsche`, `Model Year` e `Pay Method`) e botão de reset imediato.
* **Insights Dinâmicos:** Cards de leitura rápida que sintetizam os principais destaques do recorte atual.
* **Identidade Visual (Dark Telemetry UI):** Interface inspirada no portal oficial da Porsche Brasil e em painéis de telemetria automotiva (`#080c1
