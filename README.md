# Clusterização Híbrida de Projetos de P&D

## 📖 Descrição do Projeto
Este projeto foi desenvolvido com o objetivo de organizar e categorizar automaticamente uma base de dados de projetos de P&D (Pesquisa e Desenvolvimento). Utilizando uma abordagem de **Clusterização Híbrida**, combinamos representações semânticas profundas (**BERTimbau**) com técnicas de mineração de termos (**TF-IDF/SVD**) e uma camada customizada de **Reconhecimento de Entidades Nomeadas (NER)** para criar uma taxonomia técnica e precisa dos dados.

## 💡 Diferencial Tecnológico: NER Customizado
O pipeline de extração de entidades deste projeto foi desenvolvido especificamente para o domínio técnico de Pesquisa e Desenvolvimento (P&D).

Diferente de modelos de NER genéricos — que são treinados para identificar apenas entidades básicas como "Pessoa", "Organização" ou "Local" — este modelo foi treinado para identificar **Tecnologias** e **Eixos de Inovação**. Isso permite uma análise granular e inédita do portfólio, possibilitando que identifiquemos exatamente quais tecnologias (ex: "inteligência artificial", "baterias de íons-lítio") são mais aplicadas em cada eixo estratégico da organização.

## 🎯 Objetivo de Negócio
* **Automação:** Classificação inteligente de portfólios de inovação, reduzindo o esforço manual.
* **Inteligência Estratégica:** Identificação de clusters temáticos (ex: Sustentabilidade, IA, Manufatura Avançada) para apoiar a tomada de decisão.
* **Visibilidade:** Mapeamento de temas transversais e competências técnicas ocultas nos resumos de projetos.

## 🚀 Tecnologias e Ferramentas
* **Linguagem:** Python
* **NLP & Embeddings:** BERTimbau (HuggingFace), TF-IDF, SVD.
* **Modelagem:** K-Means (Scikit-Learn).
* **Processamento de Entidades:** NER customizado (Spacy).
* **Pipeline:** Pandas para manipulação de dados e automação de artefatos.

## 📊 Principais Resultados
* **Taxonomia:** Identificação e validação de 8 clusters temáticos distintos.
* **Qualidade:** Validação estatística via *Silhouette Score* para otimização da segmentação.
* **Granularidade:** Extração de entidades técnicas (NER) que permitem o enriquecimento dos clusters e análise detalhada por domínio.

## 📁 Estrutura do Repositório
```text
├── data/                  # Dataset original (anonimizado)
├── notebooks/             # Pipeline completo (ETL, NLP, NER e Clusterização)
├── results/               # Artefatos, métricas e tabelas de entidades extraídas
├── README.md              # Documentação do projeto
└── requirements.txt       # Dependências e ambientes configurados
