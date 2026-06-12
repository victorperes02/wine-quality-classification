# wine-quality-classification


Classificação da Qualidade do Vinho
Classificação da qualidade do vinho usando aprendizado profundo

Este repositório implementa um estudo comparativo de três arquiteturas de aprendizado profundo para classificação da qualidade do vinho: Redes Neurais Convolucionais (CNNs) , Redes de Memória de Longo Prazo (LSTMs) e Autoencoders . Utilizando atributos físico-químicos de conjuntos de dados de vinhos tintos e brancos, os modelos são avaliados com base em suas métricas de desempenho, como precisão, recall, pontuação F1 e acurácia.

Conjuntos de dados
Os modelos utilizam os conjuntos de dados de Qualidade do Vinho do Repositório de Aprendizado de Máquina da UCI . Os conjuntos de dados, winequality-red.csve winequality-white.csv, devem ser colocados no Data/diretório para que os scripts funcionem.

Características
CNN: Utiliza camadas convolucionais para capturar padrões espaciais nos dados.
LSTM: Explora as relações temporais nos atributos físico-químicos.
Autoencoder: Utiliza redução de dimensionalidade para extração de características e classificação.
Requisitos
Python 3.7+
Bibliotecas: pandas, numpy, torch, sklearn, seaborn, matplotlib,imblearn
Instale os pacotes Python necessários usando:

pip install -r requirements.txt
Roteiros
CNN.py: Implementa uma CNN para classificação da qualidade do vinho.
LSTM.py: Implementa uma LSTM para tarefas de classificação.
Autoencoders.py: Utiliza um Autoencoder para extração de características e um classificador secundário para previsão.
Cada roteiro inclui:
Pré-processamento de dados, incluindo balanceamento de classes com SMOTE.
Validação cruzada K-fold para avaliação robusta de desempenho.
Treinamento e avaliação de modelos.
Uso
Certifique-se de que os caminhos do conjunto de dados sejam válidos (primeira seção do código).
Execute qualquer um dos scripts:
python 1_CNN.py
python 2_LSTM.py
python 3_Autoencoders.py
Observações
As CNNs superaram outros modelos, alcançando a maior acurácia, precisão, recall e pontuação F1. As LSTMs demonstraram desempenho competitivo, evidenciando sua utilidade em tarefas de classificação. Os autoencoders apresentaram dificuldades devido à compressão de características, resultando em perda de variância entre as classes.

Conclusão
Este estudo destaca a eficácia dos modelos de aprendizagem profunda para a classificação da qualidade do vinho:

As CNNs são mais adequadas para dados tabulares estruturados. As LSTMs oferecem adaptabilidade e resultados robustos. Os autoencoders, embora úteis para redução de dimensionalidade, podem comprometer a precisão da classificação. Trabalhos futuros poderiam abordar desafios como desequilíbrio de classes e tamanho limitado do conjunto de dados, explorando técnicas avançadas de sobreamostragem e aumento de dados.
