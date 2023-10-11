---
title: Pergunte a um especialista - Medindo a velocidade
description: Saiba como medir e rastrear a velocidade usando o [!DNL Workfront] relatórios. Esse workshop foi gravado em 14 de agosto de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
jira: KT-9912
last-substantial-update: 2023-08-15T00:00:00Z
exl-id: 83053de2-e386-4243-a9c8-a2ad9d51790f
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '3958'
ht-degree: 1%

---

# Pergunte a um especialista - Medindo a velocidade

Saiba como medir e rastrear a velocidade usando o [!DNL Workfront] relatórios. Esse workshop foi gravado em 14 de agosto de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341057/?quality=12)

## Campos personalizados usados na apresentação

Economize tempo copiando e colando os cálculos abaixo.

>[!NOTE]
>
>A sintaxe para cálculos de campo personalizado mudou desde que a apresentação foi feita em 2019, no entanto, os conceitos e outras instruções fornecidas na apresentação ainda são precisos.
>**Os cálculos incluídos abaixo foram atualizados para refletir as regras de sintaxe mais recentes.**

**Primeira data de compromisso**

Formato: Data

Cálculo:

```
IF(ISBLANK({DE:First Commit Date}),{defaultBaseline}.{plannedCompletionDate},{DE:First Commit Date})
```

**Primeira duração**

Formato: Texto

Cálculo:

```
IF(ISBLANK({DE:First Duration}),{defaultBaseline}.{durationMinutes},{DE:First Duration})
```

**Taxa Trabalho para Confirmação**

Formato:Número

Cálculo:

```
ROUND(DIV({actualDurationMinutes},{DE:First Duration}),1)
```

**Status da Proporção Trabalho para Confirmação**

Formato:Texto

Cálculo:

```
IF({DE:Work-to-Commit Ratio}>2,"Terrible",IF({DE:Work-to-Commit Ratio}>1.6,"Poor",IF({DE:Work-to-Commit Ratio}>1.2,"Not Bad","Excellent")))
```

**Velocidade ajustada**

Formato:Número

Cálculo:

```
ROUND(DIV({actualDurationMinutes},{durationMinutes}),1)
```

**Status da Velocidade Ajustada**

Formato:Texto

Cálculo:

```
IF({DE:Adjusted Velocity}>2,"Terrible",IF({DE:Adjusted Velocity}>1.6,"Poor",IF({DE:Adjusted Velocity}>1.2,"Not Bad","Excellent")))
```

## P&amp;R

**Pergunta**

Olá, obrigado por organizar este webinário. Tenho uma pergunta sobre o Field no Workfront. Em nosso sistema, criamos um campo personalizado chamado &quot;Estado&quot;, que é uma combinação de Status e Condição. Este campo Estado contém muitas estátuas em milhares de projetos, o que é muito importante para o nosso extrato de dados Tableau. No entanto, agora queremos eliminar esse campo e usar Condição, o campo nativo. Você tem alguma ideia de como posso virar esse campo sem perder dados? Tudo o que consigo pensar em fazer isso sem perder dados agora é trocar manualmente de projeto para projeto.

**Resposta**

Para uma situação como essa, você pode usar a filtragem e a edição em massa para semiautomatizar a tarefa de preencher o campo de Condição com base no campo personalizado Estado.

Estas são as etapas:

1. Determine quais valores de Estado deseja mapear para valores de Condição. Por exemplo, digamos que você tenha um valor de Estado de &quot;Atrasado&quot; e &quot;Muito Atrasado&quot; que são mapeados para um valor de Condição de &quot;Com Problemas&quot;
1. Criar um relatório de projeto mostrando todos os projetos com um valor de Estado de &quot;Atrasado&quot; e &quot;Muito Atrasado&quot;
1. Execute o relatório. Verifique se está mostrando todos os projetos (consulte as opções na parte inferior direita do relatório)
1. Clique na caixa de seleção na parte superior esquerda do relatório na barra com os cabeçalhos da coluna. Isso selecionará todos os projetos no relatório
1. Clique no botão Editar acima da lista de relatórios
1. Defina o tipo de condição como Manual
1. Defina o campo Condição como Com problema
1. Clique em Salvar alterações


**Pergunta**

Como é excelente, não ruim etc. definidos?

**Resposta**

Este foi apenas um exemplo, mas aqui está como eu configurei. Primeiro, calculei dois índices:

Velocidade ajustada

A fórmula para isso é Duração real/Duração planejada (que é armazenada no campo Duração em um projeto). Como a duração planejada do projeto pode mudar sempre que o projeto é replanejado, a duração planejada representa o replanejamento final.

Taxa Trabalho para Confirmação

Essa fórmula é como a Velocidade ajustada, exceto que, em vez de usar o valor da Duração planejada do replanejamento final, queremos usar a Duração planejada prometida inicialmente ao cliente. Estamos presumindo que a linha de base Original contém essas informações (e estamos planejando a partir de agora solicitar que nossos gerentes de projeto planejem seus projetos dessa forma para que possamos capturar dados precisos). Capturamos esse valor de duração da linha de base original e o chamamos de Primeira duração.

Dividindo a Duração Real pela Duração Planejada ou pela Primeira Duração, obtemos um número que pode nos informar a proximidade com que chegamos ao destino. Se a Duração planejada ou a Primeira Duração for igual à Duração real, o índice será igual a 1. Se a Duração real for maior, a resposta será maior que 1. Quanto maior o número pior nós fizemos na reunião de nossa data.

Assim, considerando tudo o que decidi atribuir status para a Velocidade ajustada e a Relação trabalho-para-compromisso, da seguinte maneira:

* 1,1 ou abaixo, eu chamei de Excelente.
* De 1.2 a 1.5 eu chamei Not Bad.
* 1.6 a 1.9 Eu chamei de Pobre.
* 2 ou mais eu chamei de Terrível.

**Pergunta**

O que o trabalhador precisa fazer para rastrear o tempo necessário para realizar os projetos?

**Resposta**

Não estamos rastreando as horas reais gastas trabalhando nos projetos aqui, estamos apenas rastreando e comparando a duração. Mas, se você estiver rastreando horas e quiser usar horas reais sobre horas planejadas para calcular a velocidade, é possível fazer esse mesmo tipo de relatório comparando as horas planejadas com as horas reais. Você também capturaria as horas planejadas a partir da linha de base original.

**Pergunta**

É possível fornecer filtros usados para o Velocity?

**Resposta**

Usei duas regras de filtro para os relatórios do Velocity:

* Categorias >> ID >> Igual >> Dados do projeto WPI (este é o formulário personalizado que continha todos os campos calculados. Desejo ver apenas os projetos que estão usando este formulário personalizado)
* Projeto >> Status >> Igual >> Concluído (quero ver apenas os projetos concluídos porque eles têm um valor de Duração real que representa quanto tempo levou para concluir tudo. Os projetos atuais não forneceriam uma Duração real precisa para calcular a velocidade)

Também adicionei outro filtro para manter meu relatório pequeno o suficiente para gerenciar o webinário, mas em seu ambiente de produção, você provavelmente desejaria ver todos os projetos com o formulário personalizado WPI em um período específico. Talvez você queira filtrar a Data de conclusão atual do projeto para isso.

**Pergunta**

Se você copiar um projeto, ele terá as mesmas linhas de base para o novo projeto?

**Resposta**

Não, as linhas de base não estão incluídas no projeto copiado

**Pergunta**

Para um processo de aprovação de tarefa, você pode me mostrar como criar um relatório que forneça uma trilha de auditoria por tarefa em um projeto com um carimbo de data/hora para cada aprovador?

**Resposta**

Criar um relatório de Tarefa. Na guia Colunas (Exibir) clique em Adicionar coluna. Na caixa &quot;Mostrar nesta coluna:&quot;, digite &quot;approv&quot;. Isso mostrará os vários campos de aprovação disponíveis para relatório. Sugiro que você adicione uma coluna para tudo no início (exceto qualquer ID), para que possa ver quais informações são exibidas.

Em seguida, acesse a guia Filtros e adicione uma regra de filtro para:

Tarefa >> É Aprovação >> Igual >> Verdadeiro. Isso só mostrará tarefas que tenham uma aprovação anexada.

Adicione filtros adicionais, conforme necessário.

**Pergunta**

Gostaria de criar um relatório de prova. Uma lista de projetos que mostra quantas provas eles têm e quantas versões dessa prova existem.

**Resposta**

Criar um relatório de documento.

A visualização padrão mostrará o número da versão. Você vai querer deixar isso aí, mas pode alterar qualquer outra coluna.

Agrupar o relatório por Nome do projeto.

Filtrar o relatório pela versão atual: a ID da prova não está em branco.

Isso fornecerá uma lista de todas as provas em cada projeto. Ele terá uma linha para cada prova e exibirá o número da versão (que será o mesmo que o número total de versões).

**Pergunta**

É possível usar a velocidade no nível da tarefa? Em vez do nível do projeto?

**Resposta**

Sim, mas será necessário copiar o formulário personalizado do projeto e criar um formulário personalizado de tarefa a partir dele. Em seguida, será necessário editar o cálculo no campo Primeira data de confirmação e alterar a referência para &quot;Linha de base padrão&quot; para &quot;Tarefa de linha de base padrão&quot;. Faça o mesmo para a Primeira Duração. Depois disso, você poderá anexar o formulário personalizado de tarefa a qualquer tarefa que desejar medir. Será necessário criar relatórios de tarefa em vez de relatórios de projeto para eles. No entanto, você ainda precisará verificar se a linha de base do projeto original está definida como a linha de base padrão. Todos os dados da tarefa são mantidos na mesma linha de base que os dados do projeto.

**Pergunta**

A primeira data de confirmação precisa ser definida manualmente pelo proprietário do projeto? Ou ele poderia extrair de campos existentes?

**Resposta**

A Primeira Data de Commit é capturada na linha de base padrão. Desde que a linha de base padrão seja a original, isso mostrará a data de conclusão planejada do projeto no momento em que foi definido pela primeira vez como status Atual.

**Pergunta**

Os campos calculados em formulários personalizados ainda precisam ser atualizados periodicamente corretamente? Ou isso acontecerá automaticamente durante a noite (ou em algum outro acionador) agora?

**Resposta**

Os campos calculados são recalculados:

* Quando um usuário edita o objeto
* Na edição de itens em massa com as expressões personalizadas Recalcular ativadas
* Modificações no formulário com a opção &quot;Atualizar cálculos anteriores&quot; selecionada

**Pergunta**

Se a velocidade estiver considerando a Duração, a Porcentagem concluída na Preferência do projeto deve se basear na Duração?

**Resposta**

Não, a opção Preferências do Projeto se refere apenas à forma como o Percentual Concluído é calculado. O valor duration em si não é afetado por essa configuração.

**Pergunta**

Qual é a diferença entre a duração do primeiro e do plano?

**Resposta**

Primeira duração é o número de dias que você prometeu originalmente ao cliente que o projeto levaria. Obtemos esse número da linha de base original que foi registrada quando o projeto foi alterado de Planejamento para Atual.

Duração planejada é o número de dias desde o início do projeto até a Data de conclusão planejada. Inicialmente, essas duas durações são as mesmas, mas se o projeto já foi replanejado e a Data de conclusão planejada mudou, a Duração planejada também mudou.

O valor dos relatórios do Velocity vem da possibilidade de ver o quanto a Duração planejada mudou desde a Primeira Duração. Podemos ver isso desde quando começamos a registrar linhas de base como projetos alterados de Planejamento para Atual.

**Pergunta**

É possível definir os trabalhadores por cor para que sejam iguais em todos os relatórios?

**Resposta**

Se você agrupar por Atribuído a >> Nome em um relatório de tarefa, poderá atribuir uma cor a trabalhadores específicos na guia Gráfico. Basta escolher a opção Cores Personalizadas ao lado da caixa Atribuído a >> Nome na guia Gráfico e adicionar uma cor para cada trabalhador.

**Pergunta**

Estou tentando determinar se é possível criar um painel com uma área que procura um formulário personalizado em nível de tarefa para ver se ele está presente e secundário se determinados campos não estiverem em branco. Isso é possível?

**Resposta**

Vamos ver se eu entendo a sua pergunta. Suponha que eu tenha um formulário personalizado de tarefa chamado Formulário Tammy com um campo chamado Campo Tammy.

Você está querendo um relatório de tarefas que irá mostrar todas as tarefas que têm Tammy Form anexado e onde Tammy Field tem algum valor nele.

Sim, você pode fazer isso. Você só precisaria de um filtro no seu relatório de tarefas com duas regras de filtro:

Categorias >> ID Forma Tammy Igual

Task > Tammy Field Is Not Blank

**Pergunta**

Existe uma maneira de criar um relatório para procurar um documento nomeado específico na Biblioteca de documentos? Parte do painel que queremos medir se determinados documentos existirem.

**Resposta**

Sim. É necessário criar um relatório de documento. Parece que você deseja fornecer um nome de documento específico sempre que executar o relatório. Se esse for o caso, eu recomendaria ir até Opções de relatório e selecionar Prompts de relatório. Adicione um prompt para Documento >> Nome.

**Pergunta**

Você pode escolher uma cor/valor hexadecimal não listado na guia do gráfico, mas essa é uma nova cor, que é um novo valor hexadecimal. Por exemplo, uma nova cor das cores da minha marca para permitir que eu personalize os relatórios?

**Resposta**

Sim, você pode digitar qualquer código de RGB que tenha sido capaz de encontrar. É um código padrão que informa a quantidade de vermelho, verde e azul contida na cor. A Workfront aceitará qualquer valor hexadecimal de 000000 a FFFFFF, portanto, se você souber o código da cor da sua marca, poderá usá-lo.

**Pergunta**

Você pode reafirmar a definição dos relatórios no painel (fornecer uma declaração do que cada relatório mede)?

**Resposta**

Gráfico de status da velocidade ajustada

> Isso mostra o quão bem fizemos ao concluir projetos no prazo ao comparar a Duração real do projeto com a Duração planejada. A duração planejada foi ajustada à medida que o projeto era replanejado durante seu ciclo de vida.

Gráfico de Status da Proporção Trabalho-para-Compromisso

> Isso mostra o quão bem fizemos ao concluir projetos no prazo ao comparar a Duração real do projeto com a Primeira Duração. Sendo a primeira duração a hora original, prometemos ao cliente que o projeto levaria para ser concluído. A Primeira Duração foi calculada a partir do valor da Duração do projeto quando ele foi alterado pela primeira vez do status Planejamento para Atual. Essa foi a Duração registrada na linha de base Original.

Relatório da lista de status do Velocity

> Este relatório contém todos os campos personalizados calculados e as datas significativas para os mesmos projetos nos gráficos. Seu objetivo é permitir que verifiquemos nossos cálculos e obtenhamos informações mais detalhadas, se desejado.

**Pergunta**

Como você adicionou os novos dados ao eixo x?

**Resposta**

Quando você agrupa por qualquer item em um relatório, é possível criar um gráfico. Em seguida, defina o eixo X ou Y na guia Chart.

**Pergunta**

Você pode ultrapassar a diferença entre a primeira duração e a duração real?

**Resposta**

Primeira duração é o número de dias que você prometeu originalmente ao cliente que o projeto levaria. Obtemos esse número da linha de base original que foi registrada quando o projeto foi alterado de Planejamento para Atual.

Duração Efetiva é o número de dias desde o início do projeto até a Data de Término Efetivo.

**Pergunta**

Como a linha de base do projeto influencia nesse relatório?

**Resposta**

A linha de base Original do projeto contém a Data de conclusão planejada e a Duração planejada que existia quando o projeto foi alterado pela primeira vez para o status Atual. Se o processo era para planejar o projeto antes de defini-lo como Atual, isso representaria a data em que você confirmou a conclusão do projeto.

**Pergunta**

Existe uma maneira de aplicar em massa o novo formulário a projetos antigos?

**Resposta**

Sim, você pode selecionar vários projetos em uma lista. Quando você faz isso, uma opção &quot;Editar&quot; aparece no canto superior esquerdo da lista. Clicar em Editar quando vários objetos forem selecionados colocará você no que chamamos de &quot;edição em massa&quot;. Você pode adicionar um formulário personalizado a vários projetos dessa maneira.

Um atalho para adicionar formulários personalizados a um grande número de projetos é criar um relatório que você filtra para incluir apenas os projetos que deseja. Em seguida, em vez de selecionar projetos individualmente, basta clicar na caixa de seleção acima da primeira caixa de seleção na lista e selecionar toda a lista.

**Pergunta**

É possível remover entradas duplicadas de dentro do agrupamento em um relatório de atribuição, mas não entre agrupamentos?

**Resposta**

A melhor maneira de pensar sobre agrupamentos em relatórios de listas é:

Primeiro, você controla quais itens são exibidos na lista usando a guia Filtro. Não haverá entradas duplicadas. O filtro é aplicado a cada objeto. Se ele passar pelo filtro, aparecerá uma vez na lista; caso contrário, não aparecerá.

O próximo agrupamento é aplicado à lista filtrada. Um agrupamento identifica uma coisa sobre os objetos na lista, como o nome do portfólio em que ele está (não é possível agrupar em uma lista de itens, somente em uma única coisa). Assim, todos os objetos com o mesmo valor aparecerão nesse agrupamento, como todos os projetos no mesmo portfólio. Qualquer projeto que não tenha um portfólio selecionado aparecerá no agrupamento chamado &quot;Sem valor&quot;.

Como resultado, não há como qualquer objeto aparecer em mais de um agrupamento. E se um objeto aparece na lista é totalmente controlado pelo filtro (e se a pessoa que está executando o relatório tiver direitos para visualizá-lo).

**Pergunta**

Você recomendaria algum outro relatório para rastrear a Velocity? Apenas uma recomendação de alto nível é ótima porque eu sei que não há tempo suficiente para entrar em detalhes.

**Resposta**

Assim como em qualquer relatório, a primeira coisa que você precisa fazer é decidir o que deseja saber. A próxima etapa é acessar essas informações, o que em alguns casos significa que você precisa começar a rastreá-las.

Uma razão pela qual decidi comparar a Duração real com dois tipos de Duração planejada foi porque pensei que ela fornecesse insights interessantes sobre a velocidade. Os dados também já estavam disponíveis, então não tive que começar a rastreá-los. Com alguns cálculos eu poderia extrair os dados em um formulário que eu poderia relatar sobre ele.

Mas você também pode decidir rastrear outras informações sobre tarefas ou projetos para relatar.

O Workfront não tem nenhum relatório velocity integrado, portanto, eu recomendaria que você e sua equipe fizessem um brainstorm sobre o que você deseja saber para determinar a velocidade e, em seguida, ver o que você precisa rastrear.

**Pergunta**

Você consegue calcular algo no nível da COLUNA? Em vez de chamar um CAMPO calculado de um formulário personalizado?

**Resposta**

Teria sido possível usar uma expressão de valor no modo de texto para fazer esses cálculos. Não poderíamos ter feito a Primeira Duração ou a Primeira Data de Confirmação, mas precisávamos capturá-los em um local onde não seriam alterados.

Quanto ao Status da taxa de trabalho para confirmação e Status da velocidade ajustada, eles precisavam ser campos personalizados para que pudéssemos usá-los na guia Gráfico. A guia Chart não reconhece agrupamentos em modo texto, eles precisam ser campos personalizados. E como precisávamos que a Taxa de trabalho para compromisso e a Velocidade ajustada calculassem esses status, também precisávamos que eles fossem campos personalizados. Nesse caso, todos eles precisavam ser campos personalizados, mas é sempre bom considerar de ambas as maneiras e escolher o que funcionará melhor. Obrigado pela pergunta.

**Pergunta**

Nossos projetos mudam com frequência devido a atrasos ou alterações por parte dos clientes. Nosso relatório pode mostrar tudo como &quot;terrível&quot;. O que é uma recomendação para rastrear motivos de alteração? Pensamos em adicionar um formulário personalizado no nível do documento que relate o motivo da alteração (seja interna ou no cliente), mas imaginando o que é uma prática recomendada.

**Resposta**

A prática recomendada é usar uma lista suspensa para rastrear isso. Coloque quantos &quot;motivos&quot; você puder pensar nele para começar, em seguida, adicione uma opção &quot;outro&quot; para capturar um motivo que não está na lista. Se o novo motivo parecer ou se tornar comum, adicione-o à lista suspensa. Você pode facilmente criar relatórios em uma lista suspensa e agrupar nesse campo (não é possível agrupar em caixas de seleção ou em uma lista suspensa de várias seleções).

Só mais um comentário sobre isso. Talvez você não queira incluir todos os projetos nos relatórios do Velocity. Se você está consertando erros ou &quot;indo onde ninguém foi antes&quot; você provavelmente não está fazendo o mesmo tipo de compromisso com uma data de conclusão como se você estivesse construindo uma casa que você construiu muitas vezes antes.

Portanto, concentre seus relatórios de velocidade em lugares onde eles podem ajudá-lo a atingir suas metas.

**Pergunta**

Se eu definir a linha de base padrão em um projeto como &quot;Original&quot; e, em seguida, tirar o projeto do atual e colocá-lo novamente na atual, ele alterará minha linha de base padrão?

**Resposta**

Sim. Sempre que você alterar o status para Atual, receberá uma nova linha de base que será o novo padrão. Mas todas as linhas de base anteriores ainda existirão e você pode definir manualmente a linha de base original para ser a linha de base padrão novamente.

**Pergunta**

Há uma maneira de configurar em um relatório quais campos são editáveis? Posso definir restrições para determinados campos?

**Resposta**

Você pode restringir os direitos de exibição e edição para campos em um formulário personalizado. Será necessário incluir os campos em uma seção e, nas configurações da seção, você pode escolher os direitos necessários para que os usuários possam exibir ou editar campos na seção.

**Pergunta**

É possível criar um relatório que procure um documento nomeado específico na biblioteca de documentos?

**Resposta**

Sim. É necessário criar um relatório de documento. Parece que você deseja fornecer um nome de documento específico sempre que executar o relatório. Se esse for o caso, eu recomendaria ir até Opções de relatório e selecionar Prompts de relatório. Adicione um prompt para Documento >> Nome.

**Pergunta**

Nos relatórios, por que os valores estão disponíveis como coluna, mas não estão disponíveis para seleção ou agrupamento. Por exemplo: Origem da ocorrência.

**Resposta**

O motivo principal pelo qual uma coluna pode ser visualizada, mas não está disponível para agrupamento, é que ela pode conter uma lista, como caixas de seleção, campos personalizados ou atribuições de tarefas. O agrupamento em uma lista não é permitido.

**Pergunta**

Como posso me separar em um relatório (por quais campos) quando a entrada de hrs aconteceu e quando as hrs foram realmente executadas?

**Resposta**

O campo Data de entrada do objeto Hora refere-se à data em que as horas foram trabalhadas. Isso faz com que a Data de entrada seja diferente de outros objetos, onde significa a data em que o objeto foi criado. Mesmo que não haja uma data de criação para horas, há uma &quot;Data da última atualização&quot;, que é inicialmente a data de criação e, em seguida, qualquer data em que a hora foi editada posteriormente.

**Pergunta**

Do ponto de vista dos relatórios, como podemos acessar os dados da linha de base? Tenho um projeto com várias linhas de base. Quero ver como as tarefas individuais foram planejadas em cada linha de base. Existe uma maneira de escrever um relatório que mostrará o plano do projeto para cada linha de base?

**Resposta**

Um relatório mostrará os campos que você deseja ver para a linha de base atualmente definida como padrão, para que você possa alterar a linha de base e atualizar seu relatório para ver os campos com a nova linha de base.

Mas se você quiser ver as informações sobre suas tarefas graficamente, é possível fazer isso usando o recurso Gráfico de Gantt. Ative o Gantt em uma lista de tarefas (usando o ícone de Gantt no canto superior direito ao lado de Salvamento automático), vá para o ícone Configurações logo abaixo e à direita e clique nele. Marque a caixa Linha de Base para mostrar todas as linhas de base. Você pode selecionar uma de cada vez e ver as alterações em suas tarefas no modo de exibição de Gantt.

**Pergunta**

Como criar um relatório para encontrar as alterações em seu status para um período definido, por exemplo, mês passado.

**Resposta**

O recurso Analytics no Workfront fornece uma maneira inteligente de exibir dados históricos, incluindo alterações de status.

Mas você também pode obter informações de alteração de status usando um relatório de Nota. Você pode filtrar para ver as alterações de status nos projetos se estiver rastreando o campo Status do projeto.

Primeiro, vá para Setup>Interface>Update Feeds e verifique se o Status do projeto é um dos campos incorporados que estão sendo rastreados. Se não for, é necessário adicioná-lo.

Agora crie um relatório de Nota e faça o seguinte:

Na guia Colunas (Exibir):

* Substitua a coluna &quot;Texto da observação&quot; por &quot;Texto de auditoria&quot;. Isso exibirá informações sobre o que o status mudou de e para
* Deixe as colunas &quot;Project: Name&quot; e &quot;Entry Date&quot;
* Clique na coluna &quot;Data de entrada&quot; e marque &quot;Classificar por esta coluna&quot; no painel Configurações de coluna. Se você quiser ver as alterações de status mais recentes no topo, classifique-as em ordem decrescente.

Na guia Groupings:

* Agrupar por Projeto: Nome

Na guia Filtros, crie as seguintes regras de filtro:

* Nota >> Tipo de Auditoria >> Igual >> Alteração de Status
* adicione regras adicionais para filtrar pela Data de Entrada do Aviso. Você pode preferir deixar isso de fora dos Filtros e usar um prompt de relatório
* Filtre por projeto, portfólio ou outros dados, conforme desejado.

**Pergunta**

Como planejador, você pode obter relatórios para outros usuários?

**Resposta**

Um Planejador pode criar relatórios e compartilhá-los com qualquer usuário, mesmo com pessoas que não sejam usuários. Ao exibir o relatório, vá para Ações de relatório>Compartilhamento e clique no ícone de engrenagem no canto superior direito da caixa Acesso ao relatório. Escolha a opção &quot;Tornar público para usuários externos&quot;. opção. Você pode copiar o link fornecido e enviá-lo a qualquer pessoa. Ele verá o relatório em tempo real em seu navegador.
