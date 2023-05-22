---
title: Pergunte ao especialista - Avaliação da qualidade e engajamento
description: Saiba como criar relatórios que respondem a perguntas sobre qualidade e engajamento. Este webinário foi gravado em 13 de novembro de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9914
source-git-commit: edd0bdb28a9b3d065a64a95af6a216b747577c77
workflow-type: tm+mt
source-wordcount: '1211'
ht-degree: 1%

---

# Pergunte ao especialista - Avaliação da qualidade e engajamento

Saiba como criar relatórios que respondem a perguntas sobre qualidade e engajamento. Este webinário foi gravado em 13 de novembro de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341120/?quality=12)

## P&amp;R

**Pergunta**

Alguns campos estão disponíveis para filtrar, mas não estão disponíveis ao tentar agrupar por eles. Você está trabalhando para torná-las opções consistentes?

**Resposta**

As ferramentas de relatório não permitirão agrupar por um campo dinâmico ou por um que possa ter várias opções selecionadas de uma vez, como um campo de caixa de seleção. Você só pode agrupar em campos que tenham um único valor, mesmo que tenham muitas opções.

Você pode filtrar por caixas de seleção e visualizá-las, mas não pode agrupá-las.

**Pergunta**

No exemplo de iteração em funções de trabalho, posso mostrar a principal em negrito?

**Resposta**

Na iteração, é possível identificar a função principal. Precisamos fazer isso em uma expressão de valor, mas os códigos de HTML não são reconhecidos em uma expressão de valor. Então precisamos encontrar outra maneira de identificar o papel como sendo o principal. Coloquei &quot;**&quot; antes e depois do nome da função principal neste código. Experimente e veja como você gosta:

```
displayname=All Job Roles 
listdelimiter=<p> 
listmethod=nested(userRoles).lists 
textmode=true
type=iterate 
valueexpression=IF({user}.{roleID}={role}.{ID},CONCAT("**",{role}.{name},"**"),{role}. {name})
valueformat=HTML
```

Isso lhe dará uma lista como esta:

```
Support Engineer 
QA Engineer 
**Designer**
```

Onde Designer é a função principal desse usuário.

**Pergunta**

Oi! Estou organizando um fluxo de trabalho para nossa equipe Editorial que acompanha onde um artigo está em seu ciclo de vida (escrita inicial —> revisões de departamentos —> edições finais —> publicação). Eles desejam ver facilmente em qual etapa ou tarefa ele está no momento. O feedback que estou recebendo é que a visualização padrão de Marco (com o sombreamento vermelho ou verde) é muito &quot;ocupada e complexa&quot;. Há alguma maneira de mostrar apenas o &quot;Nome do projeto&quot; e o &quot;Marco atual&quot; em uma tabela ou grade?

**Resposta**

Sim. Você pode criar um relatório de tarefa que mostrará as tarefas de etapa que estão sendo trabalhadas no momento e a qual tarefa ele está associado. Você pode fazer isso em uma tabela ou em um relatório de lista.

**Pergunta**

É possível combinar informações de prova com informações do projeto em um relatório?

**Resposta**

Se você tiver criado um relatório Aprovação de prova, as informações do projeto podem ser colocadas em colunas usando o modo de texto. Por exemplo, se você deseja fazer referência ao nome do projeto em uma coluna, você pode usar o seguinte:

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name 
valueformat=HTML
```

**Pergunta**

Também gostaria de obter mais informações sobre como relatar dados de prova, pois estão relacionados ao projeto. Por exemplo, um relatório de projeto que inclui decisão de prova e comentários.

**Resposta**

Para fazer referência às informações do projeto e às informações de prova em um único relatório, é necessário criar um relatório Aprovação de prova. Atualmente, os comentários de uma prova não podem ser extraídos para esse relatório, no entanto, cada decisão do aprovador de prova pode ser encontrada em seu próprio item de linha na coluna Decisão do aprovador.

**Pergunta**

Eu uso sharecol com frequência para criar status de página única (muitas colunas). No entanto, acho que, se depois de criar um relatório que desejo adicionar uma coluna na parte superior da página, é muito demorado voltar e modificar. Você tem dicas ou truques para fazer esse tipo de mudança?

**Resposta**

Se estiver falando em colocar uma coluna na parte superior de uma lista de colunas do modo texto, bastará renumerar as colunas manualmente.

Mas se você já tiver criado o relatório com a primeira coluna sendo algumas colunas compartilhadas e quiser colocar outra coluna compartilhada no topo da lista, isso é mais fácil.

No editor de relatórios, adicione algumas novas colunas e arraste-as para a extrema esquerda da tela Colunas (Exibir). depois de fazer isso, dê uma olhada no que costumava ser a coluna da esquerda e você observará que os números de coluna do modo texto foram incrementados. Arraste até lá quantas colunas em branco forem necessárias. Certifique-se de colocar algo nessas colunas em branco antes de salvá-las ou elas serão removidas.

**Pergunta**

Olá - no que diz respeito ao relatório final de erros - como os relatórios podem ser feitos para vários projetos - se erros estão chegando para vários projetos?

**Resposta**

Você pode filtrar por portfólio ou projeto, dependendo de como organizou seu trabalho.

Você também pode filtrar por filas de solicitações. Talvez você queira configurar filas de solicitações para cada projeto, onde é possível criar usuários clientes como Revisores que podem fazer logon e enviar tíquetes diretamente para as filas de solicitações que você compartilhou com eles.

**Pergunta**

Os primeiros relatórios foram baseados em projetos/nome do projeto, isso pode ser feito em tarefas também e, em caso afirmativo, qual é a melhor maneira de agrupá-los, pois, possivelmente, o nome da tarefa seria diferente com mais frequência do que não...obrigado!

**Resposta**

Todos esses relatórios podem ser feitos como relatórios de tarefas, problemas ou projetos, dependendo de como você decide rastrear as coisas.

Uma maneira comum de agrupar tarefas seria agrupá-las primeiro pelo nome do projeto e depois pelo nome da tarefa em cada projeto. Dessa forma, se você tiver duas tarefas com o mesmo nome, será fácil ver em qual projeto elas estão.

**Pergunta**

Eu quero saber quais provas estão pendentes, a qual tarefa e projeto eles estão vinculados, quando foi roteado, quando deve e quem é o moderador e o aprovador.

**Resposta**

Provas pendentes podem ser filtradas por Aguardando decisão > Igual > Verdadeiro em um relatório de Aprovação de prova. Há uma coluna para Aprovador, que informará quem ainda não tomou uma decisão.

Você pode fazer referência à tarefa ou ao projeto ao qual a prova está vinculada usando o modo de texto (consulte exemplos abaixo).

```
displayname=Task Name
textmode=true 
valuefield=documentVersion:document:task:name 
valueformat=HTML
```

```
displayname=Project Name
textmode=true 
valuefield=documentVersion:document:project:name
valueformat=HTML
```

Quanto à data do roteamento, data de vencimento e moderador, esses campos atualmente não podem ser extraídos para nenhum dos relatórios do Workfront, portanto, seria necessário clicar no botão Prova diretamente para visualizar essas informações.

**Pergunta**

Você pode configurar um formulário personalizado para enviar automaticamente a um solicitante quando a solicitação for concluída? Como uma pesquisa de &quot;satisfação do cliente&quot;?

**Resposta**

Aqui está uma coisa que você pode fazer que pode atender às suas necessidades. Você pode anexar um Lembrete de Notificação a um problema que enviará um email para &quot;Informado por&quot; depois que for inserida a Data de conclusão efetiva. A pessoa Cadastrada por é a pessoa que criou a ocorrência.

Você criaria a Notificação de lembrete como fizemos no webinário para &quot;Lembrete para preencher a Revisão após a ação (AAR)&quot;, exceto que isso seria um lembrete de Problema. É provável que você queira criar um template de email para ele também para fornecer um link para a pesquisa. Você terá que aplicar a notificação de lembrete manualmente a cada problema (ou usar a edição em massa).

Uma integração seria melhor, pois poderia automatizar as etapas manuais, mas a notificação de lembrete pode ser feita imediatamente.

**Pergunta**

Criei um relatório que mostra projetos por tipo de modelo. Posso listar o proprietário do projeto, mas não as pessoas atribuídas a um projeto.

**Resposta**

Se você quiser puxar a Equipe do projeto (guia Equipe) para uma coluna no relatório do projeto, será necessário criá-la no modo de texto. O modo de texto é o seguinte:

```
displayname=Staffing 
listdelimiter=<p> 
listmethod=nested(projectUsers).lists 
textmode=true
type=iterate 
valuefield=user:name 
valueformat=HTML
```

## Código do Modo de Texto para o Relatório de Envolvimento do AAR

```
column.0.displayname=Task Details
column.0.value=<b>Project Name:</b>&nbsp;
column.0.valueformat=HTML
column.0.sharecol=true
column.1.valuefield=project:name
column.1.valueformat=HTML
column.1.sharecol=true
column.2.value=<br>
column.2.valueformat=HTML
column.2.sharecol=true
column.3.value=<b>Task Name:</b>&nbsp;
column.3.valueformat=HTML
column.3.sharecol=true
column.4.valuefield=name
column.4.valueformat=HTML
column.4.sharecol=true
column.5.value=<br>
column.5.valueformat=HTML
column.5.sharecol=true
column.6.value=<b>Task Owner:</b>&nbsp;
column.6.valueformat=HTML
column.6.sharecol=true
column.7.valuefield=assignedTo:name
column.7.valueformat=HTML
column.7.sharecol=true
column.8.value=<br>
column.8.valueformat=HTML
column.8.sharecol=true
column.9.value=<b>Actual Completion Date:</b>&nbsp;
column.9.valueformat=HTML
column.9.sharecol=true
column.10.valuefield=actualCompletionDate
column.10.valueformat=HTML
column.11.displayname=Name of Reviewer
column.11.linkedname=Name of Reviewer
column.11.namekey=view.relatedcolumn
column.11.namekeyargkey.0=Name of Reviewer
column.11.namekeyargkey.1=name
column.11.querysort=DE:Name of Reviewer:name
column.11.valuefield=Name of Reviewer:name
column.11.valueformat=customReferenceObjectAsString
column.12.displayname=AAR 1
column.12.description=In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.12.value=<b>AAR 1 Score:</b>&nbsp;
column.12.valueformat=HTML
column.12.sharecol=true
column.13.valuefield=AAR 1 - In your view, does the work match stakeholders’ expectations? Did we achieve the intended results?
column.13.valueformat=customDataLabelsAsString
column.13.sharecol=true
column.14.value=<br>
column.14.valueformat=HTML
column.14.sharecol=true
column.15.value=<br><b>AAR 1 User Comment:</b>&nbsp;
column.15.valueformat=HTML
column.15.sharecol=true
column.16.valuefield=AAR 1 User Comment
column.16.valueformat=customDataLabelsAsString
column.17.linkedname=direct
column.17.namekey=AAR 1 Reviewer Comment
column.17.querysort=DE:AAR 1 Reviewer Comment
column.17.valuefield=AAR 1 Reviewer Comment
column.17.valueformat=customDataLabelsAsString
column.18.linkedname=direct
column.18.displayname=AAR 1 Needs Attn
column.18.querysort=DE:AAR 1 Needs Attention
column.18.valuefield=AAR 1 Needs Attention
column.18.valueformat=customDataLabelsAsString
column.19.linkedname=direct
column.19.displayname=AAR 1 Needs Attn Notes
column.19.querysort=DE:AAR 1 Needs Attention Notes
column.19.valuefield=AAR 1 Needs Attention Notes
column.19.valueformat=customDataLabelsAsString
column.20.displayname=AAR 2
column.20.description=Do You Believe This Work Will Make an Impact?
column.20.value=<b>AAR 2 Score:</b>&nbsp;
column.20.valueformat=HTML
column.20.sharecol=true
column.21.valuefield=AAR 2 - Do You Believe This Work Will Make an Impact?
column.21.valueformat=customDataLabelsAsString
column.21.sharecol=true
column.22.value=<br>
column.22.valueformat=HTML
column.22.sharecol=true
column.23.value=<br><b>AAR 2 User Comment:</b>&nbsp;
column.23.valueformat=HTML
column.23.sharecol=true
column.24.valuefield=AAR 2 User Comment
column.24.valueformat=customDataLabelsAsString
column.25.linkedname=direct
column.25.namekey=AAR 2 Reviewer Comment
column.25.querysort=DE:AAR 2 Reviewer Comment
column.25.valuefield=AAR 2 Reviewer Comment
column.25.valueformat=customDataLabelsAsString
column.26.linkedname=direct
column.26.displayname=AAR 2 Needs Attn
column.26.querysort=DE:AAR 2 Needs Attention
column.26.valuefield=AAR 2 Needs Attention
column.26.valueformat=customDataLabelsAsString
column.27.linkedname=direct
column.27.displayname=AAR 2 Needs Attn Notes
column.27.querysort=DE:AAR 2 Needs Attention Notes
column.27.valuefield=AAR 2 Needs Attention Notes
column.27.valueformat=customDataLabelsAsString
column.28.displayname=AAR 3
column.28.description=Are you proud of the work you did on this?
column.28.value=<b>AAR 3 Score:</b>&nbsp;
column.28.valueformat=HTML
column.28.sharecol=true
column.29.valuefield=AAR 3 - Are you proud of the work you did on this?
column.29.valueformat=customDataLabelsAsString
column.29.sharecol=true
column.30.value=<br>
column.30.valueformat=HTML
column.30.sharecol=true
column.31.value=<br><b>AAR 3 User Comment:</b>&nbsp;
column.31.valueformat=HTML
column.31.sharecol=true
column.32.valuefield=AAR 3 User Comment
column.32.valueformat=customDataLabelsAsString
column.33.linkedname=direct
column.33.namekey=AAR 3 Reviewer Comment
column.33.querysort=DE:AAR 3 Reviewer Comment
column.33.valuefield=AAR 3 Reviewer Comment
column.33.valueformat=customDataLabelsAsString
column.34.linkedname=direct
column.34.displayname=AAR 3 Needs Attn
column.34.querysort=DE:AAR 3 Needs Attention
column.34.valuefield=AAR 3 Needs Attention
column.34.valueformat=customDataLabelsAsString
column.35.linkedname=direct
column.35.displayname=AAR 3 Needs Attn Notes
column.35.querysort=DE:AAR 3 Needs Attention Notes
column.35.valuefield=AAR 3 Needs Attention Notes
column.35.valueformat=customDataLabelsAsString
column.36.displayname=Done
column.36.valuefield=Review Complete
column.36.valueformat=customDataLabelsAsString
```
