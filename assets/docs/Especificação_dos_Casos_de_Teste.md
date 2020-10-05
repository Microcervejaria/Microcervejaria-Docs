# **Especificação dos Casos de Teste** 
&nbsp;

# UC1 - Autenticação
## TC01 - Autenticação realizada com sucesso
   
    Descrição:
    Este caso de teste verificará se a autenticação via QRcode foi realizada de maneira correta.

    Pré-condições:
    O usuário deve estar deslogado.

    Pós-condições:
    O usuário deverá estar autenticado no sistema.

    Dados necessários:
    Possuir codigo(QRcode) para comunicação com hardware

## TC02 - Autenticação com QRcode inválido
    Descrição:
    Este caso de teste verificará se a autenticação está correta e a validade do código(QRcode)

    Pré-condições:
    O usuário deve estar deslogado.

    Pós-condições:
    O usuário deverá ser informado de que o código(QRcode) é inválido.

    Dados necessários:
    Possuir um código(QRcode) válido

# UC2 - Iniciar Processo
## TC03 - Inicialização do processo iniciada com sucesso
    Descrição:
    Este caso de teste verificará se o processo de produção da microcervejaria irá inicializar corretamente.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário deverá ser informado/notificado de que o processo de produção foi iniciado.

    Dados necessários:
    Receitas

## TC04 - Inicialização do processo de produção inválida
    Descrição:
    Este caso de teste verificará se o processo de produção de microcervejaria está correta e possui os dados necessários para inicialização.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário deverá ser informado/notificado de que o processo de produção falhou.

    Dados necessários:
    Não se aplica

## TC05 - Consulta do processo de produção 
    Descrição:
    Este caso de teste verificará se a consulta mostrará corretamente o tempo e as temperaturas.

    Pré-condições:
    O usuário deve estar Autenticado.

    Pós-condições:
    O usuário irá visualizar o tempo e as temperaturas ao longo do processo

    Dados necessários:
    Tempo e Temperatura