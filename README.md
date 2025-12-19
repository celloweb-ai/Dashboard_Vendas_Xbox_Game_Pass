# 📊 Dashboard de Vendas - Xbox Game Pass

> Projeto de análise e visualização de dados de assinaturas do Xbox Game Pass desenvolvido em Excel

[![Excel](https://img.shields.io/badge/Excel-217346?style=flat&logo=microsoft-excel&logoColor=white)](https://www.microsoft.com/excel)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 🎯 Objetivo

Este projeto tem como objetivo criar um dashboard de vendas com foco na organização e visualização de dados de assinaturas do Xbox Game Pass. O desafio consiste em transformar dados brutos em informações visuais claras e úteis, permitindo uma análise eficaz do desempenho de vendas e a tomada de decisões baseadas em dados.

## 📁 Estrutura do Repositório

```
dashboard-vendas-xbox-game-pass/
│
├── data/
│   ├── base.xlsx                      # Base de dados bruta
│   └── dashboard_xbox_finalizado.xlsx # Dashboard completo
│
├── README.md                          # Documentação do projeto
└── LICENSE                            # Licença MIT
```

## 📊 Sobre os Dados

### Base de Dados (`base.xlsx`)

A base contém **295 registros de assinaturas** do Xbox Game Pass de janeiro a dezembro de 2024, com as seguintes informações:

#### Campos Principais:

- **Subscriber ID**: Identificador único do assinante (3231-3525)
- **Name**: Nome do assinante
- **Plan**: Tipo de plano (Ultimate, Core, Standard)
- **Start Date**: Data de início da assinatura
- **Auto Renewal**: Renovação automática (Yes/No)
- **Subscription Price**: Preço da assinatura base
- **Subscription Type**: Periodicidade (Monthly, Quarterly, Annual)

#### Add-ons Disponíveis:

- **EA Play Season Pass**: $30
- **Minecraft Season Pass**: $20

#### Descontos:

- **Coupon Value**: Valor do cupom de desconto aplicado
- **Total Value**: Valor final após descontos

### Planos e Preços

| Plano | Preço Base | Características |
|-------|------------|------------------|
| **Ultimate** | $15 | Acesso completo + EA Play + Minecraft |
| **Standard** | $10 | Acesso padrão + Season Passes opcionais |
| **Core** | $5 | Plano básico |

### Paleta de Cores Xbox

O dashboard utiliza as cores oficiais da marca Xbox:

- **Verde Principal**: `#9BC848`, `#22C55E`
- **Menus**: `#2AE6B1`, `#5BF6A8`
- **Zona Negativa**: `#E8E6E9`

## 📈 Análises Implementadas

O dashboard finalizado (`dashboard_xbox_finalizado.xlsx`) contém as seguintes análises:

### 1. Faturamento Total por Tipo de Assinatura

**Assinaturas Mensais:**
- Faturamento Total: **$3,571**
- Com auto-renovação: $747
- Sem auto-renovação: $2,824

### 2. Vendas de Add-ons

**EA Play Season Pass:**
- Total de assinaturas: **1,350**
- Disponível apenas para plano Ultimate

**Minecraft Season Pass:**
- Total de assinaturas: **1,800**
- Disponível para planos Standard e Ultimate
- Standard: 900 assinaturas
- Ultimate: 900 assinaturas

### 3. Perguntas de Negócio Respondidas

✅ **Pergunta 1**: Qual o faturamento total de vendas de planos anuais?
✅ **Pergunta 2**: Qual o faturamento total segmentado por auto-renovação?
✅ **Pergunta 3**: Total de vendas de assinaturas do EA Play Season Pass
✅ **Pergunta 4**: Total de vendas de assinaturas do Minecraft Season Pass

## 🚀 Como Reproduzir

### Pré-requisitos

- Microsoft Excel 2016 ou superior
- Conhecimento básico de tabelas dinâmicas
- Conhecimento básico de gráficos no Excel

### Passo a Passo

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/celloweb-ai/dashboard-vendas-xbox-game-pass.git
   cd dashboard-vendas-xbox-game-pass
   ```

2. **Abra a base de dados:**
   - Navegue até a pasta `data/`
   - Abra o arquivo `base.xlsx`

3. **Explore o dashboard:**
   - Abra o arquivo `dashboard_xbox_finalizado.xlsx`
   - Navegue pelas abas:
     - **Assets**: Paleta de cores e logos
     - **Bases**: Dados brutos
     - **Cálculos**: Tabelas dinâmicas e métricas
     - **Dashboard**: Visualizações finais

4. **Personalize (opcional):**
   - Modifique os dados na aba "Bases"
   - Atualize as tabelas dinâmicas (Dados → Atualizar Tudo)
   - Os gráficos serão atualizados automaticamente

## 🛠️ Tecnologias Utilizadas

- **Microsoft Excel**: Ferramenta principal
- **Tabelas Dinâmicas**: Análise e agregação de dados
- **Gráficos Dinâmicos**: Visualizações interativas
- **Formatação Condicional**: Destaque de informações relevantes

## 📚 Aprendizados

Este projeto demonstra competências em:

- ✅ Organização e estruturação de dados
- ✅ Análise exploratória de dados (EDA)
- ✅ Criação de dashboards visuais
- ✅ Uso de tabelas dinâmicas para análise
- ✅ Design de informação e UX de dashboards
- ✅ Documentação técnica de projetos

## 🤝 Contribuindo

Contribuições são bem-vindas! Para contribuir:

1. Faça um fork do projeto
2. Crie uma branch para sua feature (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add: nova análise de dados'`)
4. Push para a branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👤 Autor

**Marcus Vasconcellos**

- GitHub: [@celloweb-ai](https://github.com/celloweb-ai)
- LinkedIn: [marcusvasconcellos](https://www.linkedin.com/in/marcusvasconcellos)
- Email: marcus@vasconcellos.net.br

## 🎓 Projeto Desenvolvido

Projeto desenvolvido como parte do bootcamp **DIO - CAIXA - Artificial Intelligence in Practice**.

---

⭐ Se este projeto foi útil para você, considere dar uma estrela!

📫 Sugestões e feedback são sempre bem-vindos!