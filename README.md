# 🔍 Análise da População Prisional de Minas Gerais (2017-2024)

## 📌 Visão Geral

Este projeto apresenta uma **análise exploratória detalhada da população prisional do estado de Minas Gerais** no período de 2017 a junho de 2024, com foco em características demográficas e socioeducacionais.

A análise investiga padrões e tendências na composição da população carcerária, identificando disparidades de gênero, perfil educacional e distribuição geográfica nas unidades prisionais de MG.

---

## 🎯 Perguntas de Pesquisa

Este projeto foi desenvolvido para responder às seguintes questões:

- Como evoluiu a população prisional ao longo dos 7 anos analisados?
- Qual é a distribuição por sexo na população carcerária de MG?
- Qual é o nível de escolaridade predominante entre os presos?
- Quais são as disparidades socioeducacionais na população prisional?

---

## 📊 Dataset

| Aspecto | Descrição |
|--------|-----------|
| **Origem** | Dados abertos - Secretaria de Estado de Justiça e Segurança Pública (SEJUSP) de Minas Gerais |
| **Período** | Janeiro de 2017 a Junho de 2024 (7 anos e 6 meses) |
| **Total de Registros** | 284.627 registros após limpeza |
| **Unidades Prisionais** | 268 estabelecimentos prisionais mapeados |
| **Municípios Cobertos** | 188 municípios do estado de MG |
| **Regionalizações** | 19 RISP (Regiões Integradas de Segurança Pública) |

### 📋 Variáveis Principais

- **Características Demográficas**: Sexo na admissão
- **Características Educacionais**: Nível de escolaridade na admissão (9 categorias)
- **Localização**: Município, RISP, estabelecimento prisional
- **Temporal**: Ano e mês da admissão
- **Contagem**: Quantidade de pessoas por categoria

---

## 🔧 Metodologia

### 1️⃣ **Importação e Exploração Inicial**
   - Carregamento de dados em formato Excel
   - Verificação de dimensões e estrutura
   - Identificação de tipos de dados

### 2️⃣ **Limpeza de Dados**
   - Remoção de registros duplicados e inconsistentes
   - Tratamento de valores ausentes
   - Padronização de nomes de colunas
   - **Resultado**: Redução de 328.773 para 284.627 registros

### 3️⃣ **Detecção e Tratamento de Outliers**
   - Identificação de valores extremos nas variáveis numéricas
   - Remoção de outliers significativos (67.882 em sexo, 28.777 em escolaridade)
   - Validação de integridade dos dados

### 4️⃣ **Análise Exploratória (EDA)**
   - Estatísticas descritivas por variável
   - Distribuições de frequência
   - Análise temporal (tendências por ano)
   - Tabulações cruzadas (instituição × escolaridade)

### 5️⃣ **Visualizações**
   - Gráficos de barras para distribuição de escolaridade
   - Análises de composição por sexo
   - Representação geográfica por RISP

### 6️⃣ **Interpretação e Insights**
   - Síntese de padrões identificados
   - Discussão de implicações sociais
   - Conexões com contexto nacional

---

## 📈 Principais Insights

### 🔴 **Escolaridade Predominante**

Os dados revelam uma concentração significativa nos **níveis mais baixos de escolaridade**:

- **1º Grau Incompleto**: 51.110 registros (maior concentração)
- **Analfabeto / Semi-Alfabetizado**: Representação significativa
- **Nível superior**: Representação mínima

**Insight**: Os níveis mais baixos de escolaridade concentram a maior parte da população prisional, sugerindo uma possível relação entre **baixa escolaridade e vulnerabilidade social**, alinhado com pesquisas sobre determinantes sociais da criminalidade.

### 🔴 **Disparidade de Gênero**

A população prisional é **predominantemente masculina**:

- **Sexo Masculino**: 253.692 registros (89%)
- **Sexo Feminino**: Participação significativamente menor

**Insight**: Existe uma forte **desigualdade de gênero no sistema prisional**, comportamento consistente com dados nacionais e internacionais que indicam maior incidência de criminalidade e encarceramento de homens.

### 🔴 **Distribuição Geográfica**

- **Penitenciária Prof. Aluízio Ignácio de Oliveira** (Ribeirão das Neves): Maior volume de presos
- **Distribuição**: Concentração em regiões metropolitanas (especialmente 01ª RISP - Belo Horizonte)
- **19 RISP mapeadas** em todo o estado

### 🔴 **Período Analisado: 2017-2024**

- Dados abrangem período de mudanças significativas na segurança pública estadual
- Permite análise de tendências e oscilações na população carcerária
- Cobre período pré e pós-reforma na gestão penitenciária

---

## 💻 Tecnologias Utilizadas

```
🐍 Python 3
📊 Pandas - Manipulação, limpeza e transformação de dados
📈 NumPy - Operações numéricas e estatísticas
📉 Matplotlib & Seaborn - Visualizações gráficas profissionais
🔗 Google Colab - Ambiente de desenvolvimento e análise
```

---

## 🚀 Como Reproduzir

### Pré-requisitos
```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### Dados
Carregue o arquivo Excel com dados da SEJUSP-MG:
```python
df = pd.read_excel('Dados_Abertos_Pop_Pris_Sexo_Escolaridade_Jan_2017_Jun_2024.xlsx')
```

### Execução
1. Importe e explore os dados
2. Execute limpeza e tratamento de outliers
3. Padronize variáveis categóricas
4. Gere análises exploratórias
5. Crie visualizações
6. Sintetize insights

---

## 📁 Estrutura do Projeto

```
📦 analise-populacao-prisional-mg/
├── 📓 analise_populacaoprisionalMG_2017_2024.ipynb    # Notebook principal
├── 📄 README.md                                        # Este arquivo
├── 📊 dados_brutos.xlsx                               # Dataset original
└── 💾 dados_limpos.csv                                # Dataset tratado
```

---

## 🎓 Competências Demonstradas

- ✅ **Análise Exploratória Avançada (EDA)**: Investigação sistemática de datasets reais com múltiplas dimensões
- ✅ **Limpeza de Dados**: Tratamento rigoroso de inconsistências, duplicatas e outliers (redução de 14% de registros)
- ✅ **Análise Estatística**: Estatísticas descritivas, distribuições, identificação de padrões
- ✅ **Visualização de Dados**: Comunicação clara de insights complexos através de gráficos
- ✅ **Pensamento Crítico**: Interpretação de dados com consciência de implicações sociais
- ✅ **Documentação**: Código limpo, comentado e reprodutível
- ✅ **Análise Social**: Conexão entre dados e contexto de segurança pública

---

## 📚 Contexto

- **Realizado em**: Fevereiro de 2026
- **Dados**: Dados públicos SEJUSP-MG (2017-2024)
- **Propósito**: Projeto pessoal de análise exploratória
- **Autora**: Danielli Meilene Coutinho Arçari

---

## 🔗 Links Relacionados

- 💼 [LinkedIn](https://www.linkedin.com/in/danielli-arcari/)
- 🌐 [Portfólio Completo](https://danielli-arcari.github.io/)
- 📧 **Email**: axiadmc@gmail.com
- 💻 [GitHub](https://github.com/danielli-arcari)
- 📊 [Notebook (Google Colab)](https://colab.research.google.com/drive/1ESr8ZIiVcNlW785A_7c3kQjfPLPLXbCu?usp=sharing)

---

## 💡 Possíveis Extensões Futuras

- 📊 **Análise Temporal**: Série temporal da população carcerária (2017-2024)
- 🗺️ **Análise Geoespacial**: Mapeamento de unidades prisionais e densidade por região
- 🤖 **Modelagem Preditiva**: Previsão de tendências futuras na população carcerária
- 👥 **Análise de Interseccionalidade**: Cruzamento de múltiplas variáveis (gênero × escolaridade × região)
- 📈 **Benchmark Estadual**: Comparação com outros estados brasileiros
- 🎓 **Impacto de Políticas**: Análise de efeito de políticas de segurança específicas

---

## 📖 Observações Importantes

Este projeto utiliza **dados públicos oficiais** da Secretaria de Estado de Justiça e Segurança Pública de Minas Gerais. A análise tem caráter **exploratório e descritivo**, com objetivo de identificar padrões e tendências na população prisional.

As conclusões refletem os dados disponíveis e não devem ser generalizadas além do contexto específico do estado de Minas Gerais (2017-2024).

---

**Este projeto demonstra capacidade de executar análises exploratórias profundas em dados reais, com rigor metodológico, tratamento cuidadoso de dados e comunicação clara de insights complexos.**

*Desenvolvido com foco em qualidade, reprodutibilidade e consciência social.*
