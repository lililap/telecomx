# 📊 Análise de Churn - TelecomX

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-green.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5+-orange.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11+-red.svg)

## 🎯 Objetivo do Projeto

Este projeto foi desenvolvido para identificar as principais causas de **churn** (evasão de clientes) da empresa TelecomX através de análise exploratória de dados. O objetivo é fornecer insights acionáveis para reduzir a taxa de evasão e melhorar a retenção de clientes.

> **Desenvolvido para:** Curso de Data Science da Alura/Oracle  
> **Plataforma:** Google Colab  
> **Linguagem:** Python

## 🛠️ Tecnologias Utilizadas

- **Python 3.8+**
- **Pandas** - Manipulação e análise de dados
- **NumPy** - Computação numérica
- **Matplotlib** - Visualização de dados
- **Seaborn** - Visualizações estatísticas avançadas

## 📋 Metodologia

### 1. 🧹 Limpeza e Tratamento de Dados
- Substituição de 224 valores vazios (`''`) na coluna "Churn"
- Correção de 11 valores vazios (`' '`) na coluna "account_charges_total"
- Identificação de valores nulos usando `isnull()` e `isin()` do Pandas

### 2. 🔍 Análise Exploratória de Dados
Análise segmentada por múltiplas dimensões para identificar padrões de churn:
- Perfil demográfico (idade, gênero)
- Características do serviço (tipo de internet, contratos)
- Comportamento financeiro (gastos mensais/anuais)
- Métodos de pagamento

## 📈 Principais Fatores de Churn Identificados

| Fator | Impacto no Churn |
|-------|------------------|
| **Senioridade** | Clientes sênior têm taxa de churn **superior à média** |
| **Tenure** | Clientes novos têm **maior propensão** à evasão |
| **Fibra Ótica** | Serviço premium com taxa de churn **acima da média** |
| **Contrato Mensal** | Flexibilidade resulta em **maior evasão** |
| **Cobrança Eletrônica** | Método apresenta churn **superior à média** |
| **Gasto Mensal Alto** | Correlação com **maior churn** |
| **Gasto Anual Alto** | Correlação com **menor churn** |

## 📊 Exemplos de Visualizações

### Distribuição de Churn por Quartil de Tenure
![tenure](https://github.com/user-attachments/assets/225ae52c-ab93-455e-85e1-da350dbf5e40)


### Relação entre Gastos Mensais/Totais e Taxa de Churn
![gastos](https://github.com/user-attachments/assets/a77de266-026f-42ac-adf8-e21edb8bcfc2)


## 🚀 Como Executar o Projeto

### Pré-requisitos
- Python 3.8 ou superior
- Jupyter Notebook ou Google Colab
- Conexão com internet (para instalação de dependências)

### Instalação e Execução

1. **Clone o repositório:**
```bash
git clone https://github.com/lililap/telecomx.git
```

2. **Instale as dependências:**
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

3. **Execute o notebook:**
```bash
jupyter notebook TelecomX_Challenge_Lidia_Lapertosa.ipynb
```

### Executando no Google Colab

1. Faça upload do arquivo `.ipynb` para o Google Colab
2. Execute a primeira célula para instalar dependências:
```python
!pip install pandas numpy matplotlib seaborn
```
3. Execute as células sequencialmente

## 🎯 Principais Recomendações

### Para a TelecomX:

1. **🎯 Programa de Atenção Especial**
   - Foco em clientes sênior e novos (primeiros 6 meses)

2. **🔧 Melhoria da Experiência**
   - Revisão da jornada de clientes Fibra Ótica

3. **💼 Estratégia de Contratos**
   - Incentivos para migração de contratos mensais para anuais

4. **💳 Otimização de Pagamentos**
   - Melhoria do processo de cobrança eletrônica

5. **🎨 Retenção Personalizada**
   - Estratégias baseadas no perfil de gasto do cliente

### Para o Time de Data Science:

- **Feature Engineering:** Criar variáveis combinadas e temporais
- **Segmentação Preditiva:** Modelos específicos por segmento
- **Análise de Sobrevivência:** Implementar modelos Cox/Kaplan-Meier
- **Investigação de Interações:** Explorar relações entre variáveis
- **Validação Temporal:** Testar estabilidade dos modelos

## 📊 Insights Principais

### 🔍 Paradoxos Descobertos:
- **Tecnológico:** Fibra ótica (melhor serviço) = maior churn
- **Financeiro:** Gasto mensal alto = maior churn vs. Gasto anual alto = menor churn
- **Demográfico:** Clientes sênior mais propensos ao churn

### 🎯 Janela Crítica:
- **Primeiros 6 meses** são decisivos para retenção
- Período de onboarding é **fator crítico** de sucesso

## 📞 Contato

<div align="left">
<img src="https://github.com/user-attachments/assets/07594e84-2524-4810-a5dc-58abc9526ca3" alt="imagem autora do projeto" width="150px">

**Lidia Lapertosa**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lidia-lapertosa/)

📧 Em caso de dúvidas, entre em contato!

---

Desenvolvido como parte do curso de Data Science da **Alura/Oracle**.

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!
