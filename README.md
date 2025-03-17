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
       - Produção de Soja(R$)  :heavy_check_mark:
       - Despesas Orçamentárias :heavy_check_mark:
       - Área plantada ou colhida (hectares) :heavy_check_mark:
       - Focos de Incêndio :heavy_check_mark:
       - Área de Culturas Permanentes (hectares) :heavy_check_mark:
       - Extra: Dados Territoriais de todos os estados :heavy_check_mark: :heavy_check_mark::heavy_check_mark:
   - * Dados Não Processados:
       - População ❌
       - PIB (R$) ❌
       - Extensão de Unidades de Conservação (hectares) ❌
       - Fluxo de Crédito Rural (R$)❌
       - Rebanho Bovino (cabeças)❌
       - PIB Agrícola Estadual (R$)❌ 

### 2. ❌  *Análise Estatística dos Dados* ❌ 
   - *Juntar os Datasets Desmatamento + (Milho/ T.km**2) *: ❌ 
   - *Juntar os Datasets Desmatamento + (Soja/ T.km**2): ❌ 
   - *Juntar os Datasets Desmatamento + (Cabeça(Gado)/ T.km**2): ❌ 
   - *Juntar os Datasets Desmatamento + (Cabeça(Gado)/ T.km**2  + (Soja/ T.km**2) + (Milho/ T.km**2):❌ 

### 3. *Análise Exploratória de Dados*
   - *Gráficos Temporais*:
     - Crie gráficos de linha para identificar padrões temporais nas variáveis.
   - *Matriz de Correlação*:
     - Analise a correlação entre as variáveis para identificar relações significativas.

### 4. *Modelagem*
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
