# leitura

* [Overview](#Overview)
  * [Aplicativo de leitura](#Aplicativo-de-leitura)
    * [Components](#Components)
    * [Container](#Container)

---

## Overview

![diagram](https://www.plantuml.com/plantuml/svg/0/hLEnRjim4DqD-1ykdXmWiPPEdM8uHXF0IGF7QP59k8W7vm2ALCYZc-PlF1KTElKJz6Cb9Sk2cwHJ9v7lxjvxVAJElA2JKEhXu8XDeOCYU1If_CSiS_XjicPv30_1aoki4J8oAMoPeNACPgD35RBPXzCRZKRkhXQPHY4l4SfdgVjP9bL3FHmiflUVxrRvrylLHRwOVvfVdu-F4tv3pbipdefr-OeAmuND5yGI74Td9p1A5LZLFviIzALHh2sfSkIZAGGBqlL4gBB6rziDQQX88-Xc2a5P3oKfLZRsJ4R7dNm-VvRMmanpfADETxTzfLMqE3m5WY2i-IMY7c9A6wv_n5LCSLrl_GdKstL08D3XvKt1VAfADl503bNIjqRP1DZEma4zyROjzQ_OyygNPwDI13R43HvC5lqOD4vkltkXSdpBwPEItgtU86tmfBqFaleStp_hSB0a_VxLzifBmYR27RrFm_lH_PNq_L_OXtR2nUkL-hVZDlDuI1zA6pruMWUZ43RSk7smciGU4lyZ-lyerL7zzRpc9hNJQOciFLJei4tiZ8ngVfa_)

**Level 1: System Context diagram**

A System Context diagram is a good starting point for diagramming and documenting a software system, allowing you to step back and see the big picture. Draw a diagram showing your system as a box in the centre, surrounded by its users and the other systems that it interacts with.

Detail isn't important here as this is your zoomed out view showing a big picture of the system landscape. The focus should be on people (actors, roles, personas, etc) and software systems rather than technologies, protocols and other low-level details. It's the sort of diagram that you could show to non-technical people.

**Scope**: A single software system.

**Primary elements**: The software system in scope.
Supporting elements: People (e.g. users, actors, roles, or personas) and software systems (external dependencies) that are directly connected to the software system in scope. Typically these other software systems sit outside the scope or boundary of your own software system, and you don’t have responsibility or ownership of them.

**Intended audience**: Everybody, both technical and non-technical people, inside and outside of the software development team.





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
