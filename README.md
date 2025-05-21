📌 Modelo de Classificação de Elegibilidade de Crédito

Este projeto apresenta um modelo de classificação treinado para prever o resultado de solicitações de crédito no sistema bancário norte-americano com base em informações financeiras dos solicitantes.
🔍 Tipo de Modelo

    KNN (K-Nearest Neighbors)

    Valor de K utilizado: 10

📊 Variáveis Utilizadas no Modelo

A ordem dos atributos no vetor de entrada é a seguinte:

[salário_anual, total_dividas, historico_pagamento (score), idade]

    salário_anual: Salário anual do solicitante em dólares.

    total_dividas: Total de dívidas contraídas pelo solicitante em dólares.

    historico_pagamento (score): Score de pagamento do solicitante (ex: 0.85 significa 85% das contas pagas em dia).

    idade: Idade do solicitante em anos.

🎯 Exemplo de Previsão

Um exemplo de entrada fornecida ao modelo e sua respectiva saída:

    Entrada (X): [45000, 8000, 0.912, 32]

    Saída (y): [3] → Categoria Elegível

🗂️ Estrutura dos Arquivos

    modelo_knn.joblib: Modelo KNN já treinado e pronto para uso.

🧾 Categorias da Saída

A variável de saída (elegibilidade) representa as seguintes categorias:

    1 = Não Elegível (pedido recusado)

    2 = Elegível com Análise (exige análise adicional)

    3 = Elegível (pedido aprovado de imediato)

🧪 Avaliação

O modelo foi treinado e testado com validação cruzada. O desempenho final será avaliado com base em 500 amostras desconhecidas, conforme especificado no enunciado da atividade
