---
title: Pergunte a um especialista - Noções básicas sobre combinação e capacidade
description: Saiba como medir a combinação e a capacidade em sua empresa. Este webinário foi gravado em 2 de outubro de 2019.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9913
exl-id: 5993c6c3-0583-4d1c-94aa-2e64a699e7f1
source-git-commit: ca06e5a8b1602a7bcfb83a43f529680a5a96bacf
workflow-type: tm+mt
source-wordcount: '2224'
ht-degree: 1%

---

# Pergunte a um especialista - Noções básicas sobre combinação e capacidade

Saiba como medir a combinação e a capacidade em sua empresa. Este webinário foi gravado em 2 de outubro de 2019.

>[!VIDEO](https://video.tv.adobe.com/v/341119/?quality=12)

## P&amp;R

**Pergunta**

Como você coloca %s em um gráfico de colunas?

**Resposta**

Os valores % listados no Relatório de combinação estavam lá porque, na guia do gráfico, escolhemos &quot;Colunas de grupo&quot; e &quot;Empilhado a 100%&quot;. Se escolhêssemos &quot;Empilhado&quot;, mostraria os totais de horas planejadas e não o percentual.

**Pergunta**

Se a carga de trabalho de seu departamento/organização for uma combinação de projetos/tarefas e problemas/solicitações, como é recomendável obter uma análise de alto nível (em um relatório do Workfront) de um WPI?

**Resposta**

Projetos, tarefas e problemas precisam ter seus próprios relatórios com seus próprios formulários personalizados. No entanto, cada um deles pode usar o mesmo campo Tipo de trabalho. Talvez você queira exibir os três relatórios em um painel.

**Pergunta**

Precisamos editar tarefas em massa para torná-las operacionais ou estratégicas?

**Resposta**

A técnica que estamos sugerindo é criar um relatório que permitirá obter uma lista de tarefas operacionais. Depois disso, você pode selecionar todas as tarefas de uma só vez, editá-las em massa, anexar o formulário personalizado com o Tipo de trabalho e definir o tipo de trabalho como Operacional para todas as tarefas de uma só vez. Você seguiria o mesmo procedimento para coletar uma lista de tarefas estratégicas, editá-las em massa e adicionar o formulário personalizado etc.

Algumas ideias são mencionadas no webinário para prompts personalizados que podem ajudar você a obter uma lista, como verificar determinadas palavras no nome da tarefa, no proprietário do projeto, no portfólio ou nos usuários atribuídos. Estas são apenas ideias. Você deve criar um relatório que funcione melhor em sua situação.

**Pergunta**

Se eu tiver 4 categorias em minha combinação, posso criar uma meta para cada e, em seguida, relatar o delta entre previsão versus plano versus real? (4 categorias: Campanha, Unidade de negócios, Web e Produto). No nível do projeto, temos as categorias em campos/formulários personalizados. A meta seria criar uma previsão trimestral (orçamento/previsão) e, em seguida, rastrear as horas planejadas em direção a ela e, por fim, real.

**Resposta**

Se você tiver todas as categorias em um campo personalizado (vamos chamá-lo de Tipo de trabalho por enquanto), basta criar um agrupamento de relatório de projeto em Horas planejadas primeiro e Tipo de trabalho em segundo. Filtre seu relatório de projeto para mostrar os projetos no Planning dentro dos intervalos de datas desejados. Use um gráfico com colunas ou barras agrupadas até 100% se desejar visualizar porcentagens. Pode ser o seu Relatório de previsão.

Você pode copiar o relatório e editá-lo para criar um relatório baseado em projetos Atuais, ainda mostrando a combinação baseada em Horas planejadas.

Você pode copiar o relatório novamente, alterá-lo para agrupar por Horas efetivas em vez de Horas planejadas e mostrar somente projetos concluídos dentro dos intervalos de datas desejados. Isso mostraria a combinação de porcentagem com base nas horas reais.

**Pergunta**

Isso funcionará se você tiver várias IDs de categoria em um projeto ou tarefa?

**Resposta**

Sim, se você tiver várias IDs, elas precisarão ser separadas por uma guia, desta forma:

```
EXISTS:1:$$EXISTSMOD=NOTEXISTS
EXISTS:1:$$OBJCODE=OBJCAT
EXISTS:1:categoryID=5d76d82600e7926bb51eeb1e0886810e 5d54288d01034619f2eb2c74f6472f18
EXISTS:1:objID=FIELD:ID
```

A melhor maneira de separá-las com um caractere de tabulação é criar primeiro a lista de categorias no construtor. Coloque vários nomes de formulário personalizados e, ao alternar para o modo de texto, você os verá como IDs separadas por guias.

As várias IDs são tratadas como ORs, portanto, se qualquer uma delas estiver anexada à tarefa, ela não aparecerá no relatório.

**Pergunta**

Os prompts do relatório são &#39;ANDed&#39; ou &#39;ORed&#39;?

**Resposta**

Os prompts personalizados individuais são &#39;ANDed&#39;. Portanto, se você especificar Pam como o proprietário do projeto e Faturar como atribuído à tarefa, verá apenas as tarefas atribuídas a Bill que estão em projetos em que Pam é o proprietário do projeto.

**Pergunta**

Por que você só pode classificar por determinadas colunas? Ou seja, não é possível classificar por atribuições.

**Resposta**

&quot;Atribuições&quot; é uma lista, e você não pode classificar ou agrupar em uma lista de itens. Você só pode classificar ou agrupar em um item individual.

Para ilustrar o ponto, imagine uma lista de atribuições como esta em uma tarefa:

```
Jane
Bill
Dan
```

E uma lista de atribuições como esta em outra tarefa:

```
Bill
Jane
Helen
```

Qual tarefa deve aparecer primeiro em uma classificação? Você poderia dizer &quot;classificar pelo nome na lista&quot;, mas isso não é necessariamente útil, já que você não pode controlar a ordem. O Workfront evita o problema não permitindo que você classifique por listas.

E quanto ao agrupamento por uma lista? Se pudéssemos agrupar por uma lista de nomes, você encontraria todas as tarefas atribuídas a Jane, Bill, Dan agrupadas e todas as tarefas atribuídas a Jane, Dan, Bill (mesma lista, mas em uma ordem diferente) em um agrupamento diferente. Novamente, o Workfront evita o problema não permitindo o agrupamento por listas.

**Pergunta**

As horas planejadas são usadas para tarefas estratégicas e as horas reais para operacionais?

**Resposta**

Não. Em nosso exemplo, estamos usando o Trabalho necessário para mostrar o nível de esforço planejado para tarefas estratégicas e operacionais. Isso nos permite compará-los facilmente, seja no passado, presente ou futuro. Você também pode usar as horas reais para comparar tarefas estratégicas e operacionais, mas apenas para tarefas no passado, desde que as horas reais, são as horas que as pessoas relataram como o tempo que realmente gastaram trabalhando nas tarefas.

**Pergunta**

No planejador de recursos, como contabilizar tarefas que foram planejadas no passado, mas não concluídas? As horas planejadas não parecem ser transferidas e, portanto, não são exibidas em semanas futuras como tarefas/horas que precisam de recursos.

**Resposta**

Não há rolagem &quot;automática&quot; para frente de trabalho incompleto. Você precisará replanejar seu projeto quando isso acontecer. Talvez os recursos originalmente atribuídos a uma determinada tarefa não estejam disponíveis no novo período, portanto, o gerente do projeto deve analisar isso e decidir a melhor maneira de replanejar. Isso pode significar envolver as partes interessadas e obter aprovações para as alterações no plano.

**Pergunta**

Em vez de inserir 2 horas/dia para verificar emails, intervalos, você recomendaria ajustar o FTE?

**Resposta**

Sim, se você definir o FTE como 0,75, isso mostrará um usuário como disponível 6 horas por dia no Planejador de recursos. Essa será a disponibilidade deles todos os dias. Se desejar mostrá-los como indisponíveis para períodos diferentes dependendo da data, como indisponível no último dia de cada trimestre, um projeto de despesas gerais é a maneira de fazer isso.

Algumas pessoas preferem projetos de despesas gerais porque podem criá-los para si mesmos e alterá-los quando quiserem, ao passo que podem não ter direitos para editar seu próprio FTE.

**Pergunta**

Os dados do painel de capacidade da equipe estão disponíveis para qualquer pessoa com quem você compartilha o relatório, independentemente das permissões que eles têm no trabalho?

**Resposta**

Se um usuário não tiver permissão para visualizar o objeto, ele não estará visível no relatório/painel. No entanto, se desejar que todos vejam os mesmos resultados, você pode acessar Ações de relatório > Editar > Configurações de relatório e inserir seu nome no campo, &quot;Executar este relatório com os direitos de acesso de&quot;. Isso permitirá que os usuários compartilhados neste relatório vejam os resultados exatos que você vê. Ele não concederá a eles acesso adicional ao resultado em si, portanto, alguns resultados podem ou não ser clicáveis.

**Pergunta**

Como podemos criar um relatório que mostre toda a equipe atribuída a um projeto em geral (não no nível de tarefa)?

**Resposta**

Você pode criar uma coluna em um Relatório de projeto que mostre todos os usuários listados como parte da guia Equipe (Equipe do projeto). Você usará o seguinte modo de texto:

```
displayname=Project Team
listdelimiter=<p>
listmethod=nested(projectUsers).lists
textmode=true
type=iterate
valuefield=user:name
valueformat=HTML
```

**Pergunta**

Eu gostaria de ter um relatório/painel que incorpore como minha equipe trabalha. Em particular, os seguintes cenários: - Projetos dos quais sou proprietário / Projetos criados para mim / Tarefas que atribuí a outros / Tarefas atribuídas a mim

**Resposta**

Projetos dos quais sou proprietário

Há um relatório integrado chamado &quot;Projetos atuais&quot; que mostrará todos os projetos atuais. É possível editar esse projeto e adicionar uma regra de filtro: Projeto > ID do proprietário > Igual > $$USER.IDTe salvar e renomear o relatório como &quot;Projetos que possuo&quot;.

Projetos criados para mim

Há um relatório interno chamado &quot;Meus projetos&quot; que mostrará todos os projetos atuais dos quais você faz parte da equipe do projeto (ou seja, você é o Proprietário, Patrocinador ou está atribuído à tarefa). Não tenho certeza se é isso que você está solicitando, mas não há outras maneiras de saber se alguém criou um projeto para você além de torná-lo o proprietário do projeto, patrocinador ou atribuir você a uma tarefa.

Tarefas atribuídas a outros

Crie um relatório de tarefas com os filtros que quiser, vá para a guia Filter e clique em Switch to Text Mode (Alternar para modo de texto). Adicionar este código ao que já estiver lá:

```
EXISTS:1:$$OBJCODE=ASSGN
EXISTS:1:taskID=FIELD:ID
EXISTS:1:assignedByID=$$USER.ID
```

Isso mostrará todas as tarefas em que o usuário conectado atribuiu pelo menos um dos atribuídos atuais. Se os atribuídos foram atribuídos por várias pessoas, somente o nome da primeira pessoa que atribuiu alguém será exibido como &quot;Solicitado por&quot; na landing page da tarefa. Se quiser ver todas as pessoas atribuídas e que atribuíram cada uma, você pode adicionar uma coluna à sua visualização, alternar para o modo de texto e substituir o que houver com isso:

```
displayname=All Assignees and Requesters
listdelimiter=<p>
listmethod=nested(assignments).lists
textmode=true
type=iterate
valueexpression=CONCAT("Assigned To: ",{assignedTo}.{name},"; Requested By: ",{assignedBy}.{name})
valueformat=HTML
```

Tarefas atribuídas a mim

Há um relatório interno chamado &quot;Minhas tarefas&quot; que mostrará todas as tarefas incompletas nos projetos atuais onde você é o proprietário da tarefa. Sugiro alterar o filtro para mostrar todas as tarefas em que você é um dos muitos usuários atribuídos em potencial, não apenas o proprietário da tarefa. Para fazer isso, remova a regra de filtro

```
Task > Assigned To ID > Equal > $$USER.ID 
```

e substituindo-o por

```
Assignment Users > ID > Equal > $$USER.ID
```

**Pergunta**

Há uma maneira de personalizar rótulos em gráficos? Descobri que quando crio um gráfico para refletir os status do projeto, o nome do grupo inicial acaba sendo incluído no rótulo.

**Resposta**

Os rótulos nos gráficos usam o nome do campo no qual você está agrupando. Portanto, a única maneira de alterar os rótulos é usar um campo personalizado calculado com o nome que você quiser. Na seção de cálculo do campo, coloque o nome do campo nativo pelo qual você deseja agrupar.

**Pergunta**

Como você codifica as barras de relatório nas Atribuições de Equipe do Chuck, por favor? Ou seja, âmbar para trás, vermelho para tarde e verde para no prazo? Você também pode alterar a ordem para ser mais lógica, ou seja, vermelha/âmbar/verde ou o inverso?

**Resposta**

Para alterar as cores usadas no relatório para as opções de Status do Progresso, edite o relatório e clique na guia Gráfico. Procure o menu suspenso &quot;Cores personalizadas >&quot;. Ele aparecerá ao lado da caixa &quot;Eixo esquerdo (Y)&quot; ou da caixa &quot;Agrupar dados por&quot;, dependendo se você optar por agrupar colunas ou barras. Nessa lista suspensa é possível selecionar cores. Se você clicar nos números no canto inferior direito das opções de cores, será possível selecionar sua cor em uma paleta maior.

Infelizmente, não é possível alterar a ordem desses itens.

**Pergunta**

É possível criar um gráfico onde ele aponte para a Contagem de projetos na qual uma tarefa é atribuída a um trabalhador?

**Resposta**

Sim, veja como:

* Criar um relatório de projeto
* Se o usuário em questão for o usuário conectado, o filtro deverá incluir esta linha:

```
   Project Users > ID > Equal >$$USER.ID 
```

* Caso contrário, coloque o nome de usuário no lugar de [!DNL $$USER.ID]. Isso mostrará todos os projetos aos quais uma tarefa foi atribuída a essa pessoa, ou que é o proprietário ou patrocinador. Se você quiser ver apenas os projetos nos quais as tarefas são atribuídas, adicione estas duas regras de filtro adicionais:

```
   Project > Owner ID > Not Equal > $$USERID
   Project > Sponsor ID > Not Equal > $$USERID
```

* Crie pelo menos um agrupamento para poder criar um gráfico. Agrupar em qualquer coisa, como companhia. Então clique na guia Chart e escolha um gráfico. &quot;Contagem de registros&quot; será o padrão para um eixo. Este será o número de projetos nos quais o usuário tem uma atribuição.

Quando um usuário recebe uma atribuição em um projeto (atribuído a uma tarefa ou proprietário de projeto ou patrocinador do projeto), essa pessoa é adicionada à equipe do projeto e pode ser vista na guia Equipe, na subguia Pessoas. Se um usuário não for mais o proprietário do projeto, patrocinador ou qualquer atribuição de tarefa, seu nome ainda estará na equipe do projeto. Eles devem ser removidos manualmente se você quiser que sejam removidos. Lembre-se de que isso pode afetar a precisão dos resultados do relatório. Para remover alguém da equipe do projeto, vá para Equipe > Pessoas, selecione a pessoa ou as pessoas e clique no botão Remover exibido acima da lista.

**Pergunta**

Como você pode alterar a ordem decrescente de uma coluna no modo de texto (em um agrupamento)?

**Resposta**

Você pode optar por classificar a maioria das colunas na guia Colunas (Exibição) ao criar um relatório. Isso classificará o relatório de lista inteiro se você não tiver agrupamentos. Se você tiver agrupamentos, eles serão classificados de acordo com essa escolha em cada agrupamento.

**Pergunta**

Como posso criar uma coluna que identificará Membros da Equipe atribuídos a um estágio de aprovação?

**Resposta**

Se você estiver executando um relatório de Tarefa ou Problema/Solicitação, há uma coluna disponível no Report Builder chamada &quot;Aprovadores e Status&quot; que fornecerá essas informações.
