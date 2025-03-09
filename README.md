# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="assets/logo-fiap.png" alt="FIAP - Faculdade de Informática e Administração Paulista" border="0" width=40% height=40%></a>
</p>

<br>

# **🚀 Projeto de Machine Learning e Computação em Nuvem - FIAP**
Este repositório contém as entregas obrigatórias da **Fase 5** do curso da **FIAP**, abordando **Machine Learning** e **Computação em Nuvem**.  

---

## Integrantes: 
- <a href="https://www.linkedin.com/in/joseandrefilho">Jose Andre Filho</a>

## Professores:
### Tutor 
- <a href="https://www.linkedin.com/in/leonardoorabona/">Leonardo Ruiz Orabona</a>
### Coordenador
- <a href="https://www.linkedin.com/in/profandregodoi/">André Godoi Chiovato</a>

---
## 📂 Estrutura do Repositório

```
📦 1TIAOR20242_FASE5_CAP1
│── 📁 assets                                         # Imagens e logos do projeto
│── 📁 aws                                            # Documentação e análise de custos AWS
│   ├── 📁 images                                     # Capturas de tela e gráficos da estimativa AWS
│   ├── 📄 aws_estimativa_ec2.pdf                     # Comparação de custos AWS EC2
│   ├── 📄 README.md                                  # Detalhes da estimativa de custos AWS
│── 📁 notebooks                                      # Notebooks e datasets utilizados
│   ├── 📁 data                                       # Arquivos de dados usados na modelagem
│   ├── 📁 images                                     # Gráficos gerados pelos modelos de ML
│   ├── 📄 crop_yield.csv                             # Dataset de rendimento agrícola
│   ├── 📄 JoseAndreFilho_RM87775_pbl_fase5.ipynb     # Notebook principal
│   ├── 📄 README.md                                  # Documentação do projeto de Machine Learning
│── 📄 requirements.txt                               # Dependências do projeto
│── 📄 README.md                                      # Este arquivo (documentação geral)
```

---

## 📌 Objetivo do Projeto

Este projeto tem duas entregas obrigatórias:

1️⃣ **Previsão de Rendimento Agrícola com Machine Learning**  
2️⃣ **Comparação de Custos para Hospedagem na AWS**  

---

## 🧑‍💻 **Entrega 1: Previsão de Rendimento Agrícola (Machine Learning)**  

📍 **Localização:** [`notebooks/README.md`](notebooks/README.md)  
📍 **Objetivo:** Desenvolver um modelo de **Machine Learning** para prever o rendimento da safra agrícola, utilizando um conjunto de dados com informações sobre clima e solo.  

🔹 **Técnicas Utilizadas:**  
- **Análise Exploratória de Dados (EDA)**  
- **Clusterização (K-Means) para identificar padrões**  
- **Modelagem preditiva com 5 algoritmos diferentes:**  
  - **Regressão Linear**  
  - **Árvore de Decisão**  
  - **Random Forest**  
  - **SVR**  
  - **MLP (Rede Neural)**  
- **Métricas de avaliação:** MAE, RMSE, R²  

🔗 **Mais detalhes:** [`notebooks/README.md`](notebooks/README.md)  

---

## ☁️ **Entrega 2: Comparação de Custos AWS**  

📍 **Localização:** [`aws/README.md`](aws/README.md)  
📍 **Objetivo:** Estimar os custos de hospedar um modelo de Machine Learning na AWS, comparando as regiões **South America (São Paulo)** e **US East (N. Virginia)**.  

🔹 **Configuração da Instância EC2 Avaliada:**  
- **Tipo:** `t4g.micro`  
- **vCPUs:** 2  
- **Memória:** 1 GiB  
- **Rede:** Até 5 Gbps  
- **Armazenamento:** 50 GB (EBS SSD - gp3)  
- **Sistema Operacional:** Linux  
- **Uso:** On-Demand (100%)  

🔗 **Mais detalhes:** [`aws/README.md`](aws/README.md)  

---

## ⚙️ **Como Executar o Projeto**

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

## 📜 **Licença**
<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1"><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1"><p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://github.com/agodoi/template">MODELO GIT FIAP</a> por <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://fiap.com.br">Fiap</a> está licenciado sobre <a href="http://creativecommons.org/licenses/by/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">Attribution 4.0 International</a>.</p>

