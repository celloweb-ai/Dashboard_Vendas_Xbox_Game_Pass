# 🚀 Instruções para Geração dos Arquivos Excel

Este documento contém as instruções passo a passo para gerar os arquivos Excel do Dashboard de Vendas Xbox Game Pass.

## 📚 Pré-requisitos

Antes de começar, certifique-se de ter:

- **Python 3.8 ou superior** instalado no seu sistema
- **pip** (gerenciador de pacotes Python)
- **Git** para clonar o repositório (opcional)

### Verificar instalação do Python

```bash
python --version
# ou
python3 --version
```

Deve retornar algo como: `Python 3.8.x` ou superior.

## 📥 Passo 1: Obter o Código

### Opção A: Clonar o repositório (recomendado)

```bash
git clone https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass.git
cd Dashboard_Vendas_Xbox_Game_Pass
```

### Opção B: Download direto

1. Acesse o repositório: https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass
2. Clique em **Code** > **Download ZIP**
3. Extraia o arquivo ZIP
4. Navegue até a pasta extraída via terminal

## 📦 Passo 2: Instalar Dependências

No diretório raiz do projeto, execute:

```bash
pip install -r requirements.txt
```

Ou, se estiver usando Python 3 explicitamente:

```bash
pip3 install -r requirements.txt
```

Isso instalará:
- **pandas**: Manipulação de dados
- **numpy**: Cálculos numéricos
- **openpyxl**: Criação de arquivos Excel

## ▶️ Passo 3: Executar o Script

Execute o script de geração:

```bash
python gerar_dados_xbox.py
```

Ou:

```bash
python3 gerar_dados_xbox.py
```

## ✅ O que o Script Faz

Ao executar o script, ele:

1. **Gera 295 registros** de assinaturas Xbox Game Pass com dados aleatórios mas realistas
2. **Cria dois arquivos Excel** na pasta `/data`:
   - `base.xlsx` - Base de dados bruta com todos os registros
   - `dashboard_xbox_finalizado.xlsx` - Dashboard com múltiplas abas:
     - **Assets**: Paleta de cores Xbox
     - **Bases**: Dados brutos (idêntico ao base.xlsx)
     - **Cálculos**: Análises e métricas calculadas
     - **Dashboard**: Espaço para visualizações

3. **Exibe estatísticas** no terminal:
   - Total de registros
   - Faturamento total
   - Distribuição por plano
   - Distribuição por tipo de assinatura

## 📁 Estrutura dos Dados Gerados

### Campos no `base.xlsx`:

| Campo | Descrição | Exemplo |
|-------|-------------|----------|
| **Subscriber ID** | ID único do assinante | 3231-3525 |
| **Name** | Nome do assinante | Marcus Silva |
| **Plan** | Tipo de plano | Ultimate, Standard, Core |
| **Start Date** | Data de início | 15/03/2024 |
| **Auto Renewal** | Renovação automática | Yes, No |
| **Subscription Price** | Preço base | $15, $10, $5 |
| **Subscription Type** | Periodicidade | Monthly, Quarterly, Annual |
| **EA Play Season Pass** | Add-on EA Play | $30 ou $0 |
| **Minecraft Season Pass** | Add-on Minecraft | $20 ou $0 |
| **Coupon Value** | Desconto aplicado | $0-$25 |
| **Total Value** | Valor final | Calculado |

### Planos e Preços:

- **Ultimate**: $15 - Pode ter EA Play ($30) e Minecraft ($20)
- **Standard**: $10 - Pode ter Minecraft ($20)
- **Core**: $5 - Plano básico sem add-ons

## 🛠️ Solução de Problemas

### Erro: "ModuleNotFoundError"

**Problema**: Dependência não instalada.

**Solução**:
```bash
pip install pandas numpy openpyxl
```

### Erro: "Permission denied" na pasta /data

**Problema**: Sem permissão de escrita.

**Solução**: Crie a pasta manualmente:
```bash
mkdir data
```

### Erro: "python: command not found"

**Problema**: Python não instalado ou não no PATH.

**Solução**:
- **Windows**: Baixe em https://python.org e reinstale marcando "Add to PATH"
- **Mac**: `brew install python3`
- **Linux**: `sudo apt-get install python3`

## 📊 Próximos Passos

Após gerar os arquivos:

1. Abra `dashboard_xbox_finalizado.xlsx` no Excel
2. Explore as abas:
   - **Assets**: Veja a paleta de cores
   - **Bases**: Dados brutos
   - **Cálculos**: Métricas já calculadas
   - **Dashboard**: Crie gráficos e visualizações

3. **Crie tabelas dinâmicas** usando os dados da aba "Bases"
4. **Adicione gráficos** na aba "Dashboard"
5. **Use as cores** da aba "Assets" para manter a identidade visual Xbox

## 📝 Personalização

Para modificar os dados gerados, edite o arquivo `gerar_dados_xbox.py`:

- **Linha 14-15**: Alterar seed para gerar dados diferentes
- **Linha 21-23**: Modificar nomes disponíveis
- **Linha 28**: Ajustar distribuição de planos (Ultimate, Standard, Core)
- **Linha 31**: Ajustar distribuição de tipos (Monthly, Quarterly, Annual)
- **Linha 37-39**: Modificar preços dos planos e add-ons

## ❓ Dúvidas ou Problemas

Se encontrar algum problema:

1. Verifique se todas as dependências estão instaladas
2. Confirme que a pasta `/data` existe
3. Verifique se tem permissões de escrita
4. Abra uma issue no GitHub: https://github.com/celloweb-ai/Dashboard_Vendas_Xbox_Game_Pass/issues

## 🎉 Sucesso!

Se tudo correu bem, você deve ter:
- ✅ `data/base.xlsx` criado
- ✅ `data/dashboard_xbox_finalizado.xlsx` criado
- ✅ 295 registros de assinaturas gerados
- ✅ Análises e métricas calculadas

Bom trabalho! 🎮

---

**Desenvolvido por**: Marcus Vasconcellos  
**Projeto**: DIO - CAIXA - Artificial Intelligence in Practice  
**Licença**: MIT