# Projeto NPS Preditivo – Tech Challenge Fase 1

## 📌 Objetivo
Este projeto tem como objetivo analisar fatores que influenciam a satisfação dos clientes de um e-commerce, medida pelo **Net Promoter Score (NPS)**, e propor estratégias para antecipar problemas e melhorar a experiência do cliente.  
Além da análise exploratória (EDA), o projeto inclui reflexões sobre como modelos preditivos podem apoiar decisões de negócio.

---

## 📂 Estrutura do Repositório
nps-preditivo/
│
├── data/                # Bases de dados (raw e processed)
├── notebooks/           # Notebooks de EDA e protótipos
├── src/                 # Funções reutilizáveis (limpeza, modelagem)
├── models/              # Modelos treinados (se aplicável)
├── reports/             # Gráficos, tabelas e storytelling
├── README.md            # Documentação principal
└── environment.yml      # Dependências do projeto (Conda)

---

## 📊 Base de Dados
**Arquivo:** `Base de dados NPS.csv`  
**Descrição das variáveis principais:**
- `customer_id`: Identificador único do cliente  
- `order_id`: Identificador único do pedido  
- `customer_age`: Idade do cliente  
- `customer_region`: Região geográfica  
- `order_value`: Valor total do pedido  
- `delivery_time_days`: Tempo total de entrega  
- `delivery_delay_days`: Dias de atraso na entrega  
- `customer_service_contacts`: Número de contatos com atendimento  
- `complaints_count`: Número de reclamações  
- `nps_score`: Nota de satisfação (0–10)  

---

## 🛠️ Metodologia
1. **Entendimento do negócio**  
   - Identificação da dor: variabilidade do NPS e impacto na experiência do cliente.  
   - Reflexão sobre impacto em recompra, boca a boca e market share.  

2. **Definição da Target**  
   - Variável alvo: `nps_score`.  
   - Justificativa: métrica oficial de satisfação coletada após a compra.  

3. **Análise Exploratória (EDA)**  
   - Identificação de fatores críticos (logística, atendimento, valor do pedido).  
   - Visualizações para explicar padrões de NPS.  

4. **Reflexão sobre Modelagem Preditiva (opcional)**  
   - Estratégias possíveis: regressão (nota contínua) ou classificação (promotor/detrator).  
   - Avaliação com métricas adequadas (RMSE, MAE, precisão, recall, F1).  

---

## 🚀 Como Reproduzir
1. Clone este repositório:
   ```bash
   git clone https://github.com/usuario/nps-preditivo.git
   cd nps-preditivo
