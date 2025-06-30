# Detecção de Fraude em Transações de Cartão de Crédito: Uma Abordagem em Cascata SVM-XGBoost

Este repositório contém os materiais de um estudo focado na detecção de fraudes em transações de cartão de crédito utilizando uma abordagem híbrida inovadora. Diante do desafio do **extremo desbalanceamento de classes** em dados financeiros, implementamos um **modelo em cascata SVM-XGBoost** que combina a robustez de um Support Vector Machine (SVM) com o poder preditivo do XGBoost para identificar transações fraudulentas com alta eficácia.

## Conteúdo do Repositório

Neste repositório, você encontrará os seguintes arquivos e recursos:

- **`fraud_detection_notebook.ipynb`**: O Jupyter Notebook contendo todo o código-fonte desenvolvido para este projeto. Inclui etapas de pré-processamento de dados, implementação do modelo SVM-XGBoost em cascata, treinamento, avaliação e comparações com os modelos de referência.
- **`Artigo - Detecção Otimizada de Fraude com Cartão de Crédito - Um Sistema Híbrido em Cascata SVM-XGBoost Focado no Refinamento de Predições.pdf`**: O artigo científico completo que detalha a metodologia proposta, os experimentos realizados, os resultados obtidos e a análise das descobertas.
- **`Apresentação - Detecção Otimizada de Fraude com Cartão de Crédito - Um Sistema Híbrido em Cascata SVM-XGBoost Focado no Refinamento de Predições.pdf`**: A apresentação utilizada para descrever o projeto, seus objetivos, métodos e principais conclusões.
- **`dataset.zip\creditcard.csv`**: O dataset "Credit Card Fraud Detection" utilizado neste estudo, disponibilizado publicamente no Kaggle. Este arquivo contém as transações de cartão de crédito (devidamente anonimizadas) sobre as quais os modelos foram treinados e avaliados.

## O Projeto

Nosso trabalho explora a aplicação de um modelo em cascata onde um **SVM atua como classificador primário**, identificando padrões iniciais nas transações. Suas **probabilidades de predição** são então usadas como **meta-features para um XGBoost**, que funciona como um **refinador** para aprimorar a capacidade preditiva, especialmente para a rara classe de fraudes.

Para lidar com o severo desbalanceamento de classes (apenas 0.172% de fraudes no dataset), empregamos técnicas de **reamostragem (SMOTE)** e otimização do **limiar de decisão** com base na curva Precision-Recall, garantindo que o modelo não apenas detecte as fraudes, mas também minimize falsos positivos.

Os resultados obtidos, detalhados no artigo, demonstram que nosso modelo oferece um **equilíbrio robusto** entre a detecção de fraudes e a minimização de falsos positivos, apresentando desempenho superior ou comparável aos modelos de referência de estado da arte.

## Como Usar o Repositório

Para explorar este projeto:

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/SeuUsuario/SeuRepositorio.git
    cd SeuRepositorio
    ```
2.  **Abra o Jupyter Notebook:** Você pode abrir o `fraud_detection_notebook.ipynb` no Jupyter Lab ou Jupyter Notebook para inspecionar e executar o código. Certifique-se de ter as bibliotecas Python necessárias instaladas (listadas no notebook ou em um futuro `requirements.txt`).
3.  **Consulte os PDFs:** Revise o `Artigo_Detecao_Fraude.pdf` para uma compreensão aprofundada da pesquisa e o `Apresentacao_Final.pdf` para uma visão geral concisa.

## Contribuição

Sinta-se à vontade para explorar, usar e adaptar este código para seus próprios projetos ou pesquisas. Sugestões e contribuições são bem-vindas\!
