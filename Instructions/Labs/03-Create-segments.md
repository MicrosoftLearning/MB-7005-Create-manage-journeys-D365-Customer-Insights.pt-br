---
lab:
  title: 'Laboratório 2: Criar segmentos'
---

## Laboratório 2: Criar segmentos 

Neste laboratório, você aprenderá a:
- Atualizar informações sobre registros de clientes
- Criar um segmento 

### Tarefa 1: Atualizar a cidade para diferentes clientes

Uma das jornadas terá como alvo clientes que moram em uma cidade específica. Para garantir que você terá membros neste segmento, precisamos adicionar uma cidade a cada um dos contatos que existem atualmente.

1. Faça logon no **Dynamics 365 Customer Insights - Journeys**. Certifique-se de estar na **área Jornadas em tempo real**.

1. Em Público, selecione **Contatos**.

1. Selecione os dez primeiros contatos na lista. 

1. Na barra de comandos, selecione **Editar**.

1. No campo Endereço 1: Cidade, insira **Seattle**.

1. Selecione o botão **Salvar**.

1. Selecione os próximos 50 contatos na lista.

1. Na barra de comandos, selecione **Editar**.

1. No campo Endereço 1: Cidade, insira **Portland**.

1. Selecione o botão **Salvar**.

1. Selecione os próximos dez contatos na lista.

1. Na barra de comandos, selecione **Editar**.

1. No campo Endereço 1: Cidade, insira **Boise**.

1. Selecione o botão **Salvar**.

1. Selecione os próximos dez contatos na lista.

1. Na barra de comandos, selecione **Editar**.

1. No campo Endereço 1: Cidade, insira **Seattle**.

1. Alterne para a guia **Detalhes**. Na caixa de texto em **Observações pessoais**, insira **Negócios**.

1. Selecione o botão **Salvar**.

### Tarefa 2: Criar um segmento para clientes da Humongous Insurance

1. Navegue até **Segmentos**, no grupo Público-alvo.

1. Selecione **+ Novo segmento**.

1. Na caixa **Nomear o segmento**, insira **Humongous Insurance**. Selecione **Contato** como público-alvo. Selecione **Criar**.

1. Selecione **Adicionar um novo grupo** no designer de segmento. Primeiro, escolheremos um **grupo de atributos**.

1. No painel Atributos, expanda **Contato** e selecione **Conta**. Adicione o item ao grupo existente.

1. Na pesquisa no Grupo 1, selecione **Humongous Insurance**. A condição do Grupo 1 será "A conta é Humongous Insurance".

1. Queremos adicionar outra condição ao segmento. Selecione **+Adicionar novo** para adicionar um novo grupo e selecione **Grupo de atributos**.

1. Altere o operador para **ou**.
    - No painel Atributo, comece a digitar **Email**. Expanda **Contato**. Clique no botão de **adição** ao lado do campo de email e adicione-o ao Grupo 2.
    - Crie a seguinte condição: **O email contém humongousinsurance**

1. Selecione **Salvar**.

1. Selecione **Pronto para usar** na barra de ferramentas.

1. Selecione a guia **Membros e Insights**. Verifique se você vê contatos com um email da Humongous Insurance ou o nome da empresa Humongous. Pode ser necessário atualizar ou aguardar alguns minutos antes que os contatos apareçam.

### Tarefa 3: Criar um segmento de usuário empresarial

1. Navegue até **Segmentos** no grupo Público-alvo.

1. Selecione **+ Novo segmento**.

1. Nomeie o segmento como **Clientes empresariais**. Mantenha **Contato** selecionado como público-alvo. Selecione **Criar**.

1. No painel **Atributos**, expanda **Contato** e selecione **Conta**. Adicione o item a um grupo existente.

1. Na pesquisa no Grupo 1, selecione **Contoso, Ltd**.

1. Selecione **Salvar** e **Pronto para usar**.

1. Aguarde a construção do segmento.

1. Selecione a guia **Membros e insights** para exibir os membros do segmento.

### Tarefa 4: Criar um segmento da Contoso  
2.  Navegue até **Segmentos** no grupo Público-alvo. 

3.  Selecione**+Novo segmento. **

4.  Nomeie o segmento como **Clientes da Contoso**. Mantenha **Contato** selecionado como público-alvo. Selecione **Criar**.

5.  Adicione um novo grupo e selecione **Criar grupo de atributos**. No painel **Atributos**, expanda **Contato** e adicione **Descrição** ao Grupo 1. 

6.  No designer de segmento, altere o qualificador para **Contém**. No valor, insira **Negócios**.

7.  Selecione **Salvar** e **Pronto para usar**. 

8.  Aguarde a construção do segmento. 

9.  Selecione a guia **Membros e insights** para exibir os membros do segmento. 


### Tarefa 5: Criar um segmento de clientes de Seattle
1. Navegue até Segmentos no grupo Público-alvo.

1. Selecione **+ Novo segmento**.

1. Nomeie o segmento como **Clientes de Seattle**. Mantenha **Contato** selecionado como público-alvo.

1. Selecione o botão **Criar**.

1. Adicione um novo grupo e selecione **Criar grupo de atributos**. No painel Atributos, expanda **Contato > Endereço 1** e adicione **Endereço 1: Cidade** ao Grupo 1.

1. No designer de segmento, deixe o qualificador como está. No valor, insira **Seattle**.

1. Selecione **Salvar** e **Pronto para usar**.

1. Aguarde a construção do segmento.

1. Selecione a guia **Membros e insights** para exibir os membros do segmento.
