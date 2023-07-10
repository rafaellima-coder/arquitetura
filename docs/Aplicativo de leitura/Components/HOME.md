# Components

![diagram](https://www.plantuml.com/plantuml/svg/0/hLRBRXen5DqZyGykAo8biEcgg_1IGpKXA0nDka9cnX1B7dlY1qrJzMDG5r4hTHNr2-R7Ucqpm8GX8gWimFQzzzodZpbN6ajj4bQjL2llA8-OYGcwqpfL7vfDYRysvbJVcQbHH4Q2Qy9r8n994yUIOhvW9ZNDplkp8SDSZo-39iEQA0r7amveOyg9RAGh-A3rvMeSJcxwuSKaw7ti3Rhr4ti-9589Nczf8ISXYJYDn2GWL1j98RfJLBCI56Q_d0XjH3MGNPDK4WLXOIIGpdNWA1LSPSi5OIWb32Fch32AXK89YMaiGATHEydTJteFseVGOHJWIEvtjTtn5VbpT6y8Cfeo-WYd2a6T5ZHxWXNKSPujrIdAbdE34K7CF9Ox53mM2ULKh7swa-mF7EtwtSYi2n3GEFlD8ufzEjNAw9lI99cqXU4nbj_ghJIrm2cZ4TPq8MedtwiL19zrY-g-fhRM7S48-07arPco4TYs22Rc52DiKmJv30AEiVLOX1htGRyFbP4p716eDnehaosbJ-LLe1-bqGyj87oNXDqs2dwL2W0m0gqWUuQ5Ytv0vjbpT83J8c8NQpoK8W9GokTWkzhW1Chl2jx5C4B7fTB6F1BE7ipTPWEujoVTjarV9lYHy4qKHpR73xE3xFEP0DJiAVjBbBiMgqa_ChaRClM31Wi4ApzjWfTardj8XTIWwXSsXfykgvQyDp2WRyqAFFxlgUidziefuUx4PbEIp51IwxQeTfJFWT1q1bK3QWBxhLs9LozrRdjyuQaWj_0jFIo6QyBs4w_lvzYJcpLPQ-SScJSTrJvJPR0ZGKNcDY6qeEuYJYsXs04_q5m2M-li6JhdA1JeJfb45CqtX7auWXlnA1_nDy2LvxCVhgoIXN5Q5HIb6DuZ2XAQKBbJ9nk6vpxRuFK3ff3b_8XC2QBRDzYs-zFeQj2y2CFXQ8rY0GgqapF9DjukKBVToI7oacp70bE9bPPYNp2sJcoBeNO3AypwYsVN--25QNR5UXbIxtgu8H64jyZ3EZn5j_27P7JL0gNmDeHjCBhTWRXizOErJtAMOCeSmkWo7ERAAwNIC5SchyHdMMakDoGNvmy8LBHf0_MlzZdXiVkZz0y0)



Este diagrama de componentes de nível 3 representa a estrutura de componentes dentro de cada container no sistema de leitura de medidores de gás, água e luz. Cada componente é representado por um retângulo e demonstra as relações entre eles, apresentando os principais componentes e suas interações.

**Ator Técnico Leiturista:** Representa o técnico responsável pela leitura dos medidores.
**Ator Cliente:** Representa o cliente que utiliza os serviços de gás, água e luz.
**Ator Condomínio:** Representa o condomínio de residências.

O sistema é dividido em várias partes, cada uma dentro de sua respectiva fronteira:

**Aplicativo:**
- Coleta de Leituras: Responsável pela coleta das leituras dos medidores.
- Interface do Usuário: Oferece uma interface para interação com o aplicativo.

**API:**
- Lógica de Negócio: Implementa a lógica de negócio e processamento dos dados.
- Processamento de Dados: Realiza o processamento das informações.

**Banco de Dados:**
- Armazenamento de Leituras: Armazena as leituras dos medidores.
- Informações dos Clientes: Armazena as informações dos clientes.

**Web Application:**
- Exportação de Arquivos: Realiza a exportação de arquivos.
- Interface do Usuário: Oferece uma interface para interação com a aplicação web.

**Impressora:**
- Impressora: Responsável pela impressão de boletos.

**Notificador:**
- Envio de Notificações: Realiza o envio de notificações aos clientes.

As setas representam as interações entre os componentes, indicando como eles se comunicam e colaboram no sistema.

Relações:
- O Ator Técnico Leiturista utiliza o Aplicativo para realizar suas atividades.
- O Ator Cliente visualiza a segunda via de boletos e relatórios de consumo através do Web Application.
- O Ator Condomínio também visualiza relatórios de consumo e segunda via de boletos dos clientes através do Web Application.
- O Ator Técnico Leiturista utiliza a Impressora para imprimir os boletos.
- O Aplicativo envia leituras e recebe informações da API através do protocolo JSON/HTTPS.
- A API armazena as leituras e informações no Banco de Dados usando o protocolo JDBC.
- O Web Application envia cadastros e recebe informações de leituras da API usando o protocolo JSON/HTTPS.
- O Notificador envia notificações para o Ator Cliente.
- O Web Application exporta arquivos para o ERP no formato JSON, XML/SOAP, TXT e XLSX.
- O Web Application envia e-mails através do sistema de e-mails utilizando o protocolo SMTP.
- O sistema realiza integração de dados com o ERP através de uma API que utiliza o formato JSON.

