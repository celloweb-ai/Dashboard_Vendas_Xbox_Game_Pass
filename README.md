# 📊 Dashboard de Vendas - Xbox Game Pass

> Análise e visualização de dados de assinaturas do Xbox Game Pass com dashboard interativo em Excel

[![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/excel)
[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🔗 Acesso Rápido

📊 **[Baixar Planilha Excel](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/raw/main/data/Base%20Dados%20Xbox%20Game%20Pass.xlsx)** - Dashboard completo com dados de assinaturas

## 🎯 Objetivo

Este projeto apresenta uma solução completa de análise de dados de assinaturas do Xbox Game Pass, transformando dados brutos em insights visuais e acionáveis para tomada de decisões estratégicas. O dashboard desenvolvido em Excel permite monitorar KPIs de vendas, receitas, renovações e desempenho de add-ons.

## 📁 Estrutura do Repositório

```
Dashboard_Vendas_Xbox_Game_Pass/
│
├── data/
│   ├── Base Dados Xbox Game Pass.xlsx  # Planilha original com dados brutos
│   ├── base_dados.csv                   # Base de dados em formato CSV
│   └── sheets_data.json                 # Dados estruturados em JSON
│
├── README.md                            # Documentação do projeto
└── LICENSE                              # Licença MIT
```

## 📊 Sobre os Dados

### Base de Dados

O dataset contém **295 registros de assinaturas** do Xbox Game Pass cobrindo o período de **janeiro a dezembro de 2024**, com IDs de assinantes variando de **3231 a 3525**.

**📂 Arquivos Disponíveis:**
- **[Base Dados Xbox Game Pass.xlsx](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/blob/main/data/Base%20Dados%20Xbox%20Game%20Pass.xlsx)** - Planilha Excel completa
- **[base_dados.csv](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/blob/main/data/base_dados.csv)** - Formato CSV para análise
- **[sheets_data.json](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/blob/main/data/sheets_data.json)** - Formato JSON estruturado

### Estrutura dos Dados

| Campo | Tipo | Descrição |
|-------|------|-----------|
| **Subscriber ID** | Numérico | Identificador único do assinante (3231-3525) |
| **Name** | Texto | Nome completo do assinante |
| **Plan** | Categórico | Tipo de plano (Ultimate, Standard, Core) |
| **Start Date** | Data | Data de início da assinatura (DD/MM/YYYY) |
| **Auto Renewal** | Booleano | Status de renovação automática (Yes/No) |
| **Subscription Price** | Numérico | Preço base da assinatura ($) |
| **Subscription Type** | Categórico | Periodicidade (Monthly, Quarterly, Annual) |
| **EA Play Season Pass** | Numérico | Valor do add-on EA Play ($0 ou $30) |
| **Minecraft Season Pass** | Numérico | Valor do add-on Minecraft ($0 ou $20) |
| **Coupon Value** | Numérico | Valor do cupom de desconto aplicado ($) |
| **Total Value** | Numérico | Valor final após descontos ($) |

### Planos Disponíveis

| Plano | Preço Base | Características | Add-ons Disponíveis |
|-------|------------|------------------|---------------------|
| **Ultimate** | $15 | Acesso completo + Cloud Gaming + multiplayer | EA Play ($30) + Minecraft ($20) |
| **Standard** | $10 | Acesso padrão à biblioteca de jogos | Minecraft ($20) |
| **Core** | $5 | Multiplayer online básico | Nenhum |

### Tipos de Assinatura

- **Monthly (Mensal)**: Cobrança mensal recorrente
- **Quarterly (Trimestral)**: Cobrança a cada 3 meses
- **Annual (Anual)**: Cobrança anual com desconto

## 📈 Análises e Insights

### Métricas Principais

O dashboard permite análise de:

1. **Faturamento Total**
   - Por tipo de plano (Ultimate, Standard, Core)
   - Por periodicidade (Mensal, Trimestral, Anual)
   - Com/sem renovação automática

2. **Desempenho de Add-ons**
   - Vendas de EA Play Season Pass (exclusivo Ultimate)
   - Vendas de Minecraft Season Pass (Standard e Ultimate)
   - Receita adicional gerada por add-ons

3. **Taxa de Renovação**
   - Percentual de assinaturas com auto-renovação ativa
   - Comparação entre planos

4. **Impacto de Cupons**
   - Valor total de descontos aplicados
   - Análise de rentabilidade por tipo de cupom

5. **Sazonalidade**
   - Distribuição de assinaturas ao longo de 2024
   - Períodos de maior/menor aquisição

### KPIs do Dashboard

- ✅ Receita Total: Soma de todos os valores finais
- ✅ Ticket Médio: Valor médio por assinatura
- ✅ Taxa de Conversão: Percentual de renovação automática
- ✅ Receita por Add-on: Contribuição dos Season Passes
- ✅ Distribuição de Planos: Percentual por categoria

## 🎨 Identidade Visual

### Paleta de Cores Xbox

O dashboard utiliza as cores oficiais da marca Xbox para manter consistência visual:

- **Verde Principal**: `#107C10` (Xbox Verde)
- **Verde Claro**: `#9BC848`, `#22C55E`
- **Accent**: `#2AE6B1`, `#5BF6A8`
- **Background**: `#E8E6E9`
- **Texto**: `#1A1A1A`

## 🚀 Como Utilizar

### Pré-requisitos

- Microsoft Excel 2016 ou superior (recomendado Excel 365)
- Python 3.8+ (opcional, para processamento de dados)
- Conhecimento básico de tabelas dinâmicas e gráficos

### Instalação

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass.git
   cd Dashboard_Vendas_Xbox_Game_Pass
   ```

2. **Acesse os dados:**
   ```bash
   cd data
   ```

3. **Abra a planilha Excel:**
   - **Download direto**: [Base Dados Xbox Game Pass.xlsx](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/raw/main/data/Base%20Dados%20Xbox%20Game%20Pass.xlsx)
   - Ou navegue até a pasta `data/` e abra `Base Dados Xbox Game Pass.xlsx`
   - Explore as abas disponíveis

### Formatos Disponíveis

Os dados estão disponíveis em 3 formatos:

1. **[Excel (`.xlsx`)](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/raw/main/data/Base%20Dados%20Xbox%20Game%20Pass.xlsx)**: Formato original com formatação e fórmulas
2. **[CSV (`.csv`)](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/raw/main/data/base_dados.csv)**: Formato universal para análise em Python, R, etc.
3. **[JSON (`.json`)](https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/raw/main/data/sheets_data.json)**: Formato estruturado para APIs e aplicações web

### Exemplo de Uso em Python

```python
import pandas as pd
import json

# Carregar dados do CSV
df = pd.read_csv('data/base_dados.csv')

# Análise rápida
print(df.describe())
print(df['Plan'].value_counts())

# Carregar JSON
with open('data/sheets_data.json', 'r', encoding='utf-8') as f:
    data = json.load(f)
    print(f"Total de registros: {len(data)}")
```

## 🛠️ Tecnologias e Ferramentas

### Análise de Dados
- **Microsoft Excel**: Dashboard e visualizações
- **Tabelas Dinâmicas**: Agregação e sumarização de dados
- **Gráficos Dinâmicos**: Visualizações interativas
- **Formatação Condicional**: Destaque de informações críticas

### Processamento de Dados
- **Python**: Manipulação e limpeza de dados
- **Pandas**: Análise de dados estruturados
- **JSON**: Serialização de dados

## 📚 Competências Demonstradas

Este projeto evidencia habilidades em:

- ✅ **Análise Exploratória de Dados (EDA)**
- ✅ **Business Intelligence (BI)**
- ✅ **Data Visualization**
- ✅ **Dashboard Design**
- ✅ **Excel Avançado** (tabelas dinâmicas, gráficos, fórmulas)
- ✅ **Storytelling com Dados**
- ✅ **Documentação Técnica**
- ✅ **Gestão de Repositórios Git**

## 🔄 Atualizações Futuras

- [ ] Integração com Power BI para dashboards interativos online
- [ ] Análise preditiva com Machine Learning
- [ ] API REST para consulta de dados
- [ ] Automação de relatórios com Python
- [ ] Análise de churn e retenção de clientes
- [ ] Dashboard web interativo com Streamlit ou Dash

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um **fork** do projeto
2. Crie uma **branch** para sua feature
   ```bash
   git checkout -b feature/MinhaNovaAnalise
   ```
3. **Commit** suas mudanças
   ```bash
   git commit -m 'Add: análise de churn por plano'
   ```
4. Faça **push** para a branch
   ```bash
   git push origin feature/MinhaNovaAnalise
   ```
5. Abra um **Pull Request**

### Diretrizes de Contribuição

- Mantenha o código limpo e documentado
- Atualize o README.md se adicionar novas funcionalidades
- Teste suas mudanças antes de submeter
- Use commits semânticos (feat, fix, docs, style, refactor)

## 📝 Licença

Este projeto está sob a licença **MIT**. Consulte o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👤 Autor

**Marcus Vasconcellos**

- 🌐 GitHub: [@celloweb-ai](https://github.com/celloweb-ai)
- 💼 LinkedIn: [marcusvasconcellos](https://www.linkedin.com/in/marcusvasconcellos)
- 📧 Email: marcus@vasconcellos.net.br

## 🎓 Contexto Acadêmico

Projeto desenvolvido como parte do bootcamp **DIO - CAIXA - Inteligência Artificial na Prática**, demonstrando aplicação prática de conceitos de análise de dados, business intelligence e visualização de informações.

## 📊 Estatísticas do Projeto

![GitHub repo size](https://img.shields.io/github/repo-size/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass)
![GitHub last commit](https://img.shields.io/github/last-commit/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass)
![GitHub issues](https://img.shields.io/github/issues/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass)
![GitHub stars](https://img.shields.io/github/stars/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass?style=social)

---

<div align="center">

⭐ **Se este projeto foi útil para você, considere dar uma estrela!**

📫 **Sugestões e feedback são sempre bem-vindos!**

**Desenvolvido com 💚 e Excel**

</div>