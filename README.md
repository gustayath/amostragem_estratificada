# 📊 Estudos em Ciência de Dados: Amostragem Estratificada

[![GitHub license](https://img.shields.io/github/license/gustayath/amostragem_estratificada?color=blue)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/gustayath/amostragem_estratificada)](https://github.com/gustayath/amostragem_estratificada/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/gustayath/amostragem_estratificada)](https://github.com/gustayath/amostragem_estratificada/issues)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Gustavo%20Yath-0A66C2?style=flat&logo=linkedin)](https://www.linkedin.com/in/gustavoyath)

> 🎓 **Projeto Acadêmico / Estudos Pessoais:** Repositório dedicado ao estudo, implementação e consolidação de conceitos teóricos e práticos sobre a técnica de **Amostragem Aleatória Estratificada** aplicada à Ciência de Dados.

---

## 🎯 Objetivo dos Estudos

No fluxo de trabalho de um **Cientista de Dados**, a coleta e a seleção representativa de dados são etapas cruciais para evitar vieses em modelos estatísticos e de *Machine Learning*. 

Este projeto tem como objetivo principal **aprofundar os conhecimentos em Estatística Amostral**, desenvolvendo na prática scripts e análises para compreender:
1. Como funcionam os algoritmos de divisão por estratos.
2. A matemática por trás do cálculo e da alocação do tamanho amostral.
3. Como garantir a representatividade da população original ao reduzir a massa de dados para treino/teste.

---

## 📖 O que é Amostragem Estratificada?

A **Amostragem Estratificada** é um método probabilístico em que a população total é dividida em subgrupos mutuamente exclusivos e homogêneos chamados **estratos** (ex.: por faixa etária, gênero, região geográfica ou classe socioeconômica). Em seguida, amostras aleatórias são extraídas de cada estrato.

### 💡 Por que este conceito é vital para Ciência de Dados?
- **Preservação de Proporções:** Evita o *under-representation* (sub-representação) de categorias minoritárias em datasets desbalanceados.
- **Divisão Treino/Teste:** Garante que subgrupos cruciais apareçam tanto nos dados de treino quanto nos de validação.
- **Redução de Variância:** Melhora a precisão de estimadores populacionais em comparação à Amostragem Aleatória Simples (AAS).

---

## 🧮 Conceitos Estatísticos Explorados

Durante o desenvolvimento deste repositório, foram abordados diferentes métodos de alocação de amostras:

1. **Alocação Proporcional:**
   - Mantém exatamente a mesma proporção de cada classe/estrato que existe na população original.
   - Fórmula: $n_h = n \cdot \left(\frac{N_h}{N}\right)$

2. **Alocação Uniforme (Igualitária):**
   - Extrai a mesma quantidade fixa de elementos de cada estrato, independentemente do seu tamanho original.
   - Fórmula: $n_h = \frac{n}{H}$

3. **Alocação Ótima (Neyman):**
   - Otimiza a amostragem levando em consideração a variabilidade (desvio padrão) dentro de cada estrato.
   - Fórmula: $n_h = n \cdot \frac{N_h \cdot S_h}{\sum (N_k \cdot S_k)}$

---

## 🛠️ Tecnologias e Ferramentas

Como parte do aprendizado prático em **Python para Data Science**, as seguintes ferramentas foram utilizadas/estudadas:

* **Python 3.14**
* **Pandas:** Manipulação de DataFrames e agregação por estratos.
* **NumPy:** Vetorização e cálculos estatísticos.
* **Scikit-Learn:** Aplicação de `train_test_split` com o parâmetro `stratify`.
* **Jupyter Notebooks:** Documentação passo a passo dos experimentos e validações.

---

## 🚀 Como Executar o Projeto Localmente

```bash
# 1. Clone o repositório
git clone [https://github.com/gustayath/amostragem_estratificada.git](https://github.com/gustayath/amostragem_estratificada.git)

# 2. Acesse a pasta do projeto
cd amostragem_estratificada

# 3. Instale as dependências para reproduzir os testes
pip install pandas numpy scikit-learn jupyter

```

---

## 📁 Estrutura de Estudos no Repositório

```text
amostragem_estratificada/
├── data/              # Datasets sintéticos e reais para teste de amostragem
├── notebooks/         # Análises explicativas e experimentos passo a passo
├── src/               # Funções reutilizáveis criadas durante os estudos
├── .gitignore
├── LICENSE
└── README.md

```

---

## 💬 Feedback e Conexão

Estou constantemente aprendendo e aprimorando minhas habilidades em Ciência de Dados e Estatística. Críticas construtivas, sugestões de melhoria no código ou novas abordagens teóricas são muito bem-vindas!

* **Autor:** Gustavo Yath
* **LinkedIn:** [linkedin.com/in/gustavoyath](https://www.linkedin.com/in/gustavoyath)
* **GitHub:** [@gustayath](https://www.google.com/search?q=https://github.com/gustayath)

---

## 📄 Licença

Este repositório está sob a licença **MIT** — sinta-se à vontade para utilizar o código para seus próprios estudos. Veja o arquivo [LICENSE](https://www.google.com/search?q=LICENSE) para mais detalhes.

```

```
