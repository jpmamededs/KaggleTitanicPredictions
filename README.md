# 🚢 Titanic Survival Prediction

<div align="center">
  <img src="https://www.kaggle.com/static/images/site-logo.svg" alt="Kaggle Logo" width="300"/>
</div>

## 📋 Sobre o Projeto

Este projeto é uma solução para a competição clássica do Kaggle: **Titanic - Machine Learning from Disaster**. O objetivo é prever quais passageiros sobreviveram ao naufrágio do Titanic usando técnicas de Machine Learning.

🔗 [Link para a Competição](https://www.kaggle.com/c/titanic)

## 🎯 Objetivo

Construir um modelo preditivo que responda à pergunta: "Que tipo de pessoa tinha mais chances de sobreviver?" usando dados de passageiros como nome, idade, sexo, classe socioeconômica, etc.

## 📊 Dataset

O dataset contém informações sobre os passageiros do Titanic, incluindo:

- **PassengerId**: Identificador único do passageiro
- **Survived**: Sobrevivência (0 = Não, 1 = Sim) - *Target Variable*
- **Pclass**: Classe do bilhete (1, 2 ou 3)
- **Name**: Nome do passageiro
- **Sex**: Sexo
- **Age**: Idade
- **SibSp**: Número de irmãos/cônjuges a bordo
- **Parch**: Número de pais/filhos a bordo
- **Ticket**: Número do bilhete
- **Fare**: Tarifa paga
- **Cabin**: Número da cabine
- **Embarked**: Porto de embarque (C = Cherbourg, Q = Queenstown, S = Southampton)

### Arquivos de Dados

```
data/
├── train.csv              # Dados de treino
├── test.csv               # Dados de teste
└── gender_submission.csv  # Exemplo de submissão
```

## 🛠️ Tecnologias Utilizadas

- **Python 3**
- **Pandas** - Manipulação de dados
- **NumPy** - Operações numéricas
- **Matplotlib & Seaborn** - Visualização de dados
- **Scikit-learn** - Machine Learning
  - Logistic Regression
  - Random Forest Classifier
  - Train/Test Split
  - Cross-Validation

## 📁 Estrutura do Projeto

```
kaggle_titanic/
├── data/
│   ├── train.csv
│   ├── test.csv
│   └── gender_submission.csv
├── titanicNb.ipynb        # Notebook principal
└── README.md
```

## 🔍 Etapas do Projeto

### 1. **Análise Exploratória de Dados (EDA)**
   - Análise da distribuição de sobreviventes
   - Análise de sobrevivência por gênero
   - Análise de sobrevivência por classe
   - Visualizações com Seaborn

### 2. **Feature Engineering**
   - Preenchimento de valores faltantes (Age, Embarked, Fare)
   - Extração de títulos dos nomes (Mr, Miss, Mrs, Master, etc.)
   - Criação de novas features

### 3. **Pré-processamento**
   - Codificação de variáveis categóricas (Sex, Embarked)
   - Remoção de colunas não utilizadas (PassengerId, Name, Ticket, Cabin)
   - Normalização de dados

### 4. **Modelagem**
   - **Logistic Regression**
   - **Random Forest Classifier** (100 estimadores)
   - Validação cruzada (5-Fold CV)

### 5. **Avaliação**
   - Accuracy Score
   - Confusion Matrix
   - Classification Report
   - Feature Importance Analysis

## 🚀 Como Usar

1. **Clone o repositório ou baixe os arquivos**

2. **Instale as dependências:**
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Execute o notebook:**
   ```bash
   jupyter notebook titanicNb.ipynb
   ```

4. **Ou abra o notebook no VS Code** com a extensão Jupyter

## 📈 Resultados

O projeto compara dois modelos de Machine Learning:

- **Logistic Regression**: Modelo baseline
- **Random Forest**: Melhor performance

### Features Mais Importantes
O modelo Random Forest identifica as features mais relevantes para a previsão de sobrevivência.

## 📝 Próximos Passos

- [ ] Testar outros algoritmos (XGBoost, SVM, etc.)
- [ ] Realizar hyperparameter tuning
- [ ] Criar ensemble de modelos
- [ ] Gerar predições para o arquivo de teste
- [ ] Submeter resultados para o Kaggle

## 📄 Licença

Este projeto é open source e está disponível sob a licença MIT.

## 👤 Autor

Desenvolvido como parte do aprendizado de Machine Learning e participação em competições do Kaggle.

---

<div align="center">
  <p>⭐ Se este projeto foi útil, considere dar uma estrela!</p>
  <p>🚢 Happy Kaggling! 🚢</p>
</div>
