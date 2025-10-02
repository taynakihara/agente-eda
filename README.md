# 🤖 Agente de Análise de Dados

## 🔗 Acesse agora
**App online:** https://agente-eda-taynakihara.streamlit.app/  
> Basta abrir o link e enviar um arquivo **.csv**. É necessário gerar uma chave de API de uma LLM para que tenha acesso a Interação com a IA.

## 📝 Sobre
Aplicação **Streamlit** para análise exploratória automatizada de **qualquer CSV**, para insights sob demanda.

## ✨ Funcionalidades
- **Visão geral**: linhas, colunas, memória, tipos de dados, estatísticas.
- **Distribuições**: histogramas (numéricas) e barras (categóricas).
- **Correlação**: matriz + ranking de correlações.
- **Tendências**: detecção de coluna temporal e séries.
- **Anomalias**: outliers via IQR + boxplots.
- **Consulta IA**: perguntas sobre o dataset com contexto automático.

## 🛠️ Executar localmente
**Pré-requisitos**
- Python 3.10+ (recomendado)
- `pip`

**Instalação**
```bash
git clone https://github.com/taynakihara/agente-eda.git
cd agente-eda
pip install -r requirements.txt
```

**Rodar**
```bash
# Versão avançada (a usada no deploy)
streamlit run app_groq_advanced.py

# (Opcional) Versão básica, se existir
# streamlit run app.py
```

> Se quiser rodar com sua própria chave localmente, crie o arquivo `.streamlit/secrets.toml`:
> ```toml
> GROQ_API_KEY = "sua_chave_aqui"
> ```

## ☁️ Deploy no Streamlit Cloud (para quem for clonar)
1. Faça **fork** deste repositório.
2. Em **share.streamlit.io → Create app** selecione o repo forkeado.
3. Defina:
   - **Branch**: `main`  
   - **Main file**: `app_groq_advanced.py`
4. Em **Settings → Secrets**, adicione:
   ```toml
   GROQ_API_KEY = "sua_chave_de_api"
   ```
5. Salve e aguarde o deploy.

## 📂 Estrutura (principal)
```
agente-eda/
├── app_groq_advanced.py    # App usado no deploy
├── requirements.txt
└── README.md
```
