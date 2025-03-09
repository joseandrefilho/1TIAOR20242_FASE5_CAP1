# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# **Previsão de Rendimento de Safras com Machine Learning**

## Integrantes: 
- <a href="https://www.linkedin.com/in/joseandrefilho">Jose Andre Filho</a>

## Professores:
### Tutor 
- <a href="https://www.linkedin.com/in/leonardoorabona/">Leonardo Ruiz Orabona</a>
### Coordenador
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi Chiovato</a>

---

## **📌 Introdução**
Este projeto tem como objetivo prever o **rendimento da safra agrícola** utilizando técnicas de **Machine Learning**, baseando-se em dados climáticos e características do solo.  

Com a utilização de diferentes **modelos preditivos**, buscamos identificar **quais fatores influenciam mais o rendimento das culturas agrícolas**, além de avaliar se técnicas de **clusterização (K-Means)** podem melhorar a precisão das previsões.  

---

## **📌 Objetivo**
O objetivo deste projeto é:  
✅ Aplicar **modelos de regressão supervisionada** para prever a produção agrícola.  
✅ Utilizar **técnicas de aprendizado não supervisionado (K-Means)** para identificar padrões nos dados.  
✅ Avaliar **a influência de variáveis climáticas e do solo** no rendimento das safras.  
✅ Comparar diferentes **modelos de Machine Learning** e analisar seu desempenho.  

---

## **📌 Estrutura do Projeto**
```
.
├── assets/                                      # Recursos visuais utilizados no projeto (logos, imagens)
├── data/                                        # Dados utilizados no projeto
│   ├── crop_yield.csv                           # Dataset principal com informações climáticas e de rendimento
├── notebooks/                                   # Notebooks Jupyter contendo a análise e modelagem dos dados
│   ├── JoseAndreFilho_RM87775_pbl_fase5.ipynb   # Notebook com a análise exploratória dos dados, análise de clusterização e modelagem e avaliação dos modelos
├── requirements.txt                             # Arquivo com as dependências do projeto
├── README.md                                    # Documentação do projeto
```

---

## **📌 Etapas do Projeto**
### **1️⃣ Análise Exploratória dos Dados**
✔️ Carregamento do dataset (`crop_yield.csv`).  
✔️ Análise estatística das variáveis climáticas e de produtividade.  
✔️ Identificação de **outliers** e análise de sua influência nos dados.  
✔️ Aplicação de técnicas de **visualização de dados** (histogramas, boxplots, gráficos de dispersão).  

### **2️⃣ Clusterização dos Dados**
✔️ Aplicação do **K-Means** para agrupar os dados em diferentes clusters.  
✔️ Utilização do **Método do Cotovelo** para determinar o número ideal de clusters.  
✔️ Comparação dos grupos identificados e análise de tendências nos rendimentos das safras.  

### **3️⃣ Modelagem Preditiva**
✔️ Definição dos modelos preditivos:  
   - **Regressão Linear**  
   - **Árvore de Decisão**  
   - **Random Forest**  
   - **Suporte a Vetores (SVR)**  
   - **Rede Neural (MLPRegressor)**  
✔️ Comparação do desempenho dos modelos **com e sem clusterização**.  
✔️ Avaliação das métricas de desempenho: **MAE, RMSE, R²**.  
✔️ Otimização dos hiperparâmetros dos modelos para obter melhor precisão.  

---

## **📌 Comparação dos Modelos**
Após os treinamentos, avaliamos os modelos em dois cenários: **com clusterização (`Cluster_4`) e sem clusterização**.  

| Modelo               | Cenário        | MAE   | RMSE  | R²    |
|----------------------|---------------|--------|--------|--------|
| Regressão Linear     | Com Cluster   | **3055.46** | 4223.71 | **0.9954** |
| Regressão Linear     | Sem Cluster   | 3132.79 | 4394.16 | 0.9950 |
| Árvore de Decisão    | Com Cluster   | 3878.69 | 7737.66 | 0.9845 |
| Árvore de Decisão    | Sem Cluster   | 3440.69 | 5640.31 | **0.9917** |
| Random Forest        | Com Cluster   | **2565.34** | **5094.24** | 0.9933 |
| Random Forest        | Sem Cluster   | 2739.88 | **4746.89** | **0.9949** |
| SVR                 | Ambos         | 38974.58 | 71313.65 | **-0.3110** |
| MLP (Rede Neural)   | Ambos         | 59070.90 | 65474.19 | **-0.1051** |

✅ **Melhores modelos:** **Random Forest e Regressão Linear**.  
🚨 **Piores modelos:** **SVR e MLP (Rede Neural), que apresentaram R² negativo e alto erro**.  

---

## **📌 Tecnologias Utilizadas**
✅ **Linguagem de Programação:** Python  
✅ **Bibliotecas de Machine Learning:** `scikit-learn`  
✅ **Bibliotecas de Manipulação de Dados:** `pandas`, `numpy`  
✅ **Visualização de Dados:** `matplotlib`, `seaborn`  
✅ **Ambiente de Desenvolvimento:** Jupyter Notebook  

---

## **📌 Como Executar o Projeto**
1️⃣ **Clone este repositório** para sua máquina local:
   ```bash
   git clone https://github.com/joseandrefilho/1TIAOR20242_FASE5_CAP1.git
   ```

2️⃣ **Entre na pasta do projeto**:
   ```bash
   cd 1TIAOR20242_FASE5_CAP1
   ```

4️⃣ **Abra o arquivo `.ipynb` no VS Code**  
   - Instale a extensão **"Python"** e **"Jupyter"** no VS Code caso ainda não tenha.  
   - Execute célula por célula utilizando o atalho `Shift + Enter`.

5️⃣ **Execute as células dos notebooks** na ordem correta para reproduzir os resultados.

---

## **📌 Conclusão**
Este projeto demonstrou que **modelos de Machine Learning podem prever o rendimento da safra** com alta precisão.  
Os **modelos Random Forest e Regressão Linear** tiveram **os melhores resultados**, enquanto **SVR e MLP não foram eficientes** para este problema.  

A **clusterização (`Cluster_4`) impactou alguns modelos, mas não foi decisiva para todos**.  
O uso de **dados climáticos e do solo é essencial** para previsões agrícolas mais precisas.  

Este estudo pode ser expandido incluindo **novos fatores ambientais**, como **tipo de solo e práticas de cultivo**, para refinar ainda mais as previsões.

---

## 📊 Comparação de Modelos

Os gráficos abaixo comparam os valores reais de rendimento das safras com os valores previstos pelos modelos.  
O objetivo é verificar o quão bem cada modelo consegue prever a produtividade agrícola.

---

### Valores Reais vs Preditos

#### Random Forest
Os gráficos abaixo mostram como o modelo **Random Forest** se comportou ao prever os rendimentos da safra.  
A linha tracejada vermelha representa a previsão ideal, onde os valores reais e preditos são idênticos.  
Se os pontos estiverem próximos dessa linha, significa que o modelo fez previsões precisas.

- **Com Clusterização:** O modelo leva em conta a segmentação em clusters para suas previsões.
- **Sem Clusterização:** O modelo trabalha sem essa informação adicional.

![Random Forest - Com Cluster](images/graficos_resultados/Random%20Forest_dispersao_Com_Cluster.png)
![Random Forest - Sem Cluster](images/graficos_resultados/Random%20Forest_dispersao_Sem_Cluster.png)

✅ **Análise:** O modelo Random Forest teve previsões bastante alinhadas com os valores reais, o que indica um **ótimo desempenho**.

---

#### Regressão Linear
Agora, analisamos o desempenho do modelo **Regressão Linear**, que tenta encontrar uma relação linear entre as variáveis para prever os rendimentos.

![Regressão Linear - Com Cluster](images/graficos_resultados/Regressão%20Linear_dispersao_Com_Cluster.png)
![Regressão Linear - Sem Cluster](images/graficos_resultados/Regressão%20Linear_dispersao_Sem_Cluster.png)


✅ **Análise:** A Regressão Linear também teve um desempenho bom, mas ligeiramente inferior ao Random Forest.  
Observamos que alguns pontos se afastam mais da linha vermelha, indicando erros um pouco maiores.

---

## 📉 Distribuição dos Erros Residuais

Os gráficos abaixo mostram **os erros residuais** de cada modelo, ou seja, **a diferença entre os valores reais e os valores previstos**.

📌 **Como interpretar:**  
- Quanto mais concentrados os valores em **torno do zero**, melhor o modelo.  
- Se houver **erros grandes espalhados**, o modelo pode ter dificuldades para prever corretamente algumas safras.  

---

#### Random Forest  
Os gráficos abaixo mostram os erros do modelo **Random Forest** em ambos os cenários.

![Random Forest - Com Cluster](images/graficos_resultados/Random%20Forest_residuos_Com_Cluster.png)
![Random Forest - Sem Cluster](images/graficos_resultados/Random%20Forest_residuos_Sem_Cluster.png)

✅ **Análise:** A maioria dos erros está próxima de **zero**, o que indica que **o modelo teve poucos erros grandes**.  
Isso reforça que **o Random Forest foi o melhor modelo para prever o rendimento das safras**.

---

#### Regressão Linear  
Os gráficos abaixo mostram os erros do modelo **Regressão Linear**.

![Regressão Linear - Com Cluster](images/graficos_resultados/Regressão%20Linear_residuos_Com_Cluster.png)
![Regressão Linear - Sem Cluster](images/graficos_resultados/Regressão%20Linear_residuos_Sem_Cluster.png)

✅ **Análise:** A Regressão Linear teve mais dispersão nos erros, indicando que **suas previsões não foram tão precisas quanto as do Random Forest**.  
Ainda assim, os erros não foram tão extremos, tornando-a uma alternativa viável.

---

## 🔎 **Conclusão**
- O modelo **Random Forest** foi o mais preciso na previsão do rendimento das safras, com **erros menores e previsões bem ajustadas**.  
- A **Regressão Linear** teve um desempenho razoável, mas com erros um pouco maiores.  
- A clusterização **não impactou significativamente os modelos**, pois os gráficos de dispersão e erro mostraram resultados similares **com e sem clusterização**.

📢 **Escolha final:** **Random Forest** é a melhor opção para prever os rendimentos agrícolas desta fazenda! 🚀🌱

---

## Licença
<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
