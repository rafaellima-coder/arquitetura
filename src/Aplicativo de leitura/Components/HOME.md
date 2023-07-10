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

