# Container

`\Aplicativo de leitura\Container`

* [Overview](../../README.md)
  * [Aplicativo de leitura](../../Aplicativo%20de%20leitura/README.md)
    * [Components](../../Aplicativo%20de%20leitura/Components/README.md)
    * [**Container**](../../Aplicativo%20de%20leitura/Container/README.md)
    * [Fluxo](../../Aplicativo%20de%20leitura/Fluxo/README.md)
      * [DiagramaSequencia](../../Aplicativo%20de%20leitura/Fluxo/DiagramaSequencia/README.md)

---

[Aplicativo de leitura (up)](../../Aplicativo%20de%20leitura/README.md)

---

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
