# Previsão do INDE - ONG Passos Mágicos
## Descrição
Projeto de parceria entre a FIAP e a ONG Passos Mágicos. Criação de modelo de previsão do índice de desenvolvimento dos alunos da ONG Passos Mágicos, junto com dashboard interativo para análise facilitada dos indicadores dos alunos da ONG.
## A Passos Mágicos
A Associação Passos Mágicos tem uma trajetória de 30 anos de atuação, trabalhando na transformação da vida de crianças e jovens de baixa renda os levando a melhores oportunidades de vida. A transformação, idealizada por Michelle Flues e Dimetri Ivanoff, começou em 1992, atuando dentro de orfanatos, no município de Embu-Guaçu.
Em 2016, depois de anos de atuação, decidem ampliar o programa para que mais jovens tivessem acesso a essa fórmula mágica para transformação que inclui: educação de qualidade, auxílio psicológico/psicopedagógico, ampliação de sua visão de mundo e protagonismo. Passaram então a atuar como um projeto social e educacional, criando assim a Associação Passos Mágicos. Atualmente, atendem 1100 alunos.
## O modelo
Considerando o INDE como a principal medida do rendimento dos alunos, refletimos sobre as vantagens de se ter um modelo que consiga prever o INDE antes do final do período letivo, com base nos índices de anos anteriores. Pensamos que a previsão do INDE pode ser relevante para fornecer mais apoio e atenção extra aos alunos com índices previstos mais baixos, para que a situação ainda possa ser mudada ao longo do período letivo e para que o aluno tenha chance de aumentar seu INDE no processo. Para criar o modelo, consideramos o dataset como sendo uma série temporal de cada aluno. Diversos alunos não tem os INDEs registrados nos 3 anos contidos no dataset, portanto, para preservar a profundidade da série temporal, consideramos somente os alunos que tinham INDEs registrados em 2020, 2021 e 2022, totalizando 314 alunos. Entendemos que a quantidade de dados fornecidos não é a ideal para treinar o modelo, mas essa pode ser uma primeira versão para inspirar a criação de um modelo mais robusto com o aumento de dados futuro. 
## Entregáveis
Constam nesse repositório:
* Dataset original enviado pela PM.
* Dicionário de dados da PM.
* Relatórios de dados da PM - 2020, 2021, 2022
* Notebooks de tratamento do dataset original.
* Datasets tratados (utilizados para as análises PBI / modelo).
* Código da aplicação do modelo em streamlit.
* Dashboard em Power BI.
## Como utilizar?
**Modelo**
* Rodar o notebook _Tratamento de dados_PM_ utilizando o dataset _df_original_ para leitura.
* Com VS Code (ou outra IDE), instalar os componentes do arquivo _requirements.txt_.
* Rodar o código da aplicação do modelo em streamlit (arquivo _app.py_) utilizando o dataset resultante do notebook _Tratamento de dados_PM_ (ou o arquivo _Pm_modelo_).
* Com essas operações, o modelo estará pronto para uso.

**Dashboard**
* Rodar o notebook _PM_despivot_, usando o dataset _PM_modelo_ como base.
* Utilizar os datasets _PM_modelo_ e _PM_indices_ para atualizar as visões. 
