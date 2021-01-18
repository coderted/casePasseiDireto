# casePasseiDireto
 O intuito desse case é Processar e Analisar dados de sessões de usuário, Utilizando como ferramentas o PySpark para processar e tratar os dados e a estrutura Delta lake para armazená-los. 
 
 Como boas práticas de uso da Delta lake primeiro converti os dados brutos em parquet, depois iniciei o processo de transformação para Delta lake.
 Para uma estrutura Delta lake são necessárias três camadas e são elas: Bronze, Silver e Gold.
 
 Na Camada Bronze eu transformei os arquivos .parquet em Delta
 Na Camada Silver tratei os dados - Nele geralmente são feitos refinamentos e aplicados processos de data quality
 Na Camada Gold Eu consolidei para fins de apresentar uma visão consolidada dos dados
 
 Em cada uma das três camadas Delta os dados estão sendo separados por assunto e por data.
 Exemplo: ./RAW_DATA/COURSES/COURSES_DT=20210110 - Nesse exemplo para cada processamento dos dados de curso uma pasta será criada diarimente e conterá o arquivo json do respectivo dia, ou seja, dentro da pasta 'COURSES_DT=20210110' deverá conter o json referentes aos dados de curso que foram processados no dia 10 de janeiro de 2021.
 
 A Etapa 1 do Desafio foi 100% concluída
 Devido ao encerramento do prazo e também por eu não ter conseguido encontrar uma regra para relacionar as duas bases finais a Etapa 2 aindaa encontra-se em desenvolvimento.
