# Classificação de Timbres de Instrumentos Musicais com Machine Learning

**Projeto de Bacharelado em Engenharia Computacional** | Um pipeline completo para classificação de instrumentos musicais através de análise espectral.

## 🎯 Objetivo
Desenvolver um sistema de classificação automática que identifique 8 instrumentos musicais diferentes baseado em características espectrais do áudio.

## 📊 Fluxo de Trabalho de Dados
1. **Aquisição de Dados** - Banco de sons instrumentais
2. **Pré-processamento** - Transformada de Fourier, normalização
3. **Engenharia de Features** - Extração de características espectrais:
   - Frequências fundamentais
   - Magnitude de harmônicos
   - Energia espectral
4. **Modelagem** - Algoritmo K-Nearest Neighbors (KNN)
5. **Validação** - Métricas de acurácia e precisão

## 🛠️ Stack Tecnológico
- **Linguagem:** Python
- **Processamento de Sinais:** NumPy, SciPy
- **Machine Learning:** Scikit-learn
- **Análise de Dados:** Pandas, Matplotlib


-------------------------------------------------------------------------
<h1> Classificação de timbres. </h1>
O objetivo deste trabalho é classificar um conjunto de 416 arquivos de áudio em classes de instrumento, ou seja, identificar o timbre de cada um deles.

O conjunto de dados (disponível na pasta <i> AmostrasTratadas </i>) consiste em 52 arquivos de áudio, em formato .wav a 44100 Hz stereo para cada 8 instrumentos: cello, clarineta, flauta, oboé, trombone, trompete, viola e violino.

O classificador usado é KNN (K-Nearest Neighbours), que consiste essencialmente em, dada uma métrica (como a distância euclidiana, por exemplo) classificar um novo elemento de acordo com a proximidade com um conjunto de elementos já classificados. Assim, já se conhecendo a classificação de alguns elementos, e classificação de um novo é dada de acordo com a métrica estabelecida: o novo elemento pertence à mesma classe dos elementos já classificados mais próximos dele (seus "vizinhos").
