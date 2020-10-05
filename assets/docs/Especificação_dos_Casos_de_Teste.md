# **Especificação dos Casos de Teste**
&nbsp;

# UC01 - Autenticação
## TC01 - Autenticação realizada com sucesso

    Descrição:
    Este caso de teste verificará se a autenticação via QRcode foi realizada de maneira correta.

    Pré-condições:
    O usuário deve estar deslogado.

    Pós-condições:
    O usuário deverá estar autenticado no sistema.

    Dados necessários:
    Possuir codigo(QRcode) para comunicação com hardware.

## TC02 - Autenticação com QRcode inválido
    Descrição:
    Este caso de teste verificará se a autenticação está correta e a validade do código(QRcode).

    Pré-condições:
    O usuário deve estar deslogado.

    Pós-condições:
    O usuário deverá ser informado de que o código(QRcode) é inválido.

    Dados necessários:
    Possuir um código(QRcode) válido.

# UC02 - Gerenciar Produção de Cerveja
## TC03 - Inicialização do processo iniciada com sucesso
    Descrição:
    Este caso de teste verificará se o processo de produção da Microcervejaria irá inicializar corretamente.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário deverá ser informado/notificado de que o processo de produção foi iniciado.

    Dados necessários:
    Receitas.

## TC04 - Inicialização do processo de produção inválida
    Descrição:
    Este caso de teste verificará se o processo de produção de Microcervejaria está correta e possui os dados necessários para inicialização.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário deverá ser informado/notificado de que o processo de produção falhou.

    Dados necessários:
    Não se aplica.

## TC05 - Consulta do processo de produção
    Descrição:
    Este caso de teste verificará se a consulta mostrará corretamente o tempo e as temperaturas.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário irá visualizar o tempo e as temperaturas ao longo do processo.

    Dados necessários:
    Tempo e Temperatura.

## TC06 - Cancelar processo de produção com sucesso
    Descrição:
    Este caso de testes verificará se houve sucesso para cancelar o processo de produção de cerveja.

    Pré-condições:
    O usuário deve estar autenticado e ter um processo de produção iniciado e confirmar a opção de cancelar a produção.

    Pós-condições:
    O sistema deve cancelar a produção da produção de cerveja.

    Dados necessários:
    Identificador da receita atual que esta em produção.

## TC07 - Falha para cancelar processo de Produção
    Descrição:
    Este caso de testes verificará se houve insucesso para cancelar o processo de produção de cerveja.

    Pré-condições:
    O usuário deve estar autenticado e ter um processo de produção iniciado e confirmar a opção de cancelar a produção.

    Pós-condições:
    O sistema deve indicar a ocorrência do erro e enviar notificação para o usuário.

    Dados necessários:
    Identificador da receita atual que esta em produção.


# UC03 - Gerenciar Processo de Limpeza
## TC08 - Iniciar Processo de Limpeza com sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para iniciar o processo de limpeza.

  Pré-condições:
  O usuário deve estar autenticado e confirmar o inicio do processo de limpeza e não deve ter um processo de produção de cerveja ocorrendo.

  Pós-condições:
  O sistema deve iniciar o processo de limpeza.

  Dados necessários:
  Não se aplica

## TC09 - Falha ao iniciar processo de limpeza
  Descrição:
  Este caso de testes verificará se houve insucesso para iniciar o processo de limpeza.

  Pré-condições:
  O usuário deve estar autenticado e confirmar o inicio do processo de limpeza enquanto algum processo de produção de cerveja está ocorrendo.

  Pós-condições:
  O sistema deve apresentar uma mensagem de erro e não iniciar a produção da limpeza.

  Dados necessários:
  Não se aplica.

# UC04 - Gerenciar Receitas
## TC10 - Criar Receita com Sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para criar uma receita.

  Pré-condições:
  O usuário deve estar autenticado e solicitar a criação de uma receita.

  Pós-condições:
  Uma nova receita deve ser criada.

  Dados necessários:
  Gerais: Nome, descrição, tempo médio, quantidade de litros e ingredientes(nome, quantidade, unidade de medida)
  Aquecimento: temperatura
  Brassagem: Tempo e temperaturas
  Fervura: Tempo da fervura, ingredientes(tempo para inserir, nome, quantidade, unidade de medida)

## TC11 - Falha para criar receita
  Descrição:
  Este caso de testes verificará se houve insucesso para criação de uma nova receita.

  Pré-condições:
  Usuário deve fornecer os dados solicitados de maneira inválida ou não informa-los.

  Pós-condições:
  O sistema deve apresentar a mensagem de erro mostrando os campos cujo o preenchimento foi inválido e aguardará que o usuário preencha-os novamente e submeta a alteração.

  Dados necessários:
  Gerais: Nome, descrição, tempo médio, quantidade de litros e ingredientes(nome, quantidade, unidade de medida)
  Aquecimento: temperatura
  Brassagem: Tempo e temperaturas
  Fervura: Tempo da fervura, ingredientes(tempo para inserir, nome, quantidade, unidade de medida)

## TC12 - Editar Receita com sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para editar uma receita.

  Pré-condições: O usuário deve estar autenticado, preencher todos os campos de maneira válida e submeter a edição.

  Pós-condições:
  A alteração é feita com sucesso e o usuário é direcionado para a visualização da receita.


  Dados necessários:
  Gerais: Nome, descrição, tempo médio, quantidade de litros e ingredientes(nome, quantidade, unidade de medida)
  Aquecimento: temperatura
  Brassagem: Tempo e temperaturas
  Fervura: Tempo da fervura, ingredientes(tempo para inserir, nome, quantidade, unidade de medida)

## TC13 - Falha para editar receita
  Descrição:
  Este caso de testes verificará se houve insucesso para editar uma receita.

  Pré-condições:
  O usuário deve estar autenticado e preencher os campos de maneira inválida ou não informa-los.

  Pós-condições:
  O sistema deve apresentar a mensagem de erro mostrando os campos cujo o preenchimento foi inválido e aguardará que o usuário preencha-os novamente e submeta a alteração.

  Dados necessários:
  Gerais: Nome, descrição, tempo médio, quantidade de litros e ingredientes(nome, quantidade, unidade de medida)
  Aquecimento: temperatura
  Brassagem: Tempo e temperaturas
  Fervura: Tempo da fervura, ingredientes(tempo para inserir, nome, quantidade, unidade de medida)

## TC14 - Excluir Receita com sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para excluir uma receita.

  Pré-condições:
  O usuário deve estar autenticado e solicitar a exclusão de uma receita.

  Pós-condições:
  O sistema informa uma mensagem de sucesso e redireciona para a página principal.

  Dados necessários:
  Identificador da receita que se deseja excluir(nome).

## TC15 - Falha para excluir receita
  Descrição:
  Este caso de testes verificará se houve insucesso para excluir a receita.

  Pré-condições:
  O usuário deve estar autenticado e solicitar a exclusão.

  Pós-condições:
  O sistema deve tratar o erro e apresentar uma mensagem para o usuário na tela.


  Dados necessários:
  Identificador da receita que se deseja excluir(nome).

## TC16 - Visualizar Receita com sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para visualizar uma receita especifica.

  Pré-condições:
  O usuário deve estar autenticado e solicitar a receita que deseja visualizar.

  Pós-condições:
  A receita deve ser apresentada com sucesso para o usuário.


  Dados necessários:
  Identificador da receita que se deseja visualizar(nome).

## TC17 - Falha para visualizar receita
  Descrição:
  Este caso de testes verificará se houve insucesso para visualizar uma receita especifica.

  Pré-condições:
  O usuário deve estar autenticado e solicitar a receita que deseja visualizar.

  Pós-condições:
  O sistema deve tratar o erro e apresentar para o usuário a mensagem na tela.

  Dados necessários:
  Identificador da receita que se deseja visualizar(nome).

## TC18 - Visualizar lista de Receitas com sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para visualizar a lista de receitas com sucesso.

  Pré-condições:
  Usuário deve estar autenticado e entrar na página inicial com a lista de todas as receitas.

  Pós-condições:
  Deve apresentar a lista de todas as receitas do usuário.

  Dados necessários:
  Não se aplica

## TC19 - Falha para visualizar lista de receitas
  Descrição:
  Este caso de testes verificará se houve insucesso para visualizar a lista de receitas.

  Pré-condições:
  Usuário estar autenticado e entrar na página inicial.

  Pós-condições:
  Sistema deve tratar o erro e apresentar a mensagem para o usuário na tela.

  Dados necessários:
  Não se aplica

# UC05 - Gerenciar Notificações
## TC20 - Enviar Notificação com Sucesso
  Descrição:
  Este caso de testes verificará se houve sucesso para enviar uma notificação.

  Pré-condições:
  Usuário ter autorizado o recebimento de notificações push.

  Pós-condições:
  Usuário deve receber uma notificação no seu dispositivo.

  Dados necessários:
  Mensagem da notificação

## TC21 - Falha para enviar notificação
  Descrição:
  Este caso de testes verificará se houve insucesso para o envio de notificação.

  Pré-condições:
  Usuário não autorizou recebimento de notificações push.

  Pós-condições:
  A notificação não deve ser enviada.

  Dados necessários:
  Mensagem da notificação
