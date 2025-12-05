🏠 Predição de Preços de Imóveis na Índia
=========================================

Este projeto aplica técnicas de **regressão** e **análise de dados** para prever o preço total de imóveis na Índia utilizando um conjunto de dados do Kaggle.

📌 **Base de dados:**[https://www.kaggle.com/datasets/juhibhojani/house-price](https://www.kaggle.com/datasets/juhibhojani/house-price)

📌 Objetivo
-----------

Criar um modelo preditivo capaz de estimar o valor de imóveis após um processo completo de:

*   Limpeza e padronização dos dados
    
*   Tratamento de valores ausentes e outliers
    
*   Codificação de variáveis categóricas
    
*   Treinamento e comparação de modelos
    

🧹 Etapas Principais
--------------------

### **1\. Pré-processamento**

*   Conversão da moeda indiana (_Lac_, _Cr_ → valores numéricos)
    
*   Extração de números de campos como área e andares
    
*   Remoção de colunas irrelevantes ou totalmente nulas
    
*   Tratamento de valores faltantes (mediana, moda, “Not Informed”)
    
*   Remoção de outliers usando IQR
    
*   Agrupamento das top 20 localizações
    

### **2\. Análise Exploratória**

*   Distribuição de preços
    
*   Correlação entre variáveis
    
*   Comparação por localização e características do imóvel
    

### **3\. Modelagem**

Modelos testados:

*   **Regressão Linear**
    
*   **Ridge Regression**
    
*   **MLPRegressor** (redes neurais)
    

📊 Resultados
-------------

ModeloR² (Validação)Regressão Linear**≈ 0.51**Ridge Regression**≈ 0.51**MLP (melhor versão)**≈ 0.33**

➡️ **Modelos lineares apresentaram o melhor desempenho**, com menor tempo de execução e maior estabilidade.

🧠 Conclusão
------------

*   O dataset exige forte pré-processamento e redução de ruído.
    
*   Modelos lineares superaram redes neurais neste caso.
    
*   O projeto demonstra uma pipeline completa de regressão aplicada ao mercado imobiliário.
    
*   Próximos passos incluem testar **Random Forest**, **XGBoost** e criar novos atributos (como preço por área).
