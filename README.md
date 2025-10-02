# 🤖 Agente de Análise Exploratória de Dados (E.D.A.) - Versão Groq

## 📋 Descrição
Esta aplicação Streamlit é um **agente inteligente** que permite análise exploratória completa de **qualquer arquivo CSV** de forma automática e interativa, powered by **Groq AI**. A ferramenta foi desenvolvida para atender aos requisitos da atividade obrigatória do Institut d'Intelligence Artificielle Appliquée.

## 🚀 Funcionalidades Principais

### 📋 Visão Geral
- **Informações básicas** do dataset (linhas, colunas, tamanho)
- **Tipos de dados** e identificação automática
- **Estatísticas descritivas** completas
- **Detecção de valores nulos** e únicos

### 📊 Distribuições
- **Histogramas automáticos** para variáveis numéricas
- **Gráficos de barras** para variáveis categóricas
- **Visualizações com alto contraste** para excelente legibilidade
- **Filtragem automática de outliers** para melhor visualização

### 🔍 Correlações
- **Matriz de correlação** interativa com heatmap
- **Identificação automática** de correlações significativas
- **Classificação por força** da correlação (forte, moderada, fraca)
- **Análise de dependências** entre variáveis

### 📈 Tendências
- **Detecção automática** de colunas temporais
- **Análise de tendências temporais** interativa
- **Padrões em variáveis categóricas**
- **Valores mais e menos frequentes**

### ⚠️ Anomalias
- **Detecção automática de outliers** usando método IQR
- **Visualização com boxplots** de alta qualidade
- **Estatísticas detalhadas** de anomalias por variável
- **Percentuais e limites** claramente definidos

### 🤖 Consulta Inteligente com IA
- **Configurações avançadas** personalizáveis
- **Contexto automático** com estatísticas do dataset
- **Eficiência de custos** - API chamada apenas quando solicitado

## 🛠️ Como Executar Localmente

### Pré-requisitos
- Python 3.7+
- pip (gerenciador de pacotes Python)

### Instalação
1. Clone ou baixe este repositório
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```
3. Execute a aplicação:
   ```bash
   # Versão básica
   streamlit run app.py
   
   # Versão avançada com múltiplos modelos
   streamlit run app_groq_advanced.py
   ```
4. Acesse no navegador: `http://localhost:8501`

## ☁️ Deploy no Streamlit Cloud

### Passo a Passo
1. **Fork este repositório** no GitHub
2. **Acesse** [share.streamlit.io](https://share.streamlit.io)
3. **Conecte sua conta** do Streamlit Cloud ao GitHub
4. **Selecione este repositório** para deploy
5. **Configure** o arquivo principal como `app.py`
6. **Deploy automático** será realizado

### URL de Acesso
Após o deploy, sua aplicação estará disponível em:
`https://agente-eda-taynakihara.streamlit.app/`

## 🔑 Uso da API Groq

### Como Obter sua Chave
1. Acesse [console.groq.com](https://console.groq.com)
2. Faça login ou **crie uma conta gratuita**
3. Navegue até **API Keys**
4. **Crie uma nova chave** secreta
5. **Cole a chave** na interface da aplicação

### Características de Eficiência
- ✅ **Consultas sob demanda** - API chamada apenas quando solicitado
- ✅ **Contexto otimizado** - Envia apenas estatísticas relevantes
- ✅ **Controle de custos** - Usuário insere sua própria chave
- ✅ **Sem armazenamento** - Chave não é salva ou compartilhada
- ✅ **Tier gratuito generoso** - Milhares de tokens gratuitos por mês

## 📁 Estrutura dos Arquivos

```
streamlit_app/
├── app.py                    # Aplicação principal Streamlit (Groq básico)
├── app_groq_advanced.py      # Versão avançada com múltiplos modelos
├── requirements.txt          # Dependências Python (com groq)
├── README_GROQ.md           # Este arquivo
└── README.md                # README original
```

