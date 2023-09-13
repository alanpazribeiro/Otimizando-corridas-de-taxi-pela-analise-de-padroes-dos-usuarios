# Otimizando rotas de táxi através dos padrões dos usuários
Projeto 5 - Encontrando Padrões de utilização dos Usuários de Táxi para Otimizar Corridas

####  Passo 1. Verificando dados no em um site - Python

 Análise dos dados sobre o clima em Chicago em novembro de 2017.
 
####  Passo 2. Análise exploratória de dados - SQL

 - Verificar o número de corridas de táxi para cada empresa entre 15 e 16 de novembro de 2017
 - Verificar o número de corridas cujos nomes das companhias contenham as palavras YELLOW e BLUE
 - Verificando as corridas das companhias mais populares
 
####  Passo 3. Análise exploratória de dados - SQL

 - Verificando os indentificadores dos bairros O'Hare e Loop
 - Verificando as condições meteorológicas e alterando pra BAD (chuva/tempestade) e GOOD(outros)
 - Verificando as corridas que começam no Loop e terminam em O'Hare aos sábados, bem como as condições meteorológicas


####  Passo 4. Análise exploratória de dados - Python

  Além dos dados recuperados nas tarefas anteriores, dois CSVs:

- project_sql_result_01.csv. Ele contém os seguintes dados:
     
   - company_name: nome da empresa de táxi
   - trips_amount: o número de corridas para cada empresa de táxi de 15 a 16 de novembro de 2017.
    
- project_sql_result_04.csv. Ele contém os seguintes dados:
   
   - dropoff_location_name: bairros de Chicago onde as corridas terminaram
   - average_trips: o número médio de viagens que terminaram em cada bairro em novembro de 2017.
        
Para esses dois conjuntos de dados:
- importar os arquivos
- estudar os dados que eles contêm
- verifique se os tipos de dados estão corretos
- identificar os 10 principais bairros em termos de destinos
- fazer gráficos: empresas de táxi e número de corridas, 10 principais bairros por número de corridas em que esse - bairro é destino
- tirar conclusões com base em cada gráfico e explicar os resultados


#### Passo 5. Testando hipóteses - Python

Para esse passo, será utilizado o arquivo que contém dados sobre viagens do Loop para o Aeroporto Internacional O'Hare:

- project_sql_result_07.csv - Valores dos campos da tabela:
    - start_ts — data e hora do começo da corrida
    - weather_conditions — condições meteorológicas no momento em que a corrida começou
    - duration_seconds — duração da viagem em segundos


<b>Teste a hipótese: "A duração média dos passeios do Loop para o Aeroporto Internacional O'Hare muda nos sábados chuvosos."
<b>

Explique:
   - como você formou as hipóteses nula e alternativa
   - qual critério você usou para testar a hipótese e porque
   - Alpha: a critério

# Execução do Projeto
- Passo 1. Carregamento os dados e prepare-os para a análise
  - Verificado tipo de dado
  - Nulos/faltantes
  - organizar/renomear colunas
  - colunas tipo datetime
  - amplitude das variáveis
  - tipos de dados categóricos
  - valores duplicados
  - espaços e caracteres especiais nos dados
