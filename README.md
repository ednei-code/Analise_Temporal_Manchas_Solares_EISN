Este projeto é um estudo aprofundado de análise de séries temporais aplicado ao Número Estimado de Manchas Solares (EISN – Estimated International Sunspot Number), um dataset histórico fundamental para compreender a atividade solar, disponibilizado pelo SILSO / Royal Observatory of Belgium desde 1818.

O objetivo principal é demonstrar um fluxo completo de análise e modelagem de séries temporais, cobrindo desde a exploração inicial dos dados até a aplicação de modelos preditivos avançados.

Metodologias e Análises Realizadas:
Pré-processamento e Limpeza de Dados: Carregamento robusto de dados, tratamento de colunas e criação de um índice de tempo (datetime).
Análise Exploratória de Séries Temporais (ETS):
Visualização da série em diferentes granularidades (diária, mensal, anual) para identificar padrões de longo prazo e ciclos solares de ~11 anos.
Análise da distribuição dos valores de manchas solares e identificação de picos de atividade.
Heatmaps para visualizar a variação da atividade solar ao longo dos anos e meses.
Aplicação de Média Móvel (Rolling Mean) para suavização da série e melhor evidência dos ciclos solares.
Decomposição STL (Seasonal-Trend decomposition using Loess): Separação da série em componentes de Tendência, Sazonalidade (ciclo solar médio) e Resíduos para uma compreensão detalhada de suas dinâmicas.
Análise Comparativa por Década: Uso de Boxplots para comparar a distribuição e intensidade das manchas solares em diferentes períodos históricos.
Modelagem Preditiva de Séries Temporais:
Modelo ARIMA (Autoregressive Integrated Moving Average): Aplicação de um modelo ARIMA(1,1,1) após testes de estacionariedade (ADF) e análise de funções de autocorrelação (ACF e PACF). Avaliação do modelo e suas limitações para prever ciclos de longo prazo.
Modelo LSTM (Long Short-Term Memory) com Keras/TensorFlow: Implementação de uma rede neural recorrente LSTM para previsão. Inclui preparação de dados (escalonamento MinMaxScaler, criação de janelas temporais), treinamento do modelo e avaliação de desempenho (RMSE, MAE). Demonstração de previsão multi-passos.
Impacto e Conclusão:
Este projeto ilustra como técnicas clássicas e modernas de análise de séries temporais podem ser empregadas para desvendar e prever fenômenos complexos, como a atividade solar. Ele destaca tanto os pontos fortes quanto as limitações de diferentes modelos na captura de características específicas de séries temporais cíclicas, fornecendo insights valiosos sobre a dinâmica do Sol ao longo de mais de dois séculos.

