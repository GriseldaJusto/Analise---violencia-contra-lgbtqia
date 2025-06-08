# 📊 Análise da Violência Contra Pessoas LGBTQIA+ no Brasil

**Repositório oficial do projeto final do curso de Inteligencia Artificial organizado por PertaLabs**  
Grupo: Análise da violência contra a população LGBTQIA+ utilizando dados do Grupo Gay da Bahia (GGB)

🔗 Repositório no GitHub: [GriseldaJusto/Analise---violencia-contra-lgbtqia](https://github.com/GriseldaJusto/Analise---violencia-contra-lgbtqia)  
📄 Fonte dos dados: [Base dos Dados - Relatório de Violência LGBTQIA+ (GGB)](https://basedosdados.org/dataset/f83a600b-4aa5-4386-bc21-f5f6859e9605?table=b246fc07-f9a2-451b-a02c-8f0301682e99)

---

## 🏳️‍🌈 Contexto

O Brasil lidera rankings mundiais de violência contra pessoas LGBTQIA+. A análise utiliza dados anuais do **Grupo Gay da Bahia**, uma das instituições mais antigas de defesa dos direitos LGBTQIA+ no país. O objetivo é compreender padrões territoriais e demográficos nos registros de assassinatos dessa população.

---

## ❓ Perguntas Orientadoras

1. **Quais estados têm as maiores taxas de violência contra a população LGBTQIA+?**
2. **Há padrões sazonais ou demográficos (idade, raça ou identidade de gênero) nos crimes?**

---

## ⚙️ Metodologia

- Para a análise, os arquivos CSV foram previamente baixados da plataforma e carregados localmente no ambiente de desenvolvimento (Google Colab).
- Foi realizado o tratamento dos dados com `pandas`, incluindo remoção de nulos e padronização de colunas.
- Foram geradas visualizações com `seaborn` e `matplotlib` para responder às perguntas orientadoras.
- Utilizamos gráficos de barras para destacar:
  - Estados com mais homicídios
  - Raça/cor das vítimas
  - Identidade de gênero

---

## Análise com Machine Learning: Previsão de Risco

Neste projeto, foi explorada uma aplicação inicial de Machine Learning para prever o número de homicídios com base em atributos demográficos, utilizando o dataset por raça/cor (`df_raca`).

### Metodologia

- O conjunto de dados foi preparado transformando a variável categórica `raca_cor` em variáveis dummy (one-hot encoding).
- A variável alvo (`y`) foi o número de homicídios, e as variáveis explicativas (`X`) foram as colunas resultantes da codificação das raças.
- O modelo escolhido foi o **Random Forest Regressor**, um algoritmo robusto para regressão baseado em múltiplas árvores de decisão.
- O conjunto de dados foi dividido em treino e teste (`random_state=42` para reprodutibilidade).
- O modelo foi treinado no conjunto de treino e avaliado no conjunto de teste.

### Resultados

- O desempenho do modelo foi medido pelo **Erro Médio Absoluto (MAE)**, que indica a média do desvio absoluto entre os valores previstos e reais.
- Um gráfico de densidade (KDE plot) foi gerado para comparar visualmente a distribuição dos valores reais e previstos, utilizando uma paleta de cores suaves e estilo clean para facilitar a interpretação.

---

## 👥 Integrantes do Grupo

|        Nome         |                       GitHub                       |
|---------------------|----------------------------------------------------|
| Griselda Justo      | [@GriseldaJusto](https://github.com/GriseldaJusto) |
| Camille             | [@GriseldaJusto](https://github.com/GriseldaJusto) |
| Priscila Estevao    | [@GriseldaJusto](https://github.com/GriseldaJusto) |
| Amanda Amani        | [@GriseldaJusto](https://github.com/GriseldaJusto) |
| Manuela Oliveira    | [@GriseldaJusto](https://github.com/GriseldaJusto) |
| Raysa Leide         | [@GriseldaJusto](https://github.com/GriseldaJusto) |




