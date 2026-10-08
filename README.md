# 📊 Agregador de Dados para Declaração de Imposto de Renda

Este repositório contém uma ferramenta robusta e automatizada desenvolvida no Excel para centralizar, validar e consolidar informações essenciais para a Declaração de Imposto de Renda da Pessoa Física (IRPF). O projeto foi desenhado focando em boas práticas de modelagem de dados, arquitetura de planilhas e design focado na experiência do usuário (UX/UI Dashboard).

## 🚀 Funcionalidades Técnicas Implementadas

*   **Validação Automatizada de Dados:** Uso de listas dinâmicas baseadas nas categorias oficiais da Receita Federal, impedindo erros de digitação e inconsistências na base de lançamentos.
*   **Motor de Cálculo Fiscal (Fórmulas Avançadas):**
    *   Somas condicionais (`SOMASE` / `SOMASES`) para aglutinar rendimentos e despesas dedutíveis em tempo real.
    *   Busca inteligente por aproximação (`PROCV` com argumento `VERDADEIRO`) mapeando a tabela progressiva anual para encontrar a alíquota correta e a parcela a deduzir de forma dinâmica.
    *   Tratamento de erros sistêmicos (`SEERRO`) garantindo uma interface limpa e profissional mesmo sem lançamentos prévios.
*   **Navegação e UX Fluida:** Layout estruturado sem linhas de grade, botões com hiperlinks internos simulando um sistema/web-app e cartões de KPI integrados para rápida leitura de métricas vitais.

## 🏛️ Estrutura do Arquivo Excel

1.  **`Menu_Inicial`:** Tela de boas-vindas com botões de navegação, guia rápido de uso e links oficiais de utilidade pública (Receita Federal, Portal e-CAC).
2.  **`Lancamentos`:** Banco de dados estruturado como Tabela do Excel onde o usuário alimenta o histórico de entradas e saídas.
3.  **`Dashboard_Calculos`:** O motor analítico contendo o resumo consolidado dos rendimentos, deduções permitidas, base de cálculo e estimativa final do imposto devido.
4.  **`Suporte_Tabelas`:** Aba de infraestrutura de dados onde residem os vetores de validação e a tabela progressiva de alíquotas oficiais.

## 🛠️ Como Utilizar
1. Baixe o arquivo `Gerenciador_Imposto_Renda_DIO.xlsx` disponível neste repositório.
2. Acesse a aba `Lancamentos` e cadastre seus comprovantes, salários e despesas dedutíveis médicas/educacionais selecionando as categorias correspondentes.
3. Visualize os resultados consolidados instantaneamente na aba de cálculos ou utilize os dados para alimentar os gráficos do seu Dashboard visual.

---
*Projeto desenvolvido como parte do Desafio de Excel e GitHub da Digital Innovation One (DIO).*
