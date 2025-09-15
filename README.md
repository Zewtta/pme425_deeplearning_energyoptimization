# Otimização de Consumo Energético em Injeção Plástica com Deep Learning

## 📌 Descrição
Este projeto apresenta uma metodologia para **otimização do consumo energético** em processos de injeção plástica, utilizando **simulação virtual (Plant Simulation 2404)** e **aprendizado profundo (Deep Learning - MLP)**.  

A pesquisa foi baseada em uma injetora **ChenHsong JM-258-MK6**, cujos parâmetros operacionais foram coletados e aplicados em um modelo de simulação. Foram analisados três cenários:  
- Máquina sempre ligada  
- Máquina sempre desligada  
- Máquina com chaveamento otimizado via rede neural  

Os resultados mostraram reduções de até **6,38%** no consumo energético em relação ao cenário de referência, sem afetar o volume de produção.

---

## 🛠️ Tecnologias Utilizadas
- **Plant Simulation 2404** – Modelagem do processo de injeção plástica  
- **Python 3.x**  
- **Scikit-learn (PEDREGOSA et al., 2011)** – Treinamento da rede neural MLP  
- **Data Augmentation com Ruído Gaussiano** – Expansão da base experimental  
- **Jupyter/Colab Notebooks** – Análises e experimentos  

---

## 📊 Metodologia
1. **Modelagem da planta virtual** no Plant Simulation, representando os estados da injetora (ligada, modulando, desligada).  
2. **Geração da matriz de experimentos** variando intervalos de 1 a 1000 minutos (2000 simulações).  
3. **Expansão da base de dados** com ruído gaussiano para robustez do modelo.  
4. **Treinamento da rede neural profunda (MLP)** para prever consumo energético total e de intervalos.  
5. **Validação dos resultados** e comparação entre regimes AlwaysON, AlwaysOFF e Rede Neural Otimizada.  

---

## 📈 Resultados
- **R² = 0,679** para energia total  
- **R² = 0,960** para energia de intervalo  
- **Redução de 4,06%** em relação ao AlwaysON  
- **Redução de 6,38%** em relação ao AlwaysOFF  

As redes neurais mostraram-se eficazes como ferramenta de apoio à decisão para **estratégias de chaveamento ON/OFF** em manufatura inteligente.  

---

## 📂 Estrutura do Repositório
├── data/ # Bases de simulação e dados aumentados
├── notebooks/ # Notebooks de análise e treinamento
├── models/ # Modelos treinados da rede neural
├── figures/ # Gráficos e visualizações
└── src/ # Scripts principais em Python


---

## 🔗 Materiais Suplementares
Este projeto faz parte do artigo acadêmico:  
**“Otimização de consumo energético por simulação de manufatura de injeção plástica utilizando Deep Learning”**  

---

## 👤 Autor
**Matheus Vieira Martins**  
Programa de Mestrado em Engenharia Mecânica – FEI  
E-mail: mvmartins@fei.edu.br  
