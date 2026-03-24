# Manual do Usuário IwQuotation

Bem-vindo ao **IwQuotation**, uma aplicação de página única (SPA - Simgle Page Application) para gerenciamento de cotações no sistema IW. Este manual fornece um guia passo a passo sobre como usar o sistema para gerenciar e enviar cotações.

## Sumário
1. [Acessando a Aplicação](#1-acessando-a-aplicação)
2. [Login](#2-login-e-seleção-de-perfil)
3. [A Lista de Mapas de Cotação](#3-a-lista-de-mapas-de-cotação)
4. [Editando uma Cotação](#4-editando-uma-cotação)
    - [4.1 Dados Globais e Frete](#41-dados-globais-e-frete)
    - [4.2 Navegando pelos Itens Solicitados](#42-navegando-pelos-itens-solicitados)
    - [4.3 Inserindo Cotações de Itens](#43-inserindo-cotações-de-itens)
    - [4.4 Salvando e Finalizando](#44-salvando-e-finalizando)
5. [Recursos Adicionais](#5-recursos-adicionais)

---

## 1. Acessando a Aplicação
O módulo IwQuotation é uma parte especializada do sistema IwBrowser3. Ele é acessado por meio de uma URL específica fornecida pelo seu administrador:

`http://[endereco-do-servidor]/IwBrowser/?App=IwQuotation&Profile=[NOME_DO_PERFIL]`

- **App=IwQuotation**: Direciona o sistema para carregar o módulo de cotação.
- **NOME_DO_PERFIL**: Especifica o banco de dado dados a ser acessado na sua sessão.

Obs: é importante usar a URL correta. O IwBrowser possui mais de uma Aplicação embutida nele. Usar a URL incorreta pode carregar o login de outra aplicação que não operacional. Um modo de identificar se é a aplicação IwQuotation (correta)que está sendo acessada, deve aparecer um titulo IwQuotation no top e apenas 2 campos a serem preenchidos pelo usuário (Usuário e senha). Se aparecerem 3 campos é porque está acessando a aplicação incorreta. Quando um navegador acessa a aplicação incorreta, ele costuma gravar informações do acesso que podem fazer com que o navegador, em futuros acessos, mesmo usando-se a URL correta acabe carregando o login da aplicação incorreta. Quando isso ocorrer, todos os navegadores possuem opções de remover dados de acesso gravados. Use essa opção para que o navegador volte a ter a capacidade de acessar o IwQuotation (a aplicação correta). 

## 2. Login
Ao abrir a aplicação, você verá a **Tela de Login do IwQuotation**.

1.  **Usuário:** Digite seu nome de usuário.
2.  **Senha:** Digite sua senha.
4.  **Enviar:** Clique no botão ou pressione "Enter" para fazer o login.
5.  **Trocar Senha:** Use o link "Trocar senha" se precisar atualizar sua senha.

## 3. A Lista de Mapas de Cotação
Após o login bem-sucedido, você verá a **Lista de Mapas de Cotação**. Este painel exibe todas as solicitações de cotação ativas (Mapas) atribuídas à sua empresa/fornecedor que está associada ao seu usuário dentro do sistema IW.

- **Colunas do Grid:** Você pode ver o ID do Mapa, Data de Criação, Prazo de Entrega e detalhes do fornecedor.
- **Selecionando um Mapa:** Clique em qualquer linha do grid para abrir o editor detalhado do respectivo Mapa de cotação.

## 4. Editando uma Cotação
O editor de cotação é um espaço de trabalho completo dividido em várias áreas funcionais.

### 4.1 Dados Globais e Frete
Na parte inferior da janela, você deve preencher os termos gerais da sua proposta:

- **Dados Globais:**
    - **Validade da Proposta:** Até quando sua proposta é válida.
    - **Prazo de Entrega:** O tempo estimado para entrega.
    - **Condição de Pagamento:** Selecione na lista (ex: 30 dias, 60 dias) ou selecione "Outros" para digitar uma condição personalizada.
    - **Compra Mínima:** O valor mínimo de pedido exigido por sua empresa.
    - **Desconto Global:** Qualquer desconto adicional aplicado ao valor total.

- **Informações de Frete:**
    - **Tipo (CIF/FOB):** Selecione se o frete está incluso (CIF) ou por conta do comprador (FOB).
    - **Valor do Frete:** Insira o custo de envio, se aplicável.
    - **Valor Mín. para CIF:** Se você oferece frete grátis acima de um determinado valor, insira esse valor aqui.

### 4.2 Navegando pelos Itens Solicitados
No canto superior esquerdo, você verá o **Grid de Navegação do Mapa**.

- Este grid lista todos os itens que o comprador está solicitando.
- **Coluna "Cotado":** Uma caixa de seleção indica se você já forneceu pelo menos uma cotação válida para aquele item.
- **Seleção:** Clique em um item para ver seus detalhes e inserir seus preços.

### 4.3 Inserindo Cotações de Itens
Quando um item é selecionado, seus detalhes (Descrição, Código e Instruções do Comprador) aparecem no formulário superior central. Você pode fornecer suas cotações no **Grid de Cotações de Itens** (canto inferior esquerdo):

1.  **Marca/Fabricante:** Selecione a marca que você está oferecendo.
2.  **Qtd. Oferecida:** Insira a quantidade que você pode fornecer (o padrão é a quantidade solicitada).
3.  **Embalagem:** Insira quantas unidades vêm em uma embalagem (ex: 10, 100).
4.  **Preço por Emb.:** Insira o preço de uma embalagem completa. O sistema calculará automaticamente o total com base na quantidade.
5.  **Desc. Item:** Aplique um desconto percentual específico para este item, se desejar.
6.  **Observação do Fornecedor:** Use a área de texto à direita para adicionar notas específicas sobre este item (ex: "Oferecida marca substituta").

*Nota: Você pode fornecer até 3 opções diferentes de marca/preço para cada item do mapa.*

### 4.4 Salvando e Finalizando
No canto inferior direito, você encontrará os botões de ação:

- **Salvar:** Salva seu progresso. Você pode fechar a janela e retornar mais tarde para terminar.
- **Salvar e Fechar:** Salva todos os dados e finaliza o mapa de cotação. Use isso apenas quando tiver completado todos os itens.
- **Fechar:** Fecha o editor sem salvar as alterações mais recentes. Abandona a edição do mapa.

## 5. Recursos Adicionais
- **Menu Superior:**
    - **Logout:** Encerra sua sessão com segurança.
    - **Sobre:** Visualize informações da versão.
    - **Manuais:** Acesso rápido aos manuais do usuário e do administrador.
