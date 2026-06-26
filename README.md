# 📊 Marketing Analytics Dashboard | Power BI

![Capa do Projeto](assets/capa_dashboard.png) *(Substitua pelo caminho da sua imagem)*

## 📋 Visão Geral
Este projeto de Análise de Dados foi desenvolvido para avaliar a performance de campanhas de marketing, comportamento de clientes e conversão em pontos de vendas. O objetivo principal é transformar dados brutos de marketing em insights acionáveis, permitindo que a equipe de negócios direcione campanhas com maior precisão e ROI (Retorno sobre Investimento).

**Ferramentas Utilizadas:**
- **Power BI:** ETL (Power Query), Modelagem de Dados, DAX e Data Visualization.
- **HTML/CSS (via DAX):** Criação de visuais e cartões personalizados de alta performance (UI/UX UI).
- **Figma / PowerPoint:** (Se você usou para criar o background, cite aqui).

---

## 🎯 Problema de Negócio
A equipe de Marketing precisava responder a perguntas fundamentais para a estratégia do próximo trimestre:
1. Qual é o perfil demográfico dos nossos clientes mais engajados?
2. Como o estado civil e o número de filhos impactam o volume de compras?
3. Qual foi a taxa de sucesso das últimas campanhas e qual público mais converteu?
4. Quais canais e países geram mais receita?

---

## 🏗️ Estrutura e Modelagem de Dados
Os dados foram modelados seguindo o esquema estrela (*Star Schema*), garantindo alta performance nas consultas DAX.
* **Fato:** `fVendas`, `fCampanhas` *(coloque o nome das suas tabelas fato)*
* **Dimensões:** `dCalendario`, `dClientes`, `dLocalidade` *(coloque o nome das suas dimensões)*

---

## 🖥️ Telas do Dashboard

### 1. Visão Cliente
Análise demográfica focada em escolaridade, idade, média salarial e estado civil.
![Visão Cliente](assets/visao_cliente.png)

### 2. Visão Comportamento
Gráficos de dispersão e Árvore de Decomposição para entender cruzamentos de perfil vs. gastos.
![Visão Comportamento](assets/visao_comportamento.png)

### 3. Visão Campanhas
Análise de conversão (Comprou vs. Não Comprou) com paleta de cores focada em Data Storytelling para destacar resultados positivos.
![Visão Campanhas](assets/visao_campanhas.png)

### 4. Ponto de Vendas
Evolução temporal e ranking por categorias e top países consumidores.
![Visão Ponto de Vendas](assets/visao_pdv.png)

---

## 💻 Destaques Técnicos (DAX & UI/UX)
Para fugir do visual padrão do Power BI e oferecer uma experiência de aplicação web, utilizei o visual **HTML Content** aliado à linguagem DAX para construir cartões com degradê, sombras (CSS Box-Shadow) e ícones renderizados via SVG dinâmico.

*Exemplo do código DAX construído para a navegação:*
```dax
Botao HTML Campanhas = 
"
<div style='width:100%; height:100%; border-radius:18px; background:linear-gradient(135deg, #4B3FAF 0%, #5C4CE0 45%, #733EEE 100%); display:flex; flex-direction:column; align-items:center; justify-content:center;'>
    <!-- Estrutura SVG e CSS omitida para brevidade. Código completo na pasta dax_scripts -->
</div>
"
