# Data Warehouse--BI 


O _data warehouse_ possibilita a análise de grandes volumes de dados, coletados dos sistemas transacionais ([OLTP](https://pt.wikipedia.org/wiki/OLTP "OLTP")). São as chamadas séries históricas que possibilitam uma melhor análise de eventos passados, oferecendo suporte às tomadas de decisões presentes e a previsão de eventos futuros. Por definição, os dados em um _data warehouse_ não são voláteis, ou seja, eles não mudam, salvo quando é necessário fazer correções de dados previamente carregados. Os dados estão disponíveis somente para leitura e não podem ser alterados.


Este projeto e arquivos:
Descrevem passo a passo desde a Definição do Problema até:
- Coleta de Dados
- Limpesa dos Dados
- Análise
- Resultados; Solução

Modelos e Códigos que usei pra construir:
-   O Data Warehouse e as interfaces ETL. ( Modelo Físico ) em S.Q.L
- Modelos lógicos de Armazenamento e Consulta. ( Modelo Transacional / Dimensional
- Query S.Q.L para consulta dos campeões de vendas no banco de dados.  
- Formulas Dax de análise e Perguntas de Negócio:

Que resultam na Resolução de 6 mais valisas perguntas de negócio
- Valor Médio Vendido
- Total de Venda Por Cidade do Cliente
- Total de Venda Por Região da Localidade de Venda
- Quantidade Vendida Por Categoria de Produto
- Variação do Valor de Venda Por Dia
- Quantidade Vendida Por Marca de Produto

---------------------------------------------------

- DEFINIÇÃO DO PROBLEMA


Nessa análise ajudei um varejista de eletrônicos, que tinha 27 lojas e 750 funcinários por todo o brasil, cada loja tinha o seu próprio estoque e cadastro de clientes, produtos etc.. em uma planilha excel e atualizam o sitema de vendas de equipamento de informática periodicamente. 
A missão foi ajudar o CEO a expandir a operação. Para ajuda-lo a compreender o cenário atual, tratei de consolidar os dados de todas as lojas no S.Q.L no modelo de armazenamento (Lógico Transacional).
A criação do datawarehouse serve para facilitar o resumo dos dados e relacionamentos.
Na Construção do modelo físico usei o app *DB SCHEMA* que gera as visualizações ilustradas em anexo, os códigos S.Q.L já com os relações entre as tabelas, os índices, e a representação de como os dados serão armazenados e acessados em um sistema de banco de dados.



- COLETA DE DADOS
		No processo de E.T.L fiz a carga de dados preenchendo valores de cada tabela manualmente com códigos S.Q.L 



- LIMPESA DE DADOS
 Através do modelo Analítico (Lógico Dimensional) e servirá de fonte para o power bi consultar as análises.
Em Anexo codigos com sua devida normalização dos dados na modelagem dimensional ajuda a garantir que as consultas sejam executadas rapidamente, o que é crítico em ambientes de análise em larga escala.
- SQL


	Análise
Para explorar meus conhecimentos em S.Q.L fiz um consulta direto no power-bi, nesta query selecionei as vendas com valores somente acima de 500
- Query.SQL


	Resultados;Solução
Criação do Data Warehouse, das interfaces ETL e da construção do projeto de análise de dados no Power BI. A administração e suporte de primeiro nível será de responsabilidade da equipe de TI da empresa.
Relatório de KPIs referentes ao negócio da empresa  úteis para compreender erros/acertos na gestão até dias atuais para ajudar na definição da estratégia de crescimento para os próximos anos:
- Valor Médio Vendido
- Total de Venda Por Cidade do Cliente
- Total de Venda Por Região da Localidade de Venda
- Quantidade Vendida Por Categoria de Produto
- Variação do Valor de Venda Por Dia
- Quantidade Vendida Por Marca de Produto
