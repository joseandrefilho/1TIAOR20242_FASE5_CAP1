# FIAP - Faculdade de Informática e Administração Paulista  

<p align="center">
<a href="https://www.fiap.com.br/"><img src="../assets/logo-fiap.png" alt="FIAP" width="40%"></a>
</p>

# **Previsão de Rendimento de Safras com Machine Learning - Entrega 1**  

## Integrantes  
- [Jose Andre Filho](https://www.linkedin.com/in/joseandrefilho)  

## Professores  
- **Tutor:** [Leonardo Ruiz Orabona](https://www.linkedin.com/in/leonardoorabona/)  
- **Coordenador:** [André Godoi Chiovato](https://www.linkedin.com/in/profandregodoi/)  

---

## **📌 Objetivo**  
Este projeto utiliza **Machine Learning** para prever o **rendimento da safra agrícola**, analisando variáveis climáticas e do solo. Buscamos:  
- Aplicar **regressão supervisionada** para previsão de produção agrícola.  
- Utilizar **K-Means** para identificar padrões nos dados.  
- Comparar modelos de **Machine Learning** e analisar seu desempenho.  

---

## **📌 Metodologia**  

### **1️⃣ Análise Exploratória dos Dados**  
✔️ Carregamento e análise estatística do dataset.  
✔️ Identificação de **outliers** e visualização dos dados.  

### **2️⃣ Clusterização dos Dados**  
✔️ Aplicação do **K-Means** e uso do **Método do Cotovelo** para definir o número de clusters.  

### **3️⃣ Modelagem Preditiva**  
✔️ Teste de diferentes modelos preditivos:  
   - **Regressão Linear**  
   - **Árvore de Decisão**  
   - **Random Forest**  
   - **SVR**  
   - **MLP (Rede Neural)**  
✔️ Avaliação das métricas **MAE, RMSE, R²** e otimização de hiperparâmetros.  

---

## **📌 Resultados**  

| Modelo               | Cenário        | MAE   | RMSE  | R²    |
|----------------------|---------------|--------|--------|--------|
| **Random Forest**    | Com Cluster   | **2565.34** | **5094.24** | 0.9933 |
| **Regressão Linear** | Com Cluster   | 3055.46 | 4223.71 | 0.9954 |
| Árvore de Decisão    | Com Cluster   | 3878.69 | 7737.66 | 0.9845 |
| SVR e MLP           | Ambos         | **Desempenho insatisfatório (R² negativo)** |

✅ **Melhores modelos:** **Random Forest e Regressão Linear**.  
🚨 **SVR e MLP apresentaram baixo desempenho**.  

---

## **📌 Tecnologias Utilizadas**  
✅ **Linguagem:** Python  
✅ **Bibliotecas:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`  
✅ **Ambiente:** Google Colab / VS Code  

---

## **📌 Como Executar o Projeto**  

1️⃣ **Clone o repositório:**  
```bash
git clone https://github.com/joseandrefilho/1TIAOR20242_FASE5_CAP1.git
cd 1TIAOR20242_FASE5_CAP1
```

2️⃣ **Instale as dependências:**  
```bash
pip install -r requirements.txt
```

3️⃣ **Abra o notebook no VS Code ou Google Colab.**  
4️⃣ **Execute as células do notebook na ordem indicada.**  

---

## **📌 Conclusão**  
O **Random Forest** apresentou o melhor desempenho, seguido pela **Regressão Linear**. A clusterização **não impactou significativamente os modelos**, mas pode ser útil para estudos mais avançados. **Novas variáveis ambientais** podem melhorar as previsões futuras.  

---

## 📊 **Visualizações e Análises**  
Os gráficos a seguir mostram a comparação entre valores reais e previstos pelos modelos **Random Forest** e **Regressão Linear**.  

**Random Forest - Dispersão**  
📌 **Com Clusterização**  
![Random Forest - Com Cluster](images/Random%20Forest_dispersao_Com_Cluster.png)  

📌 **Sem Clusterização**  
![Random Forest - Sem Cluster](images/Random%20Forest_dispersao_Sem_Cluster.png)  

✅ **Análise:** O modelo Random Forest apresentou previsões bastante alinhadas com os valores reais.  

**Distribuição dos Erros**  
📌 **Random Forest**  
![Random Forest - Resíduos](images/Random%20Forest_residuos_Com_Cluster.png)  

📌 **Regressão Linear**  
![Regressão Linear - Resíduos](images/Regressão%20Linear_residuos_Com_Cluster.png)  

✅ **Conclusão:** O **Random Forest teve menor dispersão dos erros**, reforçando sua precisão.  

---
## 🎥 Vídeo Explicativo
Gravamos um vídeo demonstrando a análise dos resultados e a comparação entre os modelos.

🔗 **Link do vídeo (YouTube - Não Listado):** [Analise dos Modelos](https://youtu.be/41xVS54huB8)
---

## Licença
<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>
