# Predição de Sobrevivência - Titanic <br>
## Análise Completa + Machine Learning para Competição Kaggle | Accuracy: 87.6% <br>

## Visão Geral do Projeto <br>
Análise abrangente e modelagem preditiva para a competição Titanic do Kaggle, implementando pipeline completo de data science desde análise exploratória até otimização de hiperparâmetros. O projeto alcançou 87.6% de accuracy utilizando CatBoost Classifier otimizado. <br>

## Dataset e Variáveis <br>
Registros: 1,309 passageiros (891 treino + 418 teste) <br>
Features: 12 variáveis originais <br>
Target: Survived (0 = Não sobreviveu, 1 = Sobreviveu) <br>

## Dicionário de Variáveis <br>

Pclass: Classe do ticket (1ª, 2ª, 3ª classe) <br>
Sex: Gênero do passageiro <br>
Age: Idade do passageiro <br>
SibSp: Número de irmãos/cônjuges a bordo <br>
Parch: Número de pais/filhos a bordo <br>
Ticket: Número do ticket <br>
Fare: Preço da passagem <br> 
Cabin: Número da cabine <br>
Embarked: Porto de embarque (C=Cherbourg, Q=Queenstown, S=Southampton) <br> 



## Transformações Aplicadas <br>

Tamanho_Familia: Soma de SibSp + Parch <br>
Sozinho: Variável binária indicando passageiros solitários <br>
Letra_Cabine: Extração do deck da cabine (A, B, C, etc.) <br>
Titulo: Extração de títulos dos nomes (Mr, Mrs, Miss, Master, Misc) <br>
One-Hot Encoding: Variáveis categóricas transformadas em binárias <br>

## Tratamento de Dados Ausentes <br>

Age: Preenchimento com mediana <br>
Fare: Preenchimento com mediana <br>
Embarked: Preenchimento com moda <br>
Cabin: 77% valores ausentes - criada feature 'Letra_Cabine' <br>

# Análise Exploratória de Dados <br>
## Insights Principais <br>

Gênero: Mulheres tiveram maior taxa de sobrevivência <br>
Classe Social: Passageiros de 1ª classe sobreviveram mais <br>
Idade: Crianças tiveram prioridade nos botes salva-vidas <br>
Tamanho da Família: Famílias pequenas (2-4 pessoas) tiveram melhor taxa de sobrevivência <br>
Cabines: Passageiros em decks superiores (A, B, C) sobreviveram mais <br>

## Visualizações Implementadas<br>

Distribuição de sobrevivência por gênero e classe <br>
Análise de sobrevivência por tamanho da família <br>
Distribuição etária dos passageiros <br>
Taxa de sobrevivência por deck da cabine <br>

## Implementação de Machine Learning <br>
## Tecnologias Utilizadas <br>

Processamento: pandas, numpy <br>
Visualização: seaborn, matplotlib <br>
Machine Learning: scikit-learn, xgboost, catboost <br>
Otimização: GridSearchCV, RandomizedSearchCV <br>

## Modelos Avaliados <br>
13 algoritmos de classificação testados:<br>

RandomForestClassifier, BaggingClassifier, ExtraTreesClassifier<br>
MLPClassifier, XGBClassifier, CatBoostClassifier <br> 
LogisticRegression, SVC, LinearSVC <br>
DecisionTreeClassifier, GaussianNB, SGDClassifier, Perceptron <br>

## Resultados e Performance <br>
Top 3 Modelos (Accuracy) <br>

CatBoost Classifier: 86.5% → 87.6% (após otimização) <br>
Random Forest: 86.5% <br> 
Logistic Regression: 86.5% <br>

## Otimização de Hiperparâmetros (CatBoost)<br>

Divisão dos Dados <br>

Treino: 712 amostras <br>
Validação: 90 amostras <br>
Teste: 89 amostras

Competências Técnicas Demonstradas
Análise Exploratória de Dados

Visualização abrangente de padrões de sobrevivência <br>
Identificação de correlações entre variáveis <br>
Análise estatística descritiva completa <br>
Insights históricos e contextuais do desastre <br>

## Feature Engineering Avançada<br> 

Criação de variáveis familiares agregadas <br>
Extração de informações de texto (títulos, cabines) <br>
Tratamento sistemático de valores ausentes <br> 
Transformação de variáveis categóricas <br>

## Machine Learning <br>

Comparação sistemática de 13 algoritmos de classificação <br>
Otimização de hiperparâmetros com validação cruzada <br>
Estratégia de validação com holdout sets <br>
Prevenção de overfitting com early stopping <br>

## Engenharia de Software <br>

Pipeline automatizado de limpeza de dados <br>
Código modular e reutilizável <br>
Função genérica para processamento de datasets <br>
Estruturação para competição Kaggle<br>

# Pipeline de Modelagem <br>
## Pré-processamento <br>

Limpeza e tratamento de valores ausentes <br>
Feature engineering e criação de variáveis <br>
Encoding de variáveis categóricas <br>
Divisão estratificada dos dados <br> 

## Modelagem <br>

Teste inicial de 13 algoritmos diferentes <br>
Seleção dos top performers <br>
Otimização de hiperparâmetros via GridSearch <br>
Validação final com conjunto de teste <br>

Tecnologias: Python, Scikit-learn, CatBoost, XGBoost, Pandas, Seaborn <br>
Competências: Data Science, Feature Engineering, EDA, Classification, Hyperparameter Tuning <br>
