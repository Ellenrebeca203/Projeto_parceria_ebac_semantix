## Projeto_parceria_ebac_semantix
# Objetivo:
Prever variável 'Grade' através do desempenho escolar de alunos (SSC, HSC, Attendance_Percentage)

# Coleta de dados
- A base de dados foi coletada na plataforma da Kaggle. Trata-se de uma base de dados com informações sobre o desempenho escolar de alunos da Índia. Foram utilizados três variáveis principais (descritas abaixo), sendo 'SSC' e 'HSC' para prever a variável alvo 'grade'.

# Dados da base
- Student_ID: Id do estudante
- Name: Nome
- Class: Classe
- SSC_Marks (SSC - Secondary School Certificate): Pontuação de notas obtidas no exame nacional realizado ao final do ensino secundário (10º ano).
- HSC_Marks (HSC - Higher Secondary Certificate): Pontuação de notas obtidas no exame nacional realizado ao final do ensino médio (12º ano).
- College_Marks: Notas da faculdade
- Attendance_Percentage: Percentual de presença do aluno;
- Grade: Desempenho acadêmico na graduação (ensino superior). - TARGET

**OBS: SSC e HSC são exames padronizados do sistema educacional da Índia. As variáveis representam a pontuação de desempenho obtido pelo estudante nesses exames.**

# Etapas do Projeto 
1. Preparação de dados: leitura de dados com biblioteca pandas.
2. Pré-processamento: limpeza dos dados, verificação da distribuição, dados nulos e de Outliers;
3. Análise bivariada: análise das variáveis entre si e exclusão de colunas desnecessárias;
4. Análise de Correlação: Matriz de correlação;
5. Separação de variáveis: Separação de X e Y, treino e teste, e padronização de dados;
6. Modelagem e Avaliação: treinamento dos modelos e validação.

# Conclusões e resultados:
Foram escolhidos alguns modelos para fazer a previsão. Random Forest, Árvore de Decisão, XGBoost e SVM, foram treinados com os dados. O modelo de bruto (sem parametrização) 'Random Forest' obteve uma acurácia de 0.23, semelhantemente os modelos de XGBoost e SVM com a mesma acurácia, o modelo de Árvore de Decisão teve umma acurácia mais baixa de 0.17. Foi aplicado parâmetros mas os modelos não conseguiram fazer boas avaliações, na verdade houve queda nas métricas. Apesar de parâmetros e outras técnicas como cross-validation terem sido aplicadas, as previsões foram muito baixas para as classes, não conseguindo discriminá-las bem, o que provavelmente explica que os dados não conseguem explicar a alvo, ou que não havia dados suficientes para isto. 



