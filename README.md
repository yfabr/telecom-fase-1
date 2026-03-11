Este é o README estruturado para o seu projeto no GitHub ou para a célula inicial do seu notebook. Ele resume a proposta do desafio, as tecnologias utilizadas e o fluxo de trabalho seguido.

📡 Telecom X: Churn Prediction Analysis
📋 Sobre o Projeto
Este projeto consiste na análise exploratória de dados (EDA) da Telecom X, focando no fenômeno de Churn (Evasão de Clientes). O objetivo principal é transformar dados brutos de uma API JSON em insights estratégicos que permitam identificar por que os clientes estão deixando a empresa e como reverter esse cenário.

🛠️ Tecnologias e Ferramentas
Linguagem: Python

Manipulação de Dados: Pandas, NumPy

Visualização: Matplotlib, Seaborn

Fonte de Dados: API Telecom X (GitHub JSON)

🚀 Fluxo de Desenvolvimento
1. Ingestão e Normalização
Os dados foram importados via requisição HTTP. Devido à estrutura aninhada do JSON (sub-dicionários para customer, phone, internet e account), utilizamos a técnica de aplanamento (flattening) para converter o JSON em um DataFrame tabular.

2. Saneamento (Data Cleaning)
Tratamento de strings vazias na coluna account.Charges.Total.

Conversão de tipos de dados (Object -> Numeric).

Tratamento de valores ausentes (NaN) para clientes com tenure zero.

Verificação de consistência em variáveis categóricas.

3. Análise Exploratória (EDA)
Focamos em cruzar a variável alvo Churn com:

Variáveis Categóricas: Tipo de contrato, método de pagamento e suporte técnico.

Variáveis Numéricas: Mensalidade (MonthlyCharges) e Tempo de permanência (tenure).

📈 Principais Insights
Contratos Mensais: São o maior grupo de risco, com taxa de evasão significativamente superior aos contratos anuais.

Experiência Inicial: Clientes nos primeiros 6 meses de contrato têm a maior probabilidade de saída.

Fibra Óptica: Apresenta um churn maior que o esperado, sugerindo problemas de precificação ou percepção de valor.

📂 Como Executar
Clone este repositório.

Certifique-se de ter as bibliotecas pandas, requests e seaborn instaladas.

Execute o arquivo .ipynb para visualizar o relatório completo e os gráficos gerados.

Desenvolvido como parte do Challenge de Data Science da Telecom X. 🚀
