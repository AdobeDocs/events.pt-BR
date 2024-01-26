---
title: Pergunte ao especialista - Relatórios do modo de texto básico de sobrecarga usando o API Explorer
description: Saiba mais sobre o explorador de API, como usá-lo e como aprimorar seus relatórios usando o modo de texto básico. Esse webinário foi gravado em 22 de janeiro de 2020.
doc-type: feature video
team: Technical Marketing
kt: 9918
exl-id: f859c4eb-8b3c-4d91-9765-9957dc4678f5
duration: 4068
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '1658'
ht-degree: 1%

---

# Pergunte ao especialista - Relatórios do modo de texto básico de sobrecarga usando o API Explorer

Saiba mais sobre o [[!UICONTROL API Explorer]](https://developer.adobe.com/workfront/api-explorer/), como usá-lo e como aprimorar seus relatórios aproveitando o modo de texto básico. Esse webinário foi gravado em 22 de janeiro de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341124/?quality=12)

## Recursos adicionais

![Um gráfico que mostra exemplos de regras de código do modo de texto](assets/text-mode-chart.png)


**Coluna final &quot;Todas as funções de trabalho&quot;**

```
description="Primary =" indicates the user's primary job role
displayname=All Job Roles
listdelimiter=<p>
listmethod=nested(userRoles).lists
textmode=true
type=iterate
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("Primary = ",{role}.{name}),{role}.{name})
valueformat=HTML
```

**Modo de texto para a coluna &quot;Todas as equipes&quot;**

```
displayname=All Teams
listdelimiter=<p>
listmethod=nested(teams).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

**Modo de texto para a coluna &quot;Todos os grupos&quot;**

```
displayname=All Groups
listdelimiter=<p>
listmethod=nested(userGroups).lists
textmode=true
type=iterate
valuefield=group:name
valueformat=HTML
```

**Modo de texto para a coluna &quot;Subordinados diretos&quot;**

```
displayname=Direct Reports
listdelimiter=<p>
listmethod=nested(directReports).lists
textmode=true
type=iterate
valueexpression={name}
valueformat=HTML
```

## P&amp;R

**Pergunta**

É possível usar qualquer coleção em um relatório, usando o modo de texto?

**Resposta**

Sim, você pode usar qualquer objeto na área de coleções. Você desejará explorar e ver a que tem acesso. Nem tudo terá acesso ao objeto do usuário e ao objeto da função de trabalho, como vimos com o objeto Funções do usuário no explorador de API.

**Pergunta**

Você pode discutir o &quot;uso condicional de diferentes coleções na mesma coluna (atualizações de projeto versus atualizações de tarefa)&quot;

**Resposta**

Quando você está na área de iteração e vê o campo value ou a expressão valuefield lá, você acessa um dos itens em sua lista de coleções. Usando o campo de valor, podemos obter o nome dessa função de trabalho, por exemplo, ou qualquer item que esteja nesse item na lista. Se você estiver em uma tarefa, um objeto de tarefa poderá fazer referência ao projeto em que ele está.

**Pergunta**

Você pode discutir se a &quot;coleção de atualizações de tarefa só é possível em um relatório de tarefa&quot;?

**Resposta**

Ao criar um relatório de problemas, você pode ver as informações da tarefa se o problema foi relatado na tarefa e também pode ver essas informações de dentro da coleção. Exceto para essas situações, você precisaria estar em um relatório de tarefa para ver os dados de coleta da tarefa.

**Pergunta**

É possível compartilhar o formato de texto ([!DNL CSS]) exemplos?

**Resposta**

O Workfront não é compatível [!DNL CSS] no modo texto.

**Pergunta**

Qual é a melhor maneira e/ou mais rápida de localizar um nome de campo personalizado para relatórios no modo de texto? Eu usei a opção de edição de HTML no navegador OU adicionando um campo em um relatório e alternando para o modo de texto para capturá-lo, MAS... curioso como os outros executam isso

**Resposta**

É mais rápido selecionar o campo na interface do usuário, alternar para o Modo de texto e copiar o nome do campo. Isso garante que eu obtenha a ortografia correta para o campo.

**Pergunta**

Como posso usar o modo de texto para identificar membros de uma equipe em um relatório? Atualmente, usamos atribuições de equipes nos fluxos de trabalho de aprovação de tarefas e gostaríamos de listar os membros da equipe no estágio de aprovação atual em uma coluna semelhante a como o campo Aprovadores e Status funciona.

**Resposta**

Para fazer referência aos Membros da equipe associados ao estágio de aprovação atual, seria necessário fazer referência a uma coleção referenciada, o que não é possível no momento por meio dos recursos do modo de texto do Workfront. A coluna que sua organização está usando atualmente que mostra a Equipe associada à aprovação é sua melhor opção.

**Pergunta**

O campo e o nome do objeto precisam estar em Letras Maiúsculas e Minúsculas (por exemplo, Função vs Função)?

**Resposta**

Ao fazer referência a objetos no modo de texto, você desejará gravá-lo exatamente como a coluna à direita do API Explorer mostra. Por exemplo, se você deseja referenciar um nome de projeto de um relatório de Tarefa, seu campo de valor seria semelhante ao seguinte:

```
valuefield=project:name
```

No entanto, no caso de problemas, elas são chamadas de opTasks no API Explorer. Portanto, se você executar um relatório de Horas e quiser adicionar uma coluna para Nome do problema, o campo de valor seria semelhante ao seguinte:

```
valuefield=opTask:name
```

**Pergunta**

Estou procurando criar um relatório que mostra, para cada projeto, as tarefas ativas atuais que estão sendo trabalhadas. Como eu faria isso da melhor maneira? Imagino que seja um relatório de tarefas que também tenha colunas de informações do projeto adicionadas?

**Resposta**

É verdade. Um relatório de tarefa seria melhor para isso. Você precisaria definir &quot;Tarefas ativas&quot;. Se você estiver usando predecessores, essas serão as tarefas que estão Prontas. Portanto, você pode filtrar por Pronto = Verdadeiro. Isso traria todas as tarefas que estão prontas para começar. Em seguida, recomendo que você agrupe por Nome do projeto, dessa forma, suas tarefas são todas agrupadas e é possível ver rapidamente quais tarefas pertencem a qual projeto.

**Pergunta**

Há uma maneira de criar relatórios que calculam dados, por exemplo, % de projetos que atendem a determinados critérios?

**Resposta**

A melhor maneira de criar um relatório para apresentar ou calcular dados (%, por exemplo) seria aplicar agrupamentos ao relatório e, em seguida, aplicar um gráfico. Se você adicionasse um gráfico de pizza ao relatório, teria a opção de as fatias de pizza estarem em valores ou porcentagens.

**Pergunta**

Você pode usar o modo texto para identificar os membros de uma equipe que estão atribuídos ao estágio de aprovação de tarefa atual semelhante à coluna Aprovadores e Status?

**Resposta**

Seria necessário adicionar uma coluna da coleção no modo texto ao relatório Tarefa com o seguinte:

```
displayname=Current Approval Stage Approvers 
listdelimiter=<p> 
listmethod=nested(currentApprovalStep.stepApprovers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

**Pergunta**

É possível filtrar onde Todos os grupos contêm um grupo específico?

**Resposta**

Se você quiser filtrar os itens no seu relatório, faça isso na guia Filter do seu relatório. Portanto, se você quiser ver apenas os usuários em que um de seus grupos era de Contabilidade, você adicionaria uma regra de filtro que dizia:

```
Other Groups>ID>Equal>Accounting
```

**Pergunta**

Existe uma maneira de criar um relatório que determina a duração real de uma combinação de tarefas?

**Resposta**

Você precisaria filtrar seu relatório para incluir apenas a combinação de tarefas desejada. Em seguida, você precisaria colocar uma coluna de Duração real na visualização e resumi-la por Soma nas Configurações de coluna e, por último, seria necessário agrupar o relatório de alguma forma. Quando você executar o relatório, a barra de agrupamento mostrará o total das durações reais contidas nas linhas que estão sendo agrupadas.

**Pergunta**

Existe uma maneira de subtrair tarefas que se enquadram em um pai para determinar a duração do restante das tarefas em um pai?

**Resposta**

A duração de uma tarefa pai é calculada subtraindo-se a data de início da tarefa de início mais antiga da data de término da tarefa mais recente sob essa tarefa pai. Em um relatório, você só sabe sobre cada tarefa individual que é considerada a exibição ou não. O mecanismo de relatório não tem como se segurar nas informações de uma tarefa e usá-las ao observar outra tarefa. Assim, a única maneira de realizar o que você está solicitando é remover uma tarefa de estar sob um determinado pai enquanto estiver na lista de tarefas do projeto e observar como a duração da tarefa pai é recalculada.

**Pergunta**

Para agrupamentos condicionais, um formulário personalizado (pense em &quot;Estados Ocidentais&quot;, &quot;Estados Centrais&quot;, &quot;Estados Orientais&quot;) para decodificar os grupos individuais é uma técnica comum que funciona bem nessa nota, quando você recomenda usar agrupamentos calculados em vez de parâmetros calculados?

**Resposta**

Agrupamentos calculados (também conhecido como expressão de valor em um agrupamento) é uma maneira conveniente de obter um resultado para mostrar em sua barra de agrupamento. Isso também pode ser feito usando um campo personalizado calculado. Há vantagens e desvantagens para cada abordagem:

* As expressões de valor são calculadas sempre que a página do navegador é atualizada. Pode ser melhor do que campos personalizados calculados que são recalculados sempre que o objeto ao qual estão anexados é editado, ou quando os campos calculados são recalculados em uma edição em massa, ou quando o formulário personalizado é editado e a opção &quot;Atualizar cálculos anteriores&quot; é selecionada.
* No entanto, expressões de valor não podem ser usadas em gráficos, formatação condicional ou filtro. Será necessário usar campos personalizados calculados para eles.

**Pergunta**

Não há como alterar o nome de exibição do agrupamento de &quot;Sem valor&quot; para algo que escolhemos chamar para fins de relatório? em outras palavras, sempre será &quot;Sem valor&quot;?

**Resposta**

Há uma maneira de substituir &quot;Sem valor&quot; por algo diferente. Suponha que você tenha um relatório de projeto agrupado por Nome do Portfolio. Todos os projetos não atribuídos a um portfólio terminarão em um agrupamento com o título:

```
Portfolio: Name: No Value
```

Para alterar isso, edite o agrupamento no modo de texto e substitua esta linha:

```
group.0.valuefield=portfolio:name
```

com esta linha:

```
group.0.valueexpression=IF(ISBLANK({portfolio}.{name}),"Not in any Portfolio",{portfolio}.{name})
```

O agrupamento terá este título:

```
Portfolio: Name: Not in any Portfolio
```

**Pergunta**

Há um parâmetro para rastrear atribuições incompletas, ou seja:

1. Tarefas com uma única atribuição que não teve um indivíduo atribuído a ela ou
1. Tarefas com várias atribuições que têm pelo menos um indivíduo não atribuído para as funções solicitadas

**Resposta**

Isso pode ser feito usando um Relatório de atribuição e filtragem para

```
Assigned To ID > Is Blank and Role ID > Is Not Blank
```

Isso extrairá todas as tarefas ou problemas que foram atribuídos a uma função, mas não necessariamente a um usuário específico. Será necessário adicionar as colunas para o nome da Tarefa e do Problema para ver a qual objeto a atribuição pertence e, se agrupada por nome do Projeto, isso deve ajudar a mantê-la organizada.

**Pergunta**

Chuck, estou esquecendo, mas você se lembra da propriedade no modo texto que será renderizada como uma dica de ferramenta ao passar o mouse?

**Resposta**

description= permite exibir uma dica de ferramenta ao passar o mouse sobre o cabeçalho da coluna.

**Pergunta**

Posso relatar um campo com caixa de seleção que permite várias seleções, mas que só permite inserir a primeira seleção no relatório?

**Resposta**

Sim. As opções selecionadas no campo de caixa de seleção estão todas em uma cadeia de caracteres com cada seleção separada por vírgula. Você usará a expressão SEARCH para localizar a posição da primeira vírgula no Campo de caixa de seleção e, em seguida, usará esse índice com a expressão LEFT para exibir esses muitos caracteres do início da lista. Este é o código:

```
valueexpression=IF(SEARCH(",",{DE:Checkbox Field},0)>0,LEFT({DE:Checkbox Field},SEARCH(",",{DE:Checkbox Field},0)),{DE:Checkbox Field})
```

Se você usar uma vírgula em um nome de seleção no campo da caixa de seleção, ela só exibirá a parte dessa seleção até a primeira vírgula.
