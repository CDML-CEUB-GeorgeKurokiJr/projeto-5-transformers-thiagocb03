# Clusterização Híbrida de Projetos de P&D

## 📖 Descrição do Projeto
Este projeto foi desenvolvido com o objetivo de organizar e categorizar automaticamente uma base de projetos de P&D (Pesquisa e Desenvolvimento). Utilizando uma abordagem de **Clusterização Híbrida**, combinamos representações semânticas profundas (BERTimbau) com técnicas tradicionais de mineração de termos (TF-IDF/SVD) e reconhecimento de entidades nomeadas (NER) para criar uma taxonomia clara dos dados.

## 🎯 Objetivo de Negócio
* Automatizar a classificação de projetos para facilitar a gestão do portfólio.
* Identificar clusters estratégicos (ex: Sustentabilidade, IA, Manufatura) para apoiar a tomada de decisão.
* Aumentar a visibilidade de temas transversais que antes eram de difícil identificação.

## 🚀 Tecnologias e Ferramentas
* **Linguagem:** Python
* **NLP & Embeddings:** BERTimbau (via HuggingFace), TF-IDF, SVD.
* **Modelagem:** K-Means (Scikit-Learn).
* **Processamento:** Reconhecimento de Entidades Nomeadas (NER) personalizado.
* **Pipeline:** Integração com DataFrames (Pandas) e automação de salvamento de artefatos.

## 📊 Principais Resultados
* **Taxonomia:** Identificação de 8 clusters temáticos com alta relevância.
* **Métricas:** Modelo validado via *Silhouette Score* para otimização do número de grupos.
* **Cobertura NER:** Extração de entidades técnicas que enriquecem a interpretação dos grupos.

## 📁 Estrutura do Repositório
```text
├── data/                  # (Placeholder) Dataset original (anonimizado)
├── notebooks/             # Notebook principal com o pipeline completo
├── results/               # Artefatos exportados (CSV, JSON, .npy)
├── README.md              # Documentação do projeto
└── requirements.txt       # Dependências utilizadas
