# 📊 Dashboard de Vendas Xbox Game Pass

![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
![Status](https://img.shields.io/badge/Status-Conclu%C3%ADdo-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

Dashboard interativo desenvolvido em Excel para análise de vendas e desempenho de assinaturas do Xbox Game Pass. Projeto realizado como parte do desafio do bootcamp DIO/CAIXA de Inteligência Artificial na Prática.

## 🎯 Objetivo

Transformar dados brutos de assinaturas em visualizações claras e informativas, permitindo análise eficaz do desempenho de vendas e tomada de decisões baseadas em dados.

## 📁 Estrutura do Repositório

```
├── README.md                          # Documentação do projeto
├── base.xlsx                          # Dados brutos de assinaturas
├── dashboard_xbox_finalizado.xlsx     # Dashboard completo com visualizações
└── LICENSE                            # Licença MIT
```

## 📊 Dados Utilizados

### Base de Dados

O arquivo `base.xlsx` contém **295 registros** de assinaturas do Xbox Game Pass de **janeiro a dezembro de 2024**, incluindo:

#### Campos Principais

- **Subscriber ID**: Identificador único do assinante (3231-3525)
- **Name**: Nome do assinante
- **Plan**: Tipo de plano (Ultimate, Core, Standard)
- **Start Date**: Data de início da assinatura
- **Auto Renewal**: Renovação automática (Yes/No)
- **Subscription Price**: Preço base da assinatura
- **Subscription Type**: Periodicidade (Monthly, Quarterly, Annual)

#### Add-ons Disponíveis

- **EA Play Season Pass**: $30
- **Minecraft Season Pass**: $20
- **Coupon Value**: Descontos aplicados
- **Total Value**: Valor total após add-ons e descontos

### Planos de Assinatura

| Plano | Preço Base | Características |
|-------|------------|----------------|
| **Ultimate** | $15/mês | Acesso completo + EA Play + Minecraft |
| **Core** | $5/mês | Acesso básico |
| **Standard** | $10/mês | Acesso intermediário + add-ons opcionais |

## 📈 Análises Implementadas

### Perguntas de Negócio Respondidas

1. **Faturamento Total por Tipo de Assinatura**
   - Análise de receita mensal: **$3,571**
   - Segmentação por tipo de plano
   - Identificação de planos mais rentáveis

2. **Faturamento por Auto-Renovação**
   - Com auto-renovação: **$747**
   - Sem auto-renovação: **$2,824**
   - Análise de retenção de clientes

3. **Total de Vendas EA Play Season Pass**
   - **1,350 assinaturas vendidas**
   - Exclusivamente para plano Ultimate
   - Receita adicional significativa

4. **Total de Vendas Minecraft Season Pass**
   - **1,800 assinaturas vendidas**
   - Distribuição: 900 Standard + 900 Ultimate
   - Add-on mais popular

## 🎨 Design e Visualização

### Paleta de Cores Xbox

O dashboard utiliza a identidade visual oficial do Xbox:

- **Verde Xbox Principal**: `#9BC848`, `#22C55E`
- **Verde Menus**: `#2AE6B1`, `#5BF6A8`
- **Zona Negativa**: `#E8E6E9`

### Componentes do Dashboard

- **Gráficos de Barra**: Comparação de faturamento por plano
- **Gráficos de Pizza**: Distribuição de tipos de assinatura
- **Tabelas Dinâmicas**: Análise detalhada de métricas
- **Indicadores KPI**: Valores totais e médias
- **Filtros Interativos**: Segmentação por período e plano

## 🚀 Como Usar

### Pré-requisitos

- Microsoft Excel 2016 ou superior
- Conhecimentos básicos de navegação em planilhas

### Instruções

1. **Clone o repositório**
   ```bash
   git clone https://github.com/celloweb-ai/dashboard-vendas-xbox-game-pass.git
   ```

2. **Abra o arquivo do dashboard**
   - Navegue até `dashboard_xbox_finalizado.xlsx`
   - Abra com Microsoft Excel

3. **Explore as visualizações**
   - Navegue pelas abas: Assets, Bases, Cálculos, Dashboard
   - Utilize os filtros para análises específicas
   - Interaja com os gráficos para detalhes

4. **Consulte os dados brutos**
   - Abra `base.xlsx` para visualizar os dados originais
   - Útil para validações e análises customizadas

## 📂 Descrição das Planilhas

### base.xlsx

- **Assets**: Paleta de cores, logos e ícones
- **Bases**: Dados brutos (295 registros de assinaturas)
- **Cálculos**: Fórmulas e tabelas auxiliares (não incluído na versão base)
- **Dashboard**: Área de visualização (não incluído na versão base)

### dashboard_xbox_finalizado.xlsx

- **Assets**: Elementos visuais e identidade Xbox
- **Bases**: Dados processados e formatados
- **Cálculos**: Análises e perguntas de negócio respondidas
- **Dashboard**: Visualizações finalizadas e formatadas

## 🛠️ Tecnologias e Ferramentas

- **Microsoft Excel**: Desenvolvimento do dashboard
- **Tabelas Dinâmicas**: Agregação e análise de dados
- **Gráficos Excel**: Visualizações interativas
- **Fórmulas Avançadas**: SOMA, SE, SOMASE, tabelas de referência
- **Formatação Condicional**: Destaque de métricas importantes

## 📊 Principais Insights

### Análise de Receita

- Assinaturas **sem auto-renovação** geram **3,8x mais receita** ($2,824 vs $747)
- Plano **Ultimate** é o mais popular entre assinantes de add-ons
- **Minecraft Season Pass** supera EA Play em 33% nas vendas

### Comportamento do Cliente

- Periodicidade mensal predomina nos dados
- Add-ons aumentam significativamente o ticket médio
- Cupons de desconto variam de $1 a $20

### Oportunidades Identificadas

- Potencial para aumentar taxa de auto-renovação
- Bundles de add-ons podem maximizar receita
- Campanhas específicas por tipo de plano

## 🎓 Aprendizados do Projeto

- Organização e estruturação de dados para análise
- Criação de dashboards profissionais em Excel
- Aplicação de identidade visual em relatórios
- Análise de perguntas de negócio com dados reais
- Documentação técnica de projetos de dados

## 📝 Notas Técnicas

### Tratamento de Dados

- Campos vazios em add-ons representados por "-"
- Datas no formato YYYY-MM-DD
- Valores monetários sem símbolo de moeda
- Identificadores sequenciais de assinantes

### Cálculos Principais

```excel
# Faturamento por Auto-Renovação
=SOMASE(Bases[Auto Renewal], "Yes", Bases[Total Value])

# Total de EA Play vendidos
=CONT.SE(Bases[EA Play Season Pass], "Yes")

# Valor médio por assinatura
=MÉDIA(Bases[Total Value])
```

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:

- Reportar bugs
- Sugerir novas análises
- Melhorar a documentação
- Propor otimizações no dashboard

### Como Contribuir

1. Fork o projeto
2. Crie uma branch para sua feature (`git checkout -b feature/NovaAnalise`)
3. Commit suas mudanças (`git commit -m 'Adiciona nova análise X'`)
4. Push para a branch (`git push origin feature/NovaAnalise`)
5. Abra um Pull Request

## 📜 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

## 👨‍💻 Autor

**Marcus Vasconcellos**

- GitHub: [@celloweb-ai](https://github.com/celloweb-ai)
- LinkedIn: [Marcus Vasconcellos](https://www.linkedin.com/in/marcusvasconcellos)
- Email: marcus@vasconcellos.net.br

## 🎯 Sobre o Desafio

Este projeto foi desenvolvido como parte do bootcamp **DIO/CAIXA - Inteligência Artificial na Prática**, com o objetivo de demonstrar habilidades em:

- Análise de dados
- Visualização de informações
- Resolução de problemas de negócio
- Documentação técnica
- Organização de projetos em repositórios

## 🔗 Links Úteis

- [Documentação Excel](https://support.microsoft.com/excel)
- [Boas Práticas em Dashboards](https://www.microsoft.com/en-us/microsoft-365/blog/excel/)
- [GitHub - Markdown Guide](https://guides.github.com/features/mastering-markdown/)

---

⭐ Se este projeto foi útil para você, considere dar uma estrela no repositório!

**Desenvolvido com 💚 para a comunidade de dados e Excel**