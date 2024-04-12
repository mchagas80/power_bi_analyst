Desafio Módulo 3 – Processamento de Dados Simplificado com Power BI

Descrição

Este projeto envolve a criação de uma instância na Azure para MySQL, a criação de um banco de dados com base disponível no GitHub, e a integração do Power BI com MySQL no Azure. O objetivo é verificar problemas na base a fim de realizar a transformação dos dados.

Diretrizes para Transformação dos Dados:

Verifique os cabeçalhos e tipos de dados: Certifique-se de que os cabeçalhos e tipos de dados são adequados para a análise que você pretende realizar.

Modifique os valores monetários para o tipo double preciso: Isso garantirá que você possa realizar cálculos precisos com esses valores.

Verifique a existência dos nulos e analise a remoção: Os valores nulos podem afetar a análise, então é importante entender por que eles estão presentes e se eles devem ser removidos.

Verifique se há algum colaborador sem gerente: Os employees com nulos em Super_ssn podem ser os gerentes.

Verifique se há algum departamento sem gerente: Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas.

Verifique o número de horas dos projetos: Isso pode ajudar a entender a distribuição do trabalho.

Separar colunas complexas: Isso tornará os dados mais fáceis de analisar.

Mesclar consultas employee e departament: Isso criará uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção.

Elimine as colunas desnecessárias: Isso tornará os dados mais fáceis de entender e analisar.

Realize a junção dos colaboradores e respectivos nomes dos gerentes: Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.

Mescle as colunas de Nome e Sobrenome: Isso criará apenas uma coluna definindo os nomes dos colaboradores.

Mescle os nomes de departamentos e localização: Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.

Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir:

No contexto do Power BI, as operações de “Mesclar” e “Atribuir” têm propósitos diferentes.

Mesclar: Esta operação é usada quando você deseja combinar duas tabelas com base em uma ou mais colunas-chave comuns. Isso é semelhante a uma junção de tabelas em SQL. No seu caso, você está mesclando as tabelas employee e departament com base em uma chave comum. Isso é necessário quando você deseja combinar informações de duas tabelas diferentes em uma única tabela.
Atribuir: Esta operação é usada quando você deseja adicionar novas colunas a uma tabela existente. As novas colunas são geralmente derivadas de colunas existentes. Por exemplo, você pode querer adicionar uma nova coluna que é o resultado de uma expressão matemática aplicada a algumas colunas existentes.

Agrupe os dados a fim de saber quantos colaboradores existem por gerente: Isso fornecerá uma visão útil da estrutura da equipe.
Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela: Isso tornará os dados mais fáceis de entender e analisar.

