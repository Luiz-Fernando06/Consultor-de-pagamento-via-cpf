# 🔎 Automação de Consulta de Pagamentos por CPF


Este projeto utiliza Python + Selenium + OpenPyXL para automatizar a consulta de status de pagamentos em um site de validação de CPF e registrar os resultados em uma planilha de fechamento.

🚀 Como funciona

Entrada de dados

O script lê os dados de clientes de uma planilha dados_clientes.xlsx contendo:

Nome

Valor

CPF

Vencimento

Consulta automática

Abre o navegador com Selenium

Acessa o site de consulta de CPF

Preenche o CPF do cliente

Verifica o status do pagamento (em dia ou atrasado)

Saída de dados

Se o cliente estiver em dia:

Extrai a data do pagamento e o método de pagamento (cartão ou boleto)

Registra na planilha planilha fechamento.xlsx com status "ok"

Se o cliente estiver atrasado:

Registra na planilha planilha fechamento.xlsx com status "pendente"

📂 Estrutura esperada de arquivos

dados_clientes.xlsx → Planilha de entrada com os dados dos clientes

planilha fechamento.xlsx → Planilha de saída/fechamento com os resultados das consultas

🛠 Tecnologias utilizadas

Python

Selenium
 → Automação de navegador

OpenPyXL
 → Manipulação de planilhas Excel

📌 Observações

É necessário ter o Google Chrome e o chromedriver compatível com sua versão do navegador.

Certifique-se de que as planilhas de entrada e saída estejam no mesmo diretório do script.
