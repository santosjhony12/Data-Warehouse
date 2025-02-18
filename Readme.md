# Projetos de Data Warehouse

## O que é? 
> Um Data Warehouse (DW) é um sistema de armazenamento de dados projetado para coletar, integrar e organizar grandes volumes de informações de diferentes fontes, com o objetivo de facilitar análises e tomada de decisões. Ele é amplamente utilizado em Business Intelligence (BI) e análise de dados.

## 📊 Business Intelligence (BI)
> O BI (Business Intelligence) é um conjunto de processos, tecnologias e ferramentas que transformam dados brutos em informações estratégicas para a tomada de decisões nas empresas.

### 💡 Fluxo do BI:
- 1️⃣ Coleta de Dados – Banco de dados, planilhas, APIs, Data Warehouse
- 2️⃣ ETL (Extração, Transformação e Carga) – Limpeza e organização dos dados
- 3️⃣ Armazenamento – Data Warehouse ou Data Lake
- 4️⃣ Análises e Relatórios – Dashboards, gráficos e KPIs
- 5️⃣ Tomada de Decisão – Insights estratégicos para o negócio


## ETL (Extract, Transform, Load)
> O ETL é um processo fundamental na engenharia de dados e Business Intelligence (BI), responsável por extrair, transformar e carregar dados de diferentes fontes para um Data Warehouse ou outro sistema de armazenamento analítico.


1️⃣ Extract (Extração)
O primeiro passo é coletar dados de diversas fontes, como:
✅ Bancos de dados (SQL, NoSQL)
✅ Planilhas (Excel, CSV)
✅ APIs e Web Services
✅ Arquivos JSON, XML, logs
✅ Sistemas OLTP

2️⃣ Transform (Transformação)
Aqui os dados são limpos e organizados para garantir qualidade e consistência, incluindo:
🔄 Remover duplicatas e inconsistências
🔄 Normalizar ou desnormalizar dados
🔄 Criar colunas derivadas e agregações
🔄 Converter formatos e corrigir erros

3️⃣ Load (Carregamento)
Por fim, os dados são carregados em um destino final, como:
📊 Data Warehouse (Snowflake, Redshift, BigQuery, etc.)
📊 Banco de Dados Analítico
📊 Data Lake

OLTP e OLAP são sistemas de processamentos de dados. São distintos.

OLTP - Processamento de transação Online 
É um sistema voltado para processar transações em tempo real, garantindo rapidez, integridade e confiabilidade dos dados.
Processamentos que executam as operações diárias.
Previne anomalias nas atualizações 
Difícil de projetar em relatórios analíticos.

OLAP - Processamento Analítico Online
Processamento que suportam a tomada de decisões, por meio de consultas e cálculos.
É um sistema projetado para análises de dados, permitindo consultas complexas e relatórios estratégicos

Características de DW
Orientado a Assuntos - armazena as informações agrupadas/relacionadas
Variante com o tempo
Não volátil
Integrado


Diferença de BD tradicional x DataWarehouse
BD tradicional são transacionais como Relacional ou Orientado a Objetos já o DW são voltado para assuntos e tomadas de decisão.

Processo ETL

FONTE DE DADOS -> ETL -> DW -> DATAMARTS

Característica	OLTP	OLAP
Objetivo	Processar transações	Analisar dados
Operações	CRUD (Create, Read, Update, Delete)	Consultas complexas e agregações
Velocidade	Alta (baixa latência)	Otimizado para leitura e análise
Modelo de Dados	Normalizado (reduz redundância)	Desnormalizado (melhor para leitura)
Exemplo	Sistema bancário, e-commerce	Relatórios gerenciais, dashboards

Banco de Dados Dimensional 
É uma forma de projetar o DW.
Utiliza conceitos de múltiplos dimensões
Conceitos de medidas e dimensões
Uma medida é um valor numérico totalizado utilizado para analisar/observar um determinado negócio.
Dimensões são filtros que afetam a maneira de visualizar as medidas.


