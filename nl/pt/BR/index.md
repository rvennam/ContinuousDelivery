---

copyright:
  years: 2015, 2017
lastupdated: "2017-5-19"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Introdução à entrega contínua
{: #cd_getting_started}

Adote uma abordagem DevOps usando o {{site.data.keyword.contdelivery_full}}, que inclui cadeias de ferramentas abertas que automatizam a construção e a implementação de aplicativos. É possível começar criando uma cadeia de ferramentas de implementação simples que suporte as tarefas de desenvolvimento, implementação e operações.
{: shortdesc}

Depois de criar uma instância do {{site.data.keyword.contdelivery_short}} selecionando-a no catálogo do {{site.data.keyword.Bluemix_notm}}, é possível escolher como você deseja começar o serviço.
![Página de boas-vindas do Continuous Delivery](images/cd_landing_page.png)

* Para iniciar rapidamente e implementar seu aplicativo usando um pipeline
automatizado, na seção "Iniciando com um pipeline", clique em
**[Iniciar aqui](#starting_with_a_pipeline)**. Posteriormente,
será possível incluir mais ferramentas.
* Para criar e configurar uma cadeia de ferramentas de entrega contínua a partir
de um modelo, na seção "Iniciando a partir de um modelo de cadeia de ferramentas", clique
em **[Iniciar aqui](#starting_from_a_toolchain_template)**. A
cadeia de ferramentas integra ferramentas para planejar, desenvolver, implementar
pipelines e gerenciar aplicativos. Sempre é possível incluir ou remover ferramentas de
suas cadeias de ferramentas.
* Se você já tiver cadeias de ferramentas, na seção "Iniciando a partir de
um modelo de cadeia de ferramentas", clique em **Visualizar suas cadeias de
ferramentas**. Para obter mais informações sobre como trabalhar com cadeias de ferramentas, veja [Usando cadeias de ferramentas](/docs/services/ContinuousDelivery/toolchains_using.html){: new_window}.

**Dica**: os pipelines são gerenciados pelas cadeias de ferramentas. É possível incluir um pipeline em uma cadeia de ferramentas existente. Se você criar um pipeline e não tiver cadeias de ferramentas existentes, uma cadeia de ferramentas com um nome padrão será criada. Com a cadeia de ferramentas, é possível expandir os recursos de seu pipeline pela integração com outras ferramentas e serviços.

##Visão geral do {{site.data.keyword.contdelivery_short}}
{: #cd_overview}

Com o {{site.data.keyword.contdelivery_short}}, é possível construir, testar
e entregar aplicativos usando práticas DevOps e ferramentas líderes de mercado.
{:shortdesc}

O serviço de {{site.data.keyword.contdelivery_short}} suporta seus fluxos de trabalho DevOps:

 * É possível criar [cadeias de ferramentas](/docs/services/ContinuousDelivery/toolchains_about.html){: new_window} abertas DevOps integradas para permitir integrações de ferramentas que suportem suas tarefas de desenvolvimento, implementação e operações.

  Uma cadeia de ferramentas é um conjunto integrado de ferramentas que podem ser usadas para desenvolver, construir, implementar, testar e gerenciar aplicativos de forma colaborativa e tornar as operações repetíveis e mais fáceis de gerenciar. As cadeias de ferramentas podem incluir ferramentas de software livre, serviços do {{site.data.keyword.Bluemix_notm}}, como [{{site.data.keyword.DRA_full}}](/docs/services/ContinuousDelivery/di_working.html){: new_window} e ferramentas de terceiros, como GitHub, PagerDuty e Slack. 

 * Entregue continuamente usando pipelines [pipelines](/docs/services/ContinuousDelivery/pipeline_about.html){: new_window} automatizados.

  Automatize construções, testes de unidade, implementações etc. Construa, teste e implemente repetidamente, com mínima intervenção humana. Esteja pronto para liberar para a produção a qualquer momento.

 * Edite e envie por push seu código de qualquer lugar usando o [IDE baseado na web](/docs/services/ContinuousDelivery/web_ide.html){: new_window}.

  Crie, edite, execute e depure, bem como conclua as tarefas de controle de fonte
no GitHub. Mova sem problemas da edição do seu código para a implementação dele
em produção. 
  
 * Colabore com sua equipe e gerencie seu código-fonte com um [repositório Git (repos) e rastreador de problemas](/docs/services/ContinuousDelivery/git_working.html#git_working){: new_window} que é hospedado pela IBM e construído no GitLab Community Edition.

  Gerencie repositórios Git por meio de controles de acesso de baixa granularidade que mantêm o código seguro. Revise o código e aprimore a colaboração por meio de solicitações de mesclagem. Rastreie problemas e compartilhe ideias por meio do rastreador de problemas. Documente projetos no sistema wiki.

##Iniciando com um pipeline
{: #starting_with_a_pipeline}

Os pipelines automatizam construções, implementações e muito mais. Para iniciar com um pipeline automatizado, selecione um modelo e forneça o local de seu repositório GitHub (repo).

Para [criar um pipeline ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/devops/pipelines/dashboard/create){:new_window} que esteja configurado para implementar um aplicativo Cloud Foundry, siga estas etapas:

1. Clique em **Cloud Foundry**.
1. Se você desejar usar um nome diferente para o pipeline, mude o nome padrão. O
nome do pipeline o identifica no {{site.data.keyword.Bluemix_notm}}.
1. Se você desejar usar um nome diferente para o aplicativo, mude o nome padrão. O
nome do aplicativo o identifica no {{site.data.keyword.Bluemix_notm}}. Esse nome é o aplicativo no qual o pipeline é implementado.
1. Se você não tiver uma cadeia de ferramentas, será criada uma com um nome padrão. Se você desejar usar um nome diferente para a cadeia de ferramentas, mude o nome. Os
pipelines são gerenciados pelas cadeias de ferramentas. Com a cadeia de ferramentas, é possível ampliar os recursos de seu pipeline por meio da integração com outras ferramentas e serviços.

 **Dica**: os pipelines e as cadeias de ferramentas pertencem às
organizações (orgs). Se você pertencer a uma organização que tenha cadeias de ferramentas,
será possível usar essas cadeias de ferramentas mesmo que você não as tenha criado.

1. Selecione a cadeia de ferramentas que deseja usar ou digite um nome para a nova cadeia de ferramentas que deseja criar.
1. Selecione seu provedor Git.

 **Dica**: se o {{site.data.keyword.Bluemix_notm}} não estiver autorizado a acessar a sua conta do GitHub, você será solicitado a clicar em **Autorizar** para acessar o website GitHub. Se você não
tiver uma sessão GitHub ativa, será solicitado que efetue login. Clique em **Autorizar aplicativo** para permitir que o {{site.data.keyword.Bluemix_notm}} acesse sua conta GitHub.

 Se você não estiver autorizado a acessar o repositório {{site.data.keyword.ghe_short}}, alguém que tenha privilégios de administrador para o repositório deverá incluí-lo. Para obter instruções de autorização com o {{site.data.keyword.Bluemix_notm}} Dedicated for {{site.data.keyword.ghe_short}}, veja [Introdução ao {{site.data.keyword.Bluemix_notm}} Dedicated for {{site.data.keyword.ghe_short}}](/docs/services/ghededicated/index.html){: new_window}. Se for necessário autorizar com sua própria versão gerenciada do {{site.data.keyword.ghe_short}}, siga seus procedimentos internos.

    * Se você tiver um repositório e desejar usá-lo, para o tipo de repositório, selecione **Link**. Procure o local do repositório e
selecione-o na lista de repositórios disponíveis.

    * Se desejar criar um repositório vazio, para o tipo de repositório, selecione **Novo**. Digite um nome para o repositório.

    * Se desejar criar um clone de um repositório, para o tipo de repositório, selecione **Copiar**. Procure o local do repositório e
selecione-o na lista de repositórios disponíveis.

    * Se desejar bifurcar um repositório para que possa contribuir com mudanças por meio de solicitações pull, selecione **Bifurcar**. Procure o local do repositório e
selecione-o na lista de repositórios disponíveis.

1. Selecione um repositório ou insira uma URL de repositório.
1. Clique em **Criar**. O pipeline é criado, configurado e exibido na página Visão Geral da cadeia de ferramentas. ![Placa do Pipeline](images/cd_pipeline.png)

Para criar um [pipeline vazio ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/devops/pipelines/dashboard/create){: new_window} sem nenhum estágio pré-configurado:

1. Clique em **Customizado**.
1. Se você desejar usar um nome diferente para o pipeline, mude o nome padrão. O
nome do pipeline o identifica no {{site.data.keyword.Bluemix_notm}}.
1. Se você não tiver uma cadeia de ferramentas, será criada uma com um nome padrão. Se você desejar usar um nome diferente para a cadeia de ferramentas, mude o nome. Os
pipelines são gerenciados pelas cadeias de ferramentas. Com a cadeia de ferramentas, é possível ampliar os recursos de seu pipeline por meio da integração com outras ferramentas e serviços.
1. Selecione a cadeia de ferramentas que deseja usar ou digite um nome para a nova cadeia de ferramentas que deseja criar.
1. Clique em **Criar**. Um pipeline vazio é criado e representado como um cartão na página Visão geral da cadeia de ferramentas.

##Iniciando a partir de um modelo de cadeia de ferramentas
{: #starting_from_a_toolchain_template}

Para criar e configurar uma cadeia de ferramentas de entrega contínua por meio de um [modelo ![Ícone de link externo](../../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/devops/create){: new_window}:

1. Na página **Criar uma cadeia de ferramentas**, clique em um
modelo de cadeia de ferramentas.
1. Revise o diagrama da cadeia de ferramentas que você está prestes a criar. O diagrama
mostrará cada integração de ferramenta em sua fase de ciclo de vida na cadeia de ferramentas.

 **Dica**: alguns dos modelos de cadeia de ferramentas têm múltiplas instâncias de uma integração de ferramenta. Por exemplo, o modelo de cadeia de ferramentas de Microsserviços no {{site.data.keyword.Bluemix_notm}} Public contém três instâncias do GitHub e três instâncias do Delivery Pipeline, uma para cada um dos três microsserviços.

 O diagrama na imagem a seguir é um exemplo. Ao criar uma cadeia de ferramentas, o diagrama mostra cada integração de ferramenta que faz parte da cadeia de ferramentas.
 ![Toolchain_diagram](images/toolchain_diagram.png)
1. Revise as informações padrão para as configurações da cadeia de ferramentas. O nome da cadeia de ferramentas as identifica em
{{site.data.keyword.Bluemix_notm}}. Se você desejar usar um nome diferente, mude
o nome da cadeia de ferramentas.
1. Na seção Integrações de ferramentas, selecione cada integração de ferramenta que deseja configurar para sua cadeia de ferramentas. Algumas integrações de ferramentas não requerem configuração. Para obter informações sobre como configurar as integrações de ferramentas, consulte
[Configurando
integrações de ferramentas](/docs/services/ContinuousDelivery/toolchains_integrations.html){: new_window}.
1. Clique em **Criar**. Várias etapas são executadas automaticamente para configurar sua cadeia de ferramentas. As integrações de ferramentas configuradas são diferentes, dependendo de qual modelo de cadeia de ferramentas você selecionou e se está usando o {{site.data.keyword.Bluemix_notm}} Public ou o {{site.data.keyword.Bluemix_notm}} Dedicated. Por exemplo, quando você cria uma cadeia de ferramentas de Microsserviços no {{site.data.keyword.Bluemix_notm}} Public, estas etapas são executadas:

 * A cadeia de ferramentas é criada.
 * Se você tiver configurado o Delivery Pipeline, os pipelines serão criados e executados.
 * Se você tiver configurado o Sauce Labs, a cadeia de ferramentas será configurada para incluir tarefas de teste do Sauce Labs nos pipelines.
 * Se tiver configurado o PagerDuty, a cadeia de ferramentas será configurada para enviar notificações de alerta para o serviço PagerDuty especificado.
 * Se tiver configurado o Slack, a cadeia de ferramentas será configurada para enviar notificações sobre o status de implementação para o canal Slack especificado.
 * Se tiver configurado a integração de ferramenta do código-fonte, como o GitHub, o repositório GitHub de amostra será clonado na conta do GitHub.
