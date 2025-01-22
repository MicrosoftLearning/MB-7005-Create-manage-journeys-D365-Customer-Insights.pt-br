---
lab:
  title: 'Laboratório 4: Criar uma jornada baseada em gatilho'
---

## Laboratório 4: Criar uma jornada baseada em gatilho 

Neste laboratório, você aprenderá a:
- Criar uma jornada baseada em gatilho
- Definir critérios de saída para o segmento 

### Tarefa 1: Criar uma jornada baseada em gatilho 
1. Navegue até a área de trabalho **Jornadas em tempo real**.

1. Em **Participação**, selecione **Jornadas**.

1. Clique em **+ Nova jornada** na barra de comandos.

1. Selecione **Ignorar e criar do zero**.

1. Em **Nomear a jornada**, insira **Jornada de boas-vindas**.

1. Em **Escolher tipo de jornada**, selecione **Baseada em gatilho.**

1. Em **Escolher um gatilho**, pesquise e selecione **Contato Criado**.

1. Clique em **Criar**.

1. Nas Configurações da jornada à direita, na seção Entrada, selecione **Adicionar condição**.

1. No menu suspenso Atributo, selecione **Contato criado > Contato (Contato) > Conta (Conta) > Nome da Conta**.

1. Altere o operador para **Não é igual**.

1. Defina o valor como **Humongous Insurance**. A condição deve ser o **Nome da conta não é igual a Humongous Insurance**.

1. Configure o restante dos itens na seção Entrada da seguinte maneira:
    - Na seção **Repetir**, selecione Imediatamente.
    - Na seção Fuso horário, escolha seu fuso horário.
    - Em Início, selecione a data de hoje, 15 minutos a partir de agora.
    - Em Encerrar, selecione amanhã.

### Tarefa 2: Definir a meta da jornada
Em seguida, podemos identificar a meta específica da Jornada do Cliente.  As metas ajudam a identificar qual é o ponto final da jornada.  Podem ser coisas como impulsionar uma compra ou interagir com os clientes.  Informar uma meta para a jornada garante que a jornada seja interrompida assim que a meta for alcançada.    

Para esta jornada, estamos procurando uma porcentagem específica das pessoas com quem estamos interagindo para clicar em um link que está em um email que enviamos a elas.  

1.  Nas Configurações da jornada à direita, navegue até a seção **Meta**.

1.  Em **O objetivo desta jornada é**, selecione **Enviar uma notificação geral.**

1.  No campo **A meta é atingida quando**, selecione **Uma pessoa tiver clicado em pelo menos um link**.

1.  Insira **50** em **Número de pessoas necessárias**. Deixe a opção **Porcentagem** selecionada. 

### Tarefa 3: Definir um limite de frequência para a jornada 
A Contoso quer garantir que eles não estejam sobrecarregando os clientes com mensagens comerciais. Para garantir que isso não aconteça, eles querem aplicar um limite de frequência a essa jornada.   

1.  Nas configurações da Jornada à direita, navegue até a seção **Outras configurações**.

1.  Em Limite de frequência, certifique-se de que a opção **Aplicar limite de frequência a esta jornada – ignorar mensagens comerciais se o limite for atingido** esteja selecionada.  

1.  Em Frequência máxima nas jornadas, selecione **Ir para configurações de limite de frequência**. Uma nova janela será aberta.

1.  Na barra de comandos, selecione **+ Nova configuração**.

1.  No campo Nome, insira **Contoso**.

1.  Na seção Frequência máxima por ponto de contato, configure com base na imagem abaixo:

    ![Captura de tela das configurações do limite de frequência, com Email definido como três diários e dez mensais, mensagem de texto definida como um diário, dois semanais e três mensais. Nada há nada definido para notificação por push.](../Labs/Media/frequency-cap.png)

1. Selecione **Salvar e Fechar** para salvar e fechar suas novas configurações de Limite de frequência.  

1.  Retorne à janela que contém a Jornada de boas-vindas. **Salve** a jornada e atualize o navegador.

1.  Nas Configurações da jornada à direita, navegue até a seção **Outras configurações** novamente.

1.  Observe que o Limite de frequência da Contoso agora está aplicado a essa Jornada.  

### Tarefa 4: Criar a jornada baseada em gatilho 
Agora que definimos os critérios de jornada necessários, a próxima etapa é criar as etapas da jornada. 

1. No designer da jornada, clique no ícone de **adição (+)** no bloco Contato criado.

1. Selecione **Ramificação de atributo (ramificação com base em um valor específico).**

1. Em Nome de exibição à direita, insira **Novo Cliente de negócios**.

1. Selecione **Ramificação 1** e em **Escolher um atributo**, procure **Descrição (descrição)** em Contato.

1. Altere o valor de Igual para **Contém**.

1. Em Valor, insira **Negócios**.

1. Clique no **ícone de adição (+)** em Ramificação 1.

1. Selecione **Email: Enviar um email**.

1. Em **Selecionar email**, escolha **Email de boas-vindas 1**.

1. Clique no **ícone de adição (+)** no bloco Enviar um email.

1. Selecione **Aguardar gatilho**.

1. Para configurar a ramificação Se/então, no painel Ramificação Se/então à direita, em Aguardar por, Escolher um tipo de condição de ramificação, selecione A mensagem anterior recebe uma interação.

1. Em **Escolher uma interação**, selecione **Link por email clicado**.

1. Em **Qual é o limite de tempo?**, insira 10 minutos.

1. De volta ao Diagrama da jornada, para especificar o link clicado, selecione **criar ramificações**.

1. Selecione o atributo **Link por email clicado**.

1. Na Ramificação 1, selecione o botão de chamada para ação no email.

1. No caminho Sim, clique no **ícone de adição (+)**.

1. Selecione **Enviar um email**.

1. Em Selecionar e-mail, escolha **E-mail de boas-vindas 2**.

1. No caminho correspondente Não, clique no **ícone de adição (+)**.

1. Selecione **Enviar um email**.

1. Em Selecionar email, escolha **E-mail de boas-vindas 3**.

1. Salve a jornada.

1. Revise a jornada. Faça as alterações finais.

1. Clique em **Publicar**. Aguarde a publicação da jornada.


