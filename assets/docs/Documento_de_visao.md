# Documento de Visão

## 1. Introdução
### 1.1 Propósito
Este documento tem como objetivo trazer as definições e características, do sistema que será utilizado na Microcervejaria Automatizada. Definindo o escopo para que toda equipe possa ter conhecimento pertinente ao mesmo, e assim facilitar o desenvolvimento do software em questão, além de definições a respeito das funcionalidades, e público alvo.

### 1.2 Escopo
Sendo um projeto de Microcervejaria Automatizada desenvolvido durante matéria de Projeto Integrador II,na Faculdade do Gama da Universidade de Brasília, o projeto e necessitará de um interface pela qual o usuário possa obter informações e fazer o controle da mesma.
O sistema tem como finalidade acompanhamento e controle da Microcervejaria automatizada. Trazendo informação sobre o processo, seu estado, e quando necessário trazer alerta ao usuário sobre alguma necessidade de intervenção humana, problema durante a produção e finalização dos processos. Podendo o usuário inserir novas receitas e assim ajustar a rampa de temperatura de acordo com sua necessidade.

### 1.3  Referências

A Estrutura de tópicos do Documento de Visão. IBM Knowledge Center. Disponível em : <https://www.ibm.com/support/knowledgecenter/pt-br/SSYMRC_7.0.2/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html> Acesso em : 06/09/2020

MIT License <https://mit-license.org/> acessador em 09/09/2020

### 1.4 Visão Geral 
Este documento terá como finalidade trazer uma melhor noção das necessidade e características do projeto e os requisitos  que serão precisos para seu desenvolvimentos facilitando assim a tomada de decisões na construção e implementação da aplicação. Estando dividido nos seguintes tópicos: posicionamento, restrições, faixa de qualidade, procedência e prioridade, requisitos e documentação do produto e apêndice.

## 2. Posicionamento
### 2.1 Oportunidade de Negócio
A produção de cerveja artesanal é um processo demorado e com muitos cuidados em relação a temperatura e tempo em cada etapa. Necessitando de uma aplicação que pudesse ser integrada às panelas que possuíssem um sistema de controle destas características, trazendo ao o usuário o status da produção e o dando um controle de forma remota.

### 2.2 Instrução de Posição do Problema

<table>
<tr>
<td>
Problema
</td>
<td>
Alta necessidade do controle de temperatura e tempo de cada etapa do processo de produção de cerveja artesanal, e necessidade de intervenção humana em outros processos
</td>
</tr>

<tr>
<td>
Funções afetadas
</td>
<td>
Intervenção humana no controle da temperatura, e na preocupação do produtor quanto ao que fazer em cada etapa
</td>
</tr>

<tr>
<td>
Impacto do problema 
</td>
<td>
Desvios em temperaturas, inserir ou retirar ingredientes em momentos errados
</td>
</tr>

<tr>
<td>
Solução
</td>
<td>
Desenvolvimento de um aplicação pela qual possa se ter status do processo, a temperatura necessária e tempo a qual a mesma será aplicada, e notificar ao usuário quando houver necessidade de se inserir ou retirar algo, além das notificações de erro caso ocorram.
</td>
</tr>
</table>

### 2.3 Instrução de Posição do Produto

<table>
<tr>
<td>
Para
</td>
<td>
Produtor artesanal de cerveja o qual faça a decisão de utilizar a Microcervejaria
</td>
</tr>

<tr>
<td>
Carências
</td>
<td>
Necessidade de uma aplicação onde traz status da produção, além de notificar usuário quando necessitar de intervenção

</td>
</tr>

<tr>
<td>
Solução 
</td>
<td>
Aplicação da Microcervejaria
</td>
</tr>

<tr>
<td>
Descrição da Solução
</td>
<td>
Ferramenta que traga informações sobre o processo no qual está sendo feito no momento, notificar usuários quando houver necessidade de intervenção(adicionar ou retirar algo do processo).Além do usuário pôder adicionar a própria receita com temperaturas e tempos diferentes de cada processo
</td>
</tr>

<tr>
<td>
Diferenciais 
</td>
<td>
A aplicação da Microcervejaria se destaca por trazer informações a respeito do processo, notificar usuário e deixar  com que o mesmo adicione uma nova receita

</td>
</tr>
</table>

## 3. Descrição dos Envolvidos e Usários

Os envolvidos começar por ser grupo de alunos de Projeto integrador 2 responsável pelo projeto de Microcervejaria, os professores avaliadores desta matéria. Clientes finai, os quais poderão construir sua Microcervejaria e assim fazer uso da aplicação fornecida.

### 3.1 Resumo de parte Interessada
| Nome | Descrição | Responsabilidade |
|------| ----------| -----------------|
| Professores| Avaliadores| Orientar e avaliar ao decorrer dos Pontos de Controle da matéria.|
|Equipe | Graduandos  em Engenharias: Aeroespacial,Automotiva, Eletrônica, Energia e Software da Universidade de Brasília, que compõe o grupo da Microcervejaria | Pessoal responsável pela criação de documentos, organização do grupo e quando necessário elaboração e implementação da aplicação|
| Cliente | Usuários finais da Microcervejaria e aplicação | Utilização e quando necessário manipulação de informações que serão necessárias (criação de receitas)|

### 3.2  Resumo dos Usuários

<table>
<tr>
<td>
Nome
</td>
<td>
Descrição
</td>
<td>
Responsabilidade
</td>
<td>
Envolvidos
</td>
</tr>

<tr>
<td>
Cervejeiros produtores de cervejas artesanais
</td>
<td>
Acessar aplicação, ler informações, adicionar novas receitas, receber alertas.
</td>
<td>
- Inclusão e exclusão no sistema de novas receitas       
- Visualizar informações sobre processo.
- Visualizar informações sobre temperatura e tempo decorrente
</td>
<td>
Clientes finais da aplicação
</td>
</tr>
</table>

### 3.3 Ambiente de Usuário
 O acesso da aplicação será feita via app mobile, e pela plataforma Alexa (Amazon)

 ### 3.4 Principais Necessidades dos Usuários ou dos Envolvidos
 | Necessidades | Preocupações |
 |--------------|------------- |
 |Acesso a informações sobre microcervejaria| Temperatura e tempo de cada processo|
 |Adicionar ou deletar receitas | Nas receitas são necessários campos relacionados ao tempo e temperatura de cada etapa(rampa de temperatura)|
 |Iniciar ou pausar/parar processos | Além de seguir o processo comum da produção de cerveja, haverá um processo que engloba a limpeza do equipamento, caso haja necessidade o usuário além de ter a opção de iniciar tais processos pela aplicação, conseguirá parar os mesmo.|

### 3.5 Perfis das Partes Interessadas
#### 3.5.1 Usuário  do Aplicativo
<table>
<tr>
<td>
Representantes
</td>
<td>
Produtores de cervejas artesanais utilizadores da Microcervejaria

</td>
</tr>
<tr>
<td>
Descrição
</td>
<td>
Usuário que farão uso dos equipamentos e da Aplicação da Microcervejaria 
</td>
</tr>
<tr>
<td>
Tipo
</td>
<td>
Usuário informal
</td>
</tr>
<tr>
<td>
Responsabilidades
</td>
<td>
Utilizar a aplicação de forma que possa ter controle e ter informações sobre Microcervejaria de forma remota, e adicionar receitas

</td>
</tr>
<tr>
<td>
Critérios de Sucesso
</td>
<td>
Estar ligado às notificações que a aplicação gera. 
</td>
</tr>
<tr>
<td>
Envolvimento
</td>
<td>
Alto
</td>
</tr>
<tr>
<td>
Entregas
</td>
<td>
-----
</td>
</tr>
<tr>
<td>
Comentários ou Problemas
</td>
<td>
----
</td>
</tr>
</table>

### 3.6 Perfil de Usuário
#### 3.6.1  Produtor Artesanal- Usuário

<table>
<tr>
<td>
Representantes
</td>
<td>
Usuário

</td>
</tr>
<tr>
<td>
Descrição
</td>
<td>
Produtor artesanal de cerveja usuário da Microcervejaria
</td>
</tr>
<tr>
<td>
Tipo
</td>
<td>
Usuário final
</td>
</tr>
<tr>
<td>
Responsabilidades
</td>
<td>
Inserir novas receitas, receber notificações, interferir no processo quando necessário (notificado)


</td>
</tr>
<tr>
<td>
Critérios de Sucesso
</td>
<td>
Ser capaz de agir quando aplicação exigir

</td>
</tr>
<tr>
<td>
Envolvimento
</td>
<td>
Alto
</td>
</tr>
<tr>
<td>
Entregas
</td>
<td>
Inserir(Água, Mosto, Lúpulo) ou retirar(mosto) algo do equipamento quando solicitado

</td>
</tr>
<tr>
<td>
Comentários ou Problemas
</td>
<td>
----
</td>
</tr>
</table>

### 3.7 Principais Necessidades da Parte Interessada ou dos Usuários
|Necessidade | Prioridade | Interesses | Solução Atual | Solução Porposta|
|----------|----------|---------|---------|--------|
|Acompanhar remotamente processo| Alta |Permitir que usuário saiba qual processo está sendo executado no momento |Acompanhamento presencial|Através de sensores ter indicação de qual processo está sendo executado|
|Parar Processo remotamente|Alta|Permitir que usuário pare o processo quando desejar|Exigia parar manualmente|Existir um botão que pare o processo|
|Iniciar processo Remotamente| Alta|Permitir que usuário inicie o processo quando desejar|Exigia iniciar manualmente|Um botão onde inicia-se o processo|
|Iniciar ou parar processo de limpeza remotamente |Alta|Permitir que o usuário tenha controle sobre começar ou parar o processo remotamente|Exigir que usuário limpasse máquina manualmente |Uma aba que indicasse limpeza, e dentro dela ter botão de Iniciar ou parar|
|Adicionar receitas no App| Média| Permitir que usuário possa adicionar receitas e suas rampas de temperaturas(temperatura e tempo)|O usuário ficava encarregado de controlar a temperatura e tempo em cada receita| Uma aba para adicionar tais características|

## 4. Visão Geral do Produto
### 4.1 Perspectiva do Produto
O sistema utilizado na Microcervejaria será um app mobile .As funções se dão em acessar ao microcontrolador ,acessar o estado em que se encontra os sensores e assim ter acesso em qual etapa está, criar uma nova receita ( podendo adicionar ingredientes necessários e tempo e temperatura aplicada em cada etapa assim como os tempos de repouso), gerenciar o processo de limpeza( podendo iniciar ou parar o mesmo) . Para tudo será necessário ter acesso ao microcontrolador.

### 4.2 Resumo das Capacidades

| Benefício para Cliente | Recurso|
|------------------------|---------|
|Acessar a etapa em que a produção está|Funcionalidade de status atual, acessível a qualquer instante.|
|Estimar para fim da etapa| Funcionalidade mostrando o tempo (temporizador) que falta até a conclusão da etapa.|
|Verificar temperatura atual da panela|Acesso ao estado momentâneo do sensor de temperatura|
|Iniciar/Parar processo de limpeza remotamente| Acesso ao controlador |
| Gerenciar Receitas | Acesso ao banco de dados, podendo inserir uma nova,alterar ou deletar|

### 4.3  Licenciamento e Instalação
A licença escolhida para desenvolvimento será a MIT, onde possibilita a edição, visualização e utilização do software.

## 5.  Recursos do Produto
### 5.1 Acesso
Autenticação será feita por chave de acesso indicada no microprocessador

### 5.2 Gerenciamento de novas Receitas
Poderá adicionar novas receitas, indicando ingredientes que serão utilizados, tempos de aquecimento, tempo de fervura, de brasagem e suas temperaturas, trazendo assim as rampas de temperaturas para cada etapa e cada panela no processo.

### 5.3 Visualizar processo de produção/ Estimativa de tempo
 Cada etapa precisa ter ser executada em um determinado tempo, tendo que se aplicar temperatura ou deixar de repouso a mostura. Com isso a aplicação trará uma estimativa de tempo para finalização de cada etapa.

### 5.4 Gerenciar Processo de limpeza
Um dos critérios para que se atinja uma cerveja com uma boa qualidade é que os equipamentos estejam limpos antes do uso para que não ocorram interferências nos processos, principalmente no processo de repouso quando ocorre a fermentação. Com isso existirá um processo que poderá ser ativado remotamente pela aplicação onde efetuar a limpeza das panelas, mangueiras e bombas. Isto poderá ser iniciado ou parado pela aplicação.

### 5.5 Gerenciar processo de Produção de cerveja
 Será possível iniciar ou parar a produção. A parte de iniciação se torna óbvia por se tratar de um sistema automatizado de produção. Contudo a função de parar é necessária, pois erros podem ocorrer com o maquinário ou o usuário esquecer de adicionar algum dos ingrediente, com isso é necessário parar a produção. 	
 
 ### 5.6 Receber notificações
 Por não ser um processo 100% automatizado, o usuário irá precisar interagir com sistema algumas horas, tendo que adicionar ingredientes em tempos específicos e para não ficar na responsabilidade da memória de lembrar notificações serão geradas para usuário para esta finalidade. Ou até mesmo notificações de mudanças de etapas. Ou quando necessário notificações para que usuário retire algo( durante processo de limpeza).

 ## Restrições
 ### 6.1 Restrições de Sistema
A Aplicação se comunicará com a microcontroladores através de rede onde tanto o microcontrolador quanto ao aplicativo precisam estar conectados. Apenas usuários que tiverem chaves de acesso daquele microprocessador que conseguirá ter acesso de controle e de notificações.

### 6.2 Restrições extras 
As restrições extras que mais irão impactar será a integração entre os grupos de Software e Eletrônica para comunicação a API do microcontrolador com o Aplicação. A falta de conhecimento técnico da equipe na construção de um skill para Alexa.

## 7. Faixas de Qualidade
 Para melhor manuseio e eficiência a aplicação terá que ser responsiva de modo que possa ser utilizada em aparelhos mobile, pois um dos princípios do projeto é a portabilidade .
 
 ## 8. Precedência e Prioridade
 Em termos de importância ter acesso à API do microprocessador se torna um dos pontos chaves do projeto, após isso todas outras funcionalidade como: gerenciamento da produção, gerenciamento da limpeza, gerenciamento de receitas, visualizar processo da produção e receber notificações, são de grande importância, contudo todas dependem do acesso ao microprocessador.

## 9. Outros Requisitos do Produto
### 9.1 Requisitos de Sistema
O usuário precisará de algum dispositivos para que possa se acessar ao microprocessador

### 9.2 Requisitos de Desempenho
O dimensionamento do aplicativos se dará para suprir uma amplo gama de aparelhos para que se assim, os usuário.

