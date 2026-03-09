# 📊 Telecom X - Análise de Evasão de Clientes (Churn)

Este repositório contém a resolução do desafio prático de Data Science focado em entender e reduzir a evasão de clientes (Churn) na empresa fictícia Telecom X. O projeto abrange desde a extração de dados via API até a Análise Exploratória de Dados (EDA) e a geração de insights estratégicos para o negócio.

## 🎯 Objetivo do Projeto
A Telecom X enfrenta um alto índice de cancelamentos de serviços. O objetivo deste projeto foi coletar, tratar e analisar os dados dos clientes para identificar os principais fatores e padrões que levam à perda de usuários, fornecendo uma base sólida para futuras modelagens preditivas e estratégias de retenção.

## 🛠️ Tecnologias e Bibliotecas Utilizadas
* **Python** (Linguagem principal)
* **Pandas** (Manipulação, limpeza e tratamento de dados)
* **Requests** (Extração de dados de API)
* **Matplotlib & Seaborn** (Visualização de dados e criação de gráficos)

## 🚀 Etapas do Projeto

1. **Extração de Dados (API):** Consumo de dados no formato JSON diretamente de um repositório no GitHub.
2. **Transformação e Limpeza (ETL):** * Achatamento de dados aninhados (`json_normalize`).
   * Conversão de tipos de dados (strings para numéricos).
   * Tratamento de valores nulos e inconsistentes (espaços em branco).
   * Padronização de strings e tradução de categorias para o português.
   * Transformação de variáveis categóricas binárias (Sim/Não para 1/0).
3. **Análise Exploratória (EDA):**
   * Análise estatística descritiva.
   * Visualização da distribuição da variável alvo (Churn).
   * Cruzamento de variáveis categóricas (Contrato, Pagamento, Serviço de Internet) e numéricas (Mensalidade, Tempo de Permanência, Gasto Total) com a evasão.
4. **Geração de Insights:** Elaboração de um relatório executivo com recomendações de negócio.

## 🔍 Principais Insights e Conclusões
Após a análise, identificou-se que a base possui uma taxa de evasão de **27%**. O perfil de cliente com maior risco de cancelamento apresenta as seguintes características:
* **Tempo de Permanência:** A maioria dos cancelamentos ocorre nos primeiros meses de assinatura.
* **Tipo de Contrato:** Clientes com contratos na modalidade **Mensal** evadem significativamente mais do que aqueles com contratos anuais, devido à ausência de barreiras de saída.
* **Serviço Premium:** O serviço de internet via **Fibra Ótica** apresenta alta taxa de churn, acompanhado de mensalidades mais elevadas, sugerindo uma possível insatisfação com a relação custo-benefício.
* **Método de Pagamento:** Clientes que utilizam métodos manuais, como o **Cheque Eletrônico**, tendem a cancelar mais do que aqueles em débito automático.

## 💡 Recomendações Estratégicas
* Implementar campanhas de incentivo para migração de clientes do plano mensal para planos anuais.
* Revisar a precificação e a estabilidade técnica do serviço de Fibra Ótica.
* Oferecer benefícios para clientes que cadastrarem métodos de pagamento automáticos.
* Criar um programa de Onboarding focado nos primeiros meses de assinatura para garantir a satisfação inicial do cliente.

