Estudo do laboratório de Sensoriamento Remoto da Universidade da Amazonia (UNAMA) sobre o trabalho "Predicting the pulse of the Amazon: Machine learning insights into
deforestation dynamics"

### 1. *Coleta de Dados*
   - *Fontes de Dados*:
     -  *Dados de Desmatamento*: Utilize dados do PRODES (Programa de Monitoramento da Floresta Amazônica por Satélite) do INPE (Instituto Nacional de Pesquisas Espaciais). Disponível em: [http://www.obt.inpe.br/](http://www.obt.inpe.br/). 
       
     - *Dados de Focos de Incêndio*: Utilize dados do BDQUEIMADAS do INPE. Disponível em: [http://queimadas.dgi.inpe.br/](http://queimadas.dgi.inpe.br/).
     - *Dados Socioeconômicos*: Utilize dados do IBGE (Instituto Brasileiro de Geografia e Estatística) para variáveis como PIB, produção agrícola, população, etc. Disponível em: [https://www.ibge.gov.br/](https://www.ibge.gov.br/).
     - *Dados de Crédito Rural*: Utilize dados do Banco Central do Brasil. Disponível em: [https://www.bcb.gov.br/](https://www.bcb.gov.br/).
     - *Dados de Unidades de Conservação*: Utilize dados do ISA (Instituto Socioambiental). Disponível em: [https://www.socioambiental.org/](https://www.socioambiental.org/).
     - *Dados de Partidos Políticos*: Utilize dados de governadores e partidos políticos disponíveis no Wikipedia.

   - *Variáveis Selecionadas*:
     - Desmatamento (km²) :heavy_check_mark:
     - Focos de Incêndio :heavy_check_mark:
     - PIB (R$) :heavy_check_mark:
     - Área Plantada ou Colhida (hectares) :heavy_check_mark: 
     - Valor da Produção Agrícola (R$) :heavy_check_mark:
     - PIB Agrícola Estadual (R$) :heavy_check_mark:
     - População :heavy_check_mark:
     - Fluxo de Crédito Rural (R$) :heavy_check_mark:
     - Extensão de Unidades de Conservação (hectares) :heavy_check_mark:
     - Rebanho Bovino (cabeças) :heavy_check_mark:
     - Área de Culturas Permanentes (hectares) :heavy_check_mark:
     - Área de Culturas Temporárias (hectares) :heavy_check_mark:
     - Produção de Milho (R$) :heavy_check_mark:
     - Produção de Soja (R$) :heavy_check_mark:
     - Despesa Orçamentária (R$) :heavy_check_mark:
     - Partido Político do Governador :heavy_check_mark:
    
### 2.Processamento dos Dados:
   - * Dados Processados:
       - Partido Político do Governador :heavy_check_mark:  
       - Desmatamento :heavy_check_mark:
       - Área de Culturas Temporárias :heavy_check_mark:
       - Produção de Milho (R$) :heavy_check_mark:
   - * Dados Não Processados:
       - População ❌
       - Despesas Orçamentárias ❌
       - Produção de Milho ❌
       - Área colhida ou plantada por hectares ❌
       - Focos de Incêndio ❌ 
       - PIB (R$) ❌
       - Produção de Soja (R$) ❌
       - Área de Culturas Permanentes (hectares) ❌ 
       - Extensão de Unidades de Conservação (hectares) ❌
       - Fluxo de Crédito Rural (R$)❌
       - Rebanho Bovino (cabeças)❌
       - PIB Agrícola Estadual (R$)❌ 

### 2. *Pré-processamento de Dados*
   - *Transformação de Variáveis Categóricas*:
     - Converta a variável "Partido Político" em formato binário (0 ou 1) usando o método get_dummies do Pandas.
   - *Normalização*:
     - Normalize todas as variáveis para o intervalo de 0 a 1 usando o MinMaxScaler do scikit-learn.
   - *Divisão dos Dados*:
     - Divida o conjunto de dados em 80% para treinamento e 20% para teste.
     - Utilize validação cruzada (k-fold) para garantir a robustez dos modelos.

### 3. *Modelagem*
   - *Algoritmos de Machine Learning*:
     - *Árvores de Decisão*
     - *Random Forest*
     - *Extra Trees*
     - *Gradient Boosting*
     - *Support Vector Machine (SVM)*
   - *Avaliação de Modelos*:
     - Utilize métricas como coeficiente de determinação (R²), erro quadrático médio (MSE) e erro absoluto médio (MAE) para avaliar o desempenho dos modelos.
   - *Importância das Variáveis*:
     - Utilize SHAP (SHapley Additive exPlanations) para interpretar a importância das variáveis nos modelos.

### 4. *Análise Exploratória de Dados*
   - *Gráficos Temporais*:
     - Crie gráficos de linha para identificar padrões temporais nas variáveis.
   - *Matriz de Correlação*:
     - Analise a correlação entre as variáveis para identificar relações significativas.

### 5. *Implementação*
   - *Ferramentas*:
     - Utilize Python com bibliotecas como Pandas, scikit-learn, SHAP, e Matplotlib/Seaborn para visualização.
   - *Ambiente*:
     - Utilize Google Colab ou um ambiente local com Python instalado.

### 6. *Execução e Validação*
   - *Treinamento dos Modelos*:
     - Treine os modelos com o conjunto de treinamento e avalie com o conjunto de teste.
   - *Validação Cruzada*:
     - Utilize validação cruzada para garantir que os modelos não estão superajustados.
   - *Interpretação dos Resultados*:
     - Utilize SHAP para interpretar a contribuição de cada variável para as previsões dos modelos.

### 7. *Conclusão e Relatório*
   - *Análise dos Resultados*:
     - Compare o desempenho dos modelos e discuta as variáveis mais importantes.
   - *Recomendações de Políticas*:
     - Com base nos resultados, proponha políticas para mitigar o desmatamento.

### 8. *Publicação e Compartilhamento*
   - *Disponibilização dos Dados*:
     - Disponibilize os dados e códigos utilizados para replicação e validação por outros pesquisadores.

### Resumo dos Passos:
1. Coletar dados das fontes mencionadas.
2. Pré-processar os dados (transformação categórica, normalização, divisão em treino/teste).
3. Treinar e avaliar modelos de machine learning (Árvores de Decisão, Random Forest, Extra Trees, Gradient Boosting, SVM).
4. Realizar análise exploratória e interpretar os resultados com SHAP.
5. Concluir com recomendações políticas e disponibilizar dados e códigos.
