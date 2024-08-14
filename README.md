# Desafio: Preveja os usuários com alta chance de deixar seu Streaming

Este projeto foi criado com o intuito de aprimorar habilidades em Python utilizando um modelo de Classificação. 
O objetivo neste projeto é desenvolver um modelo de classificação que seja capaz de prever se o cliente irá cancelar o serviço ou não, levando em consideração o seu perfil no streaming.

Portanto separei este projeto em 5 partes :

# Análise exploratória dos dados

- Realizei uma descrição estatística dos dados com describe().
- Verifiquei os tipos de dados com info()
- Verifiquei a quantidade de valores faltantes com isna() e sum().

![image](https://github.com/user-attachments/assets/1f60a45c-e897-4eb7-bc3b-3c719f0ae825)

# Tratamento dos Dados

- Substitui os valores “NaN” por 0, das colunas: Time_on_platform, Num_streaming_services, Churned, Avg_rating e Devices_connected. Ultilizando a função fillna().
- Dropei as linhas nulas nas colunas Gender, Subscription_type e Age. Ultilizando dropna.
- Transformei valores churned 0 e 1 por No e Yes. Ultilizando replace.
- Transformei valores floats em valores inteiros. Ultilizando astype(int).

![image](https://github.com/user-attachments/assets/c167e93a-ca3e-4490-9cba-10d910dba00d)

# Modelagem dos Dados - Regressão Logística

- Defini as variáveis x e y para o modelo de Regressão Logística.
- Separei em train e test do modelo de Regressão Logística.
- Realizei o .fit do modelo de Regressão Logística.
- Realizar a modelagem com score.
- Plotar matrix confusão com predict e ConfusionMatrixDisplay.
- Printar as métricas com classification_report.

![image](https://github.com/user-attachments/assets/88ab79bb-30bc-4952-9479-03de32263751)


# Modelagem dos Dados - Tunning

- Definir variáveis x e y para o modelo de Tunning.
- Separar em train e test do modelo de Tunning.
- Realizar o .fit do modelo de Tunning.
- Realizar a modelagem com predict.
- Plotar matrix confusão com ConfusionMatrixDisplay.
- Printei as métricas com classification_report.

![image](https://github.com/user-attachments/assets/9c192aa0-dfcb-40a4-968e-e2b41662ce2f)


# Modelagem dos Dados - Random Forest

- Realizei a montagem do grid search com GridSearchCV.
- Realizar o .fit do modelo com RandomForestClassifier.
- Realizar o Tunning com get_params.
- Realizar a modelagem com predict.
- Plotar matrix confusão com ConfusionMatrixDisplay.
- Printar métricas com fillna.

![image](https://github.com/user-attachments/assets/0a7e8b98-691b-4cfb-a076-cd7c661c6048)
