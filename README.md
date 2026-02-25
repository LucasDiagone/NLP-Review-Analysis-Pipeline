# 🧠 NLP Review Analysis Pipeline

Pipeline completo de Processamento de Linguagem Natural (NLP) aplicado a reviews reais de e-commerce.

O projeto integra técnicas clássicas e modernas de NLP, combinando:

- 📊 Bag of Words (BoW)
- 🔢 TF-IDF
- 🧩 LDA (Topic Modeling)
- 📐 Similaridade do Cosseno
- 🤖 Regressão Logística
- 🧠 Transformers (Análise de Emoção e Sentimento)

---

## 🎯 Objetivo

Explorar diferentes abordagens de NLP para:

- Classificação de sentimento
- Detecção de emoções
- Identificação de temas (Topic Modeling)
- Busca semântica e similaridade textual
- Detecção de inconsistências entre rating e texto

O foco é demonstrar a aplicação prática de técnicas supervisionadas e não supervisionadas em dados reais.

---

## 📦 Dataset

Reviews reais de e-commerce (Mercado Livre), contendo:

- Texto da avaliação
- Nota atribuída (rating)

O rating foi utilizado como proxy para classificação supervisionada de sentimento.

O conjunto de dados foi obtido a partir do repositório público:

https://github.com/octaprice/ecommerce-product-dataset

Utilizando:

!git clone https://github.com/octaprice/ecommerce-product-dataset.git

!ls ecommerce-product-dataset/data/mercadolivre_com_br

---

## 🔎 Etapas do Projeto

### 1️⃣ Pré-processamento
- Limpeza textual
- Remoção de stopwords
- Padronização

### 2️⃣ Representação Vetorial
- Bag of Words
- TF-IDF

### 3️⃣ Análise de Emoção e Sentimento
- Modelos Transformer pré-treinados
- Classificação automática de polaridade
- Identificação de emoções específicas

### 4️⃣ Topic Modeling
- LDA (Latent Dirichlet Allocation)
- Extração de palavras-chave por tema
- Identificação do tema principal por review

### 5️⃣ Similaridade Textual
- Similaridade do cosseno
- Busca semântica
- Identificação de reviews semelhantes

### 6️⃣ Classificação Supervisionada
- Regressão Logística
- Balanceamento de classes (`class_weight="balanced"`)
- Avaliação com accuracy, precision, recall e F1-score
  
Foi utilizada a configuração `class_weight="balanced"` na Regressão Logística para compensar o desbalanceamento entre as classes (negativo, neutro e positivo), ajustando automaticamente o peso das classes minoritárias durante o treinamento.

---

## 📊 Resultados

- Acurácia aproximada de **86%** na classificação de sentimento.
- Melhor desempenho na classe majoritária (positiva).
- Impacto observado do desbalanceamento nas classes minoritárias.

---

## 🧠 Tecnologias Utilizadas

- Python
- Pandas
- Scikit-learn
- NLTK
- Transformers (Hugging Face)

---

## 🚀 Possíveis Melhorias

- Ajuste de hiperparâmetros
- Técnicas avançadas de balanceamento
- Comparação entre modelos clássicos e modelos baseados em embeddings
- Fine-tuning de modelos Transformer

---

## 📌 Conclusão

Este projeto consolida meus estudos em NLP por meio da aplicação prática em dados reais de reviews de e-commerce, integrando técnicas clássicas (BoW, TF-IDF, LDA e Regressão Logística) e modelos baseados em Transformers.

O trabalho demonstra a construção de um pipeline completo de análise textual, com foco em interpretação, avaliação crítica e aplicação real.

📎 Mais conteúdos e projetos:

- Medium: https://medium.com/@lucas.diagone  
- GitHub: https://github.com/LucasDiagone
