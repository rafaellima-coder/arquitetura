# leitura

* [Overview](#Overview)
  * [Aplicativo de leitura](#Aplicativo-de-leitura)
    * [Components](#Components)
    * [Container](#Container)
    * [Fluxo](#Fluxo)
      * [DiagramaSequencia](#DiagramaSequencia)

---

## Overview

![diagram](https://www.plantuml.com/plantuml/svg/0/SoWkIImgAStDuUMoukNIKiZCJKnFLQWmr3DLi5AmoSnDjyeeAIcmqjSlo4dC0wdJIyxFrS_9JyytrYl8IwykJaxCIRK5Ag-ru-MovkLoICrB0Qe20000)

# Descrição dos Requisitos Funcionais e Não Funcionais e Considerações Arquiteturais

## Requisitos Funcionais:
1. O sistema deve permitir o cadastro de clientes com informações como nome, endereço e tipo de serviço.
2. O sistema deve permitir o registro das leituras dos medidores de gás, água e luz.
3. O sistema deve calcular o consumo dos clientes com base nas leituras registradas.
4. O sistema deve gerar relatórios de consumo para os clientes, contendo informações detalhadas sobre seu consumo de serviços.
5. O sistema deve fornecer aos clientes uma segunda via de boletos para pagamento dos serviços.
6. O sistema deve permitir que os administradores de condomínio acessem relatórios de consumo dos clientes vinculados ao condomínio.
7. O sistema deve enviar notificações por e-mail aos clientes sobre atualizações de consumo e vencimento de boletos.

## Requisitos Não Funcionais:**
1. O sistema deve garantir a segurança das informações dos clientes, adotando medidas adequadas de proteção de dados.
2. O sistema deve ser de fácil utilização e possuir uma interface intuitiva para os usuários.
3. O sistema deve ser escalável, permitindo o crescimento do número de clientes e registros de leitura.
4. O sistema deve ser robusto e tolerante a falhas, garantindo a disponibilidade dos serviços.
5. O sistema deve ter um desempenho eficiente, processando as operações de cadastro, leitura e cálculo de consumo de forma rápida e eficaz.
6. O sistema deve ser compatível com diferentes dispositivos e navegadores, garantindo a acessibilidade para os usuários.

## Considerações Arquiteturais


### Escalabilidade

Uma consideração importante na arquitetura do sistema de leitura de medidores de gás, água e luz é a escalabilidade. Para atingir a escalabilidade, o sistema será projetado com uma arquitetura distribuída e escalável, capaz de lidar com um grande volume de leituras e usuários. Será adotado o dimensionamento horizontal, permitindo adicionar novos servidores de acordo com a demanda.

### Segurança

A segurança é uma preocupação essencial no sistema, pois envolve dados sensíveis dos clientes. Para garantir a segurança, serão implementadas medidas como criptografia de dados, controle de acesso baseado em papéis e auditoria de atividades. Serão adotadas práticas de segurança recomendadas para proteger a integridade, confidencialidade e autenticidade dos dados.

### Resiliência

A resiliência do sistema é fundamental para garantir a disponibilidade contínua dos serviços. Serão implementadas estratégias de recuperação de falhas, como o uso de servidores redundantes, balanceamento de carga e monitoramento constante da saúde do sistema. Dessa forma, o sistema poderá se recuperar rapidamente de falhas e minimizar o impacto nos usuários.

### Integração

O sistema de leitura de medidores precisa se integrar com outros sistemas, como o ERP externo e o sistema de envio de e-mails. Serão fornecidas interfaces adequadas para facilitar a integração eficiente e confiável com esses sistemas. Serão utilizados padrões e protocolos apropriados para garantir a compatibilidade e a transferência de dados sem problemas.

### Manutenibilidade

Considerações de manutenibilidade são importantes para garantir a facilidade de manutenção e evolução do sistema ao longo do tempo. A arquitetura será projetada de forma modular e bem documentada, facilitando a compreensão e modificação dos componentes individuais. A automação de testes e implantação contínua será adotada para agilizar o processo de manutenção. Serão seguidas boas práticas de desenvolvimento e documentação para garantir a manutenibilidade do sistema.

### Inversão de Controle

Será adotado o princípio de inversão de controle (IoC) para desacoplamento e maior flexibilidade. Através da inversão de controle, as dependências entre os componentes serão gerenciadas externamente, permitindo que as implementações possam ser substituídas facilmente. Isso proporcionará maior modularidade, facilidade de teste e reutilização de código.

### TDD e DDD

Será utilizado o desenvolvimento orientado a testes (TDD) como prática de desenvolvimento. Isso envolve escrever os testes antes de implementar o código, garantindo que o sistema seja testável desde o início. Além disso, será adotado o design orientado a domínio (DDD) para garantir que o sistema reflita corretamente as regras de negócio e mantenha uma linguagem ubíqua. O DDD ajudará a organizar o código em torno dos conceitos do domínio, facilitando a compreensão e manutenção.

### Princípios SOLID

Os princípios SOLID serão seguidos durante o desenvolvimento do sistema. Cada componente será projetado com base nos princípios de Responsabilidade Única (SRP), Aberto/Fechado (OCP), Substituição de Liskov (LSP), Segregação de Interfaces (ISP) e Inversão de Dependência (DIP). Isso garantirá que o sistema seja modular, flexível, fácil de entender e manter.









## Aplicativo de leitura

`\Aplicativo de leitura`

[Overview](#leitura)

![diagram](https://www.plantuml.com/plantuml/svg/0/hLEnRjim4DqD-1ykdXmWiPPEdM8uHXF0IGF7QP59k8W7vm2ALCYZc-PlF1KTElKJz6Cb9Sk2cwHJ9v7lxjvxVAJElA2JKEhXu8XDeOCYU1If_CSiS_XjicPv30_1aoki4J8oAMoPeNACPgD35RBPXzCRZKRkhXQPHY4l4SfdgVjP9bL3FHmiflUVxrRvrylLHRwOVvfVdu-F4tv3pbipdefr-OeAmuND5yGI74Td9p1A5LZLFviIzALHh2sfSkIZAGGBqlL4gBB6rziDQQX88-Xc2a5P3oKfLZRsJ4R7dNm-VvRMmanpfADETxTzfLMqE3m5WY2i-IMY7c9A6wv_n5LCSLrl_GdKstL08D3XvKt1VAfADl503bNIjqRP1DZEma4zyROjzQ_OyygNPwDI13R43HvC5lqOD4vkltkXSdpBwPEItgtU86tmfBqFaleStp_hSB0a_VxLzifBmYR27RrFm_lH_PNq_L_OXtR2nUkL-hVZDlDuI1zA6pruMWUZ43RSk7smciGU4lyZ-lyerL7zzRpc9hNJQOciFLJei4tiZ8ngVfa_)



**Level 1: Diagrama de Contexto**

**Escopo**: O diagrama de contexto representa a interação entre os atores e o sistema de leitura de medidores de gás, água e luz.

**Público-alvo**: O diagrama é destinado aos stakeholders e membros da equipe envolvidos no projeto.

**Notas**: O diagrama mostra os principais atores envolvidos no sistema, incluindo o `Ator Técnico Leiturista`, responsável pelas leituras dos medidores, o `Ator Cliente`, que pode visualizar relatórios de consumo e segunda via de boletos, e o `Ator Administrador de Condomínio`, que também tem acesso aos relatórios e segunda via de boletos. O sistema representa a plataforma que gerencia as leituras e disponibiliza as informações para os atores envolvidos.


**Level 1: Diagrama de Contexto**

**Escopo**: O diagrama de contexto representa a interação entre os atores e o sistema de leitura de medidores de gás, água e luz.

**Público-alvo**: O diagrama é destinado aos stakeholders e membros da equipe envolvidos no projeto.

**Notas**: O diagrama mostra os principais atores envolvidos no sistema, incluindo o `Ator Técnico Leiturista`, responsável pelas leituras dos medidores, o `Ator Cliente`, que pode visualizar relatórios de consumo e segunda via de boletos, e o `Ator Administrador de Condomínio`, que também tem acesso aos relatórios e segunda via de boletos. O sistema representa a plataforma que gerencia as leituras e disponibiliza as informações para os atores envolvidos.


## Components

`\Aplicativo de leitura\Components`

[Overview](#leitura)

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



## Container

`\Aplicativo de leitura\Container`

[Overview](#leitura)

![diagram](https://www.plantuml.com/plantuml/svg/0/ZLR1JXin4Br7oZ-uUm8f99UUUYA4gAGA496bq5Fax0wB9Q-zsDv0gVeng0VKIZr5_OBziOxjtUmc9C0bYiSpxyqypqnog0rL9azvk_M1YOZdCP1ROpBzgTTJzBwRC7ERptCDAfB2W33TIAOz6Yj6nOBdMTuRV3oOS2hCvUcunwa1RT0q6w0tPG9KDtFWxTQu_-tyCfnTZSAJsNZuUNXslBTlxHDGMegzlf5g5a8aM2HdOs0cLmnpwv30tf2m-EskI7qLuDq5P0eqfaM99ARoGLCcXIwU5i191fmIxg8eYQKcASGibkZJ3VOh-jdmmVWK1fmX75IyvV45L-Jjv2u7aXl6sIDQDK6T5gnunc-eOr8ywGufdfAS4Y0yVznEA4KiKoQON74wI_4NJIzvwpjBWHSiBlw8Y55VJhir_QuDfBCZcOkOgkzxqn5YJ9arKar6cBGIKWVxFzgjrIFjzRFCicUSHTIm1V86Jd79PS8eeROmvBl1D6CdVErAqcBfTAQeRoGvO9wOMQcujaarU2Os6_nydO1qWd6nJ931GWb8YcM41GF9b8n0QvgY74w0cCPoW-E8YaWUMpjIkODrT8Qtor8fVGHHurTb83SJDnAlY-VY7sZNIMKJRF1VmTpBYLy8VlD2IM7nNsDlQdgFeKvGUCYaCfRqbyk7ghiS7JOeHwbj4IsLdPVwy1PZqzVJCJopb2aojm_fQTejqcxztDfQmsPhOKVNhLMwsYuVNapG3J-3sflW4Mjp0IKp2fcekj3LmpQHJlkZiSKwI2dZJJWC0B7mCm7krc-3xOMxebn55y1tRnx_YfT-kctGohjQ4jLJa-0hqpbrMq13OkKX2-RIQWZvhd25wyeKIyNy3i5vrtagryFhZU6rpRUbM3kzd-P5LxyNRdlHk-6soRtMnANgkxlIGTaq_4eP2alTc5O54SmtXjPsp9Vf-Ldl90mdqnMA1LXR6jKMs3dz3kZuQ511L9AKhUvdjfxLahP3hl4tSdhUHwVmEiJZU7gz2T4i9w8nrKR9NVMixTdTjVciHbi7p6_ZdesiOloKRVmO-eJyQ6dtAkiKrMGstTo0deOJwta88iO_0ly1)





**Level 2: Diagrama de Contêiner**

**Escopo**: O diagrama de contêiner representa os principais componentes e tecnologias utilizados no sistema de leitura de medidores de gás, água e luz, fornecendo uma visão detalhada da arquitetura e implantação do sistema.

**Público-alvo**: O diagrama é destinado à equipe técnica envolvida no projeto, incluindo desenvolvedores, arquitetos de software e administradores de sistemas.

**Notas**: O diagrama apresenta os contêineres que compõem o sistema, bem como as tecnologias utilizadas em cada um deles. Os contêineres são unidades de software isoladas que agrupam componentes relacionados e executam funções específicas. A equipe técnica deve estar familiarizada com os conceitos do C4 Model para entender e utilizar efetivamente este diagrama.

No diagrama de contêiner, são identificados os seguintes elementos:

- `App`: Aplicativo móvel para coleta de leituras. A equipe técnica deve selecionar a tecnologia adequada para implementar o aplicativo.
- `API`: Componente responsável pela lógica de negócio e processamento de dados. A equipe técnica deve definir a tecnologia a ser utilizada para implementar a API.
- `Banco de Dados`: Armazenamento de leituras e informações dos clientes. A equipe técnica deve escolher a tecnologia apropriada para implementar o banco de dados.
- `Web Application`: Aplicativo web para exportação de arquivos. A equipe técnica deve determinar a tecnologia adequada para implementar a aplicação web.
- `Impressora`: Impressora utilizada para imprimir boletos. A equipe técnica deve selecionar a tecnologia adequada para a implementação da impressora.

Além dos contêineres internos, existem sistemas externos integrados ao sistema principal:

- `ERP`: Sistema ERP externo utilizado para integração de dados. A equipe técnica deve definir a tecnologia a ser utilizada para a integração com o ERP.
- `E-mail`: Sistema de envio de e-mails utilizado para enviar notificações aos clientes. A equipe técnica deve escolher a tecnologia apropriada para implementar o envio de e-mails.

Os relacionamentos entre os contêineres são representados pelas setas, indicando as interações e dependências entre eles. Essas informações são cruciais para a equipe técnica compreender como os componentes se comunicam e colaboram entre si na arquitetura do sistema.

Esse diagrama de contêiner fornece uma representação clara e detalhada dos componentes e tecnologias envolvidas na implementação do sistema, auxiliando a equipe técnica na compreensão e desenvolvimento do sistema de leitura de medidores.


## Fluxo

`\Aplicativo de leitura\Fluxo`

[Overview](#leitura)

![diagram](https://www.plantuml.com/plantuml/svg/0/0m00)





## DiagramaSequencia

`\Aplicativo de leitura\Fluxo\DiagramaSequencia`

[Overview](#leitura)

![diagram](https://www.plantuml.com/plantuml/svg/0/RP4nRiCm34Lt0Re3aRqNyD36JOl2G8SWAB8J5WS1CXL8IeRSfcE7JZs2BrPAi5shy2A8_8_afxIF2KEw3auhx9CFi6lp-J5-zMnx3-zaqpLOeNQ0SHNM_C5PuaI5cUurq9h1ijG5D18PWeDduuVncwqlLHMWbLP_e-3X4ThBfO4JeRDt39CDyI3feXwx1bxvPYljs6Nj6RdtBz8rDj260U_46rJfS9RsPYsYItC0v_4pgqzQ0Sn5sTG_NIjoaPPinxSvlrss0eXDNdpUALDl5CJFYHocyITO7nTvUkLbxIscUjDjKgkzZ2t__mi0)



