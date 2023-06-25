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
