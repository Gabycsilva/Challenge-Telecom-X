# Challenge--TelecomX-1
Alura One 8 - Desafio TELECOM X parte 1


# 📊 Análise de Evasão de Clientes (Churn) – TelecomX

Este projeto apresenta uma análise exploratória dos dados de clientes da **TelecomX**, com o objetivo de identificar padrões associados à evasão de clientes (churn) e propor estratégias de retenção mais eficazes.

---

## 📁 Conjunto de Dados

O conjunto de dados utilizado é o **TelecomX_Data.json**, contendo informações detalhadas sobre:

- Dados demográficos dos clientes  
- Serviços contratados (telefone, internet, pacote)  
- Informações de conta e cobrança  
- Status de cancelamento (churn)

---

## 🔍 Etapas da Análise

O notebook aborda as seguintes fases:

### 1. **Extração e Limpeza de Dados**
- Carregamento do arquivo JSON
- Combinação de estruturas aninhadas em um único DataFrame
- Renomeação de colunas para maior clareza (ex.: `customerID` → `ID_Cliente`)
- Conversão de variáveis para tipos numéricos
- Preenchimento de valores nulos e remoção de "falsos nulos" (224 linhas com espaços em branco na coluna `Cancelou`)

### 2. **Transformação de Dados**
- Criação de novas colunas para análise de cobranças diárias
- Padronização de tipos e formatos para facilitar a visualização

### 3. **Análise Exploratória**
- Comparativo entre clientes idosos e não idosos em relação ao tempo de permanência e valores pagos
- Distribuição de clientes e taxas de cancelamento por gênero
- Comparação entre clientes com pacote completo e incompleto
- Identificação dos métodos de pagamento mais associados ao churn
- Análise da distribuição de variáveis numéricas (`Meses_Permanencia`, `Cobranca_Total`) para clientes que cancelaram e não cancelaram
- Determinação do grupo com maior taxa de cancelamento

### 4. **Visualizações**
- Geração de gráficos de barras e histogramas para ilustrar os principais achados

### 5. **Relatório Final**
- Compilação das descobertas, conclusões e recomendações estratégicas

---

## 📌 Principais Descobertas

- Clientes com **menor tempo de permanência** e **pacote incompleto** apresentam maior probabilidade de cancelamento.
- O método de pagamento **Electronic Check** está fortemente associado ao churn (57,30%).
- Gênero e status de idoso têm impacto menor quando analisados isoladamente.
- O grupo com **maior taxa de cancelamento** foi o de clientes com **Pacote Incompleto** (27,51%).

---

## ▶️ Como Executar o Notebook

1. Abra o notebook em um ambiente Python com as bibliotecas necessárias instaladas (`pandas`, `numpy`, `matplotlib`).
2. Execute as células sequencialmente para replicar a análise.
3. Certifique-se de que o arquivo **TelecomX_Data.json** esteja acessível localmente ou via URL.

---

## 📄 Relatório Detalhado

Consulte a seção **"Relatório Final"** no notebook para uma descrição aprofundada das análises, interpretações e recomendações estratégicas.

---
