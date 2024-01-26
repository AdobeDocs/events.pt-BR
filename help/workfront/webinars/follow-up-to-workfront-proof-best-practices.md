---
title: Pergunte a um especialista - Acompanhamento das práticas recomendadas de prova do Workfront
description: Saiba por que você deve usar modelos de fluxo de trabalho automatizados, como criá-los e como ajustar configurações de prova para garantir a privacidade. Esse webinário foi gravado em 4 de março de 2020.
doc-type: feature video
team: Technical Marketing
kt: 9917
exl-id: 2b2f6522-2fd9-4d5e-9bc3-903c1d5e4e3b
duration: 4083
source-git-commit: 9a297cda953d4414131657f9ac84580aea0eabeb
workflow-type: tm+mt
source-wordcount: '1649'
ht-degree: 1%

---

# Pergunte a um especialista - Acompanhamento das práticas recomendadas de prova do Workfront

Saiba por que você deve usar modelos de fluxo de trabalho automatizados, como criá-los e como ajustar configurações de prova para garantir a privacidade. Esse webinário foi gravado em 4 de março de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341123/?quality=12)

## P&amp;R

**Pergunta**

Parece que nossa instância gera provas automaticamente ao carregar documentos. Existe uma maneira de ativar/desativar esta função?

**Resposta**

Sim, esta configuração pode ser desativada no seu perfil pessoal. Se você clicar em Minhas configurações > Preferências, haverá uma caixa de seleção para &quot;Gerar provas automaticamente ao carregar documentos&quot; que pode ser selecionada ou desmarcada.

**Pergunta**

Você pode criar um Fluxo de trabalho que tenha estágios vazios para poder preencher indivíduos após anexá-lo para permitir que várias equipes usem um fluxo?

**Resposta**

Sim, os modelos automatizados de fluxo de trabalho podem ter estágios em branco para que, dependendo da equipe que os utiliza, usuários diferentes possam ser adicionados.

**Pergunta**

No nosso caso de uso, o designer carrega o documento, mas o gerente da conta gera a prova e configura o fluxo de aprovação. Quando uma nova versão é necessária, o designer adiciona a versão como somente documento e o processo é reiniciado. Há uma maneira de fazer com que o gerente de conta gerencie o fluxo de prova e o designer gerencie o controle de versão sem precisar criar o fluxo toda vez que você gerar a nova prova?

**Resposta**

Se você configurar o Designer com um Nível de Acesso de Trabalho ou Plano no Workfront, ele receberá uma licença de prova. Se a licença de prova for definida como Supervisor ou Administrador, será possível criar novas versões de provas sem precisar executar a etapa manual de fazer com que o Gerente de conta converta a nova versão e aplique um fluxo de trabalho. A nova versão adotará o fluxo de trabalho da versão anterior (e também poderá ser alterada ou alterada nesse momento).

**Pergunta**

O que é recomendado para &quot;Alertas de e-mail&quot;? decisões ou todos os alertas?

**Resposta**

Recomendo que o Criador/Proprietário da prova seja definido como &quot;Decisões&quot; para o alerta por email. Recomendo que todos os outros recipients de prova sejam definidos como &quot;Desativado&quot; para o alerta de email (mesmo que o alerta de email esteja definido como desativado, eles ainda receberão notificações de Nova prova, Nova versão, Prova atrasada e @Mention Email). Essa configuração garante que os alertas de email sejam direcionados e mantenham o email em um nível mínimo.

**Pergunta**

Você pode alterar o proprietário da prova que é notificada quando as decisões são tomadas? Tentamos usar a ferramenta de revisão, mas não conseguimos alterar o proprietário do documento da pessoa que carregou o documento original. Exemplo: um gerente de marketing carregou o documento original, mas era um especialista em marketing que era responsável por obter decisões e fazer alterações.

**Resposta**

Para alterar o proprietário da prova, siga este caminho: Documentos > Selecione a prova > Clique em &quot;Detalhes da prova&quot; > Na janela de detalhes da prova, localize o destinatário que você deseja tornar o proprietário da prova > Clique no botão Elipses desse destinatário e escolha &quot;Tornar proprietário&quot;.

**Pergunta**

Existe algum rastreamento do número de rodadas de revisões ocorridas?

**Resposta**

Normalmente, rodadas de revisões correspondem ao número de versões de prova.

**Pergunta**

Uma pessoa pode estar em mais de um estágio? Em outras palavras, se tivermos um gerente em um ciclo de revisão inicial que tenha revisão final em um estágio posterior, como iremos configurar isso?

**Resposta**

Embora não seja possível adicionar um recipient de prova a mais de um estágio da revisão em uma prova, uma vez que o estágio da revisão em que estão esteja esteja ativado, ele estará na prova pelos estágios restantes dessa versão. Isso permitiria que eles continuassem a comentar e responder a comentários mesmo que outras etapas tenham começado. A chave para verificar se isso funciona é garantir que você não tenha estágios bloqueados quando o novo estágio começar.

**Pergunta**

É possível editar workflows existentes?

**Resposta**

Sim, você navegará para Workfront Proof e selecionará Fluxos de trabalho no menu à esquerda. Lá, é possível editar estágios, adicionar usuários, remover usuários, adicionar estágios etc.

**Pergunta**

Há um benefício específico em ter o fluxo de trabalho de aprovação de um documento na prova em vez da tarefa? Configuramos para que esteja na tarefa de desenvolvimento de documentos/arte. Assim, SE a arte for rejeitada em qualquer estágio do processo de aprovação, a tarefa retornará à ação para que o designer atribuído a revise. Dessa forma, não precisamos trabalhar em dois lugares. MAS, talvez eu esteja perdendo algo importante em seguir essa rota.

**Resposta**

No caso da prova, você está gerenciando o processo de aprovação usando o mecanismo de fluxo de trabalho de prova. Isso permite usar a ferramenta de revisão de prova colaborativa para coletar comentários, marcações, decisões e estágios. Você poderá utilizar vários acionadores de fluxo de trabalho para rotear a prova e usar configurações exclusivas dos estágios de prova, como Bloqueio, Estágios privados e Tomadores de decisão principais. Você também tem a opção de atribuir funções de prova exclusivas e notificações por email de prova exclusivas. Além disso, você tem a opção de revisar conteúdo tão variado quanto Provas estáticas, de vídeo e interativas (cerca de 150 tipos de arquivos diferentes).

**Pergunta**

Quem pode definir o estágio como um estágio privado? Somente administradores?

**Resposta**

A criação do template é responsabilidade do administrador, mas qualquer usuário que possa criar uma prova pode tornar o estágio privado.

**Pergunta**

O prazo está incluído na notificação por email?

**Resposta**

Sim, se você aplicar um prazo a uma prova, ela aparecerá na notificação por email.

**Pergunta**

É possível compartilhar um modelo com um grupo de prova?

**Resposta**

Você pode - no entanto, observe que ela só será compartilhada com membros do grupo que têm Licenças de comprovação. Você não poderá compartilhar modelos com Usuários ou Convidados do Workfront que não têm licenças de prova.

**Pergunta**

Como uma prova é encaminhada para o proprietário da prova se for rejeitada?

**Resposta**

O proprietário da prova permanece na prova em todos os estágios de prova. Se a prova for rejeitada, a prova em si não precisará ser encaminhada de volta ao proprietário. Em vez disso, o proprietário da prova será notificado por email sobre a decisão tomada, revisará os comentários e começará a usar uma nova versão.

**Pergunta**

Como desativar/ocultar o documento &quot;Download&quot; no Proof?

**Resposta**

Ao adicionar uma nova prova, role até a parte inferior até chegar às Configurações de prova. Você verá uma caixa de seleção &quot;Baixar arquivo original&quot; que pode ser marcada ou desmarcada?

**Pergunta**

Como essa configuração de privacidade nas Configurações da conta afeta os usuários de comprovação que estão usando especificamente a comparação automatizada (lado a lado com a comparação automática) — A configuração padrão Desabilitado impede que o revisor compare duas versões?

**Resposta**

Para a configuração de compartilhamento de &quot;Destinatários podem exibir todas as versões&quot; - se estiver definida como &quot;Desativado&quot;, se o destinatário não estiver na versão 1, mas na versão 2, ele não poderá comparar as versões 1 e 2. Observe que os usuários do Workfront com o nível de Permissão de Prova de Supervisor ou Administrador poderão ver todas as versões, independentemente da configuração.

**Pergunta**

Podemos ter várias pessoas carregando uma nova versão? por exemplo, um redator carrega a versão 1 e depois temos o revisor no estágio 1. Eles veem uma alteração que precisa ser feita. O upload pode ser da versão 2?

**Resposta**

É possível fazer com que os recipients de prova criem novas versões de provas se atenderem aos seguintes critérios: 1) Eles são o proprietário da prova ou 2) Estão definidos com a função de prova Autor ou Moderador na prova ou 3) Estão configurados com o Nível de permissão de prova de Supervisor ou Administrador.

**Pergunta**

Como lidar com várias provas (p. ex., A, B e C) com o workflow automatizado. Você começa de novo?

**Resposta**

Você pode aplicar um template de fluxo de trabalho automatizado a várias provas no momento da criação da versão inicial das provas. Para fazer isso, siga este caminho: Documentos > Adicionar novo > Prova. Na página Nova prova, selecione vários arquivos para fazer upload, aplique o modelo de fluxo de trabalho automatizado e crie as provas.

**Pergunta**

Uma prova pode ser exportada com comentários para um PDF?

**Resposta**

É possível exportar um Resumo de impressão em uma prova para um arquivo PDF. Ele conterá todos os comentários, marcações, respostas e decisões.

**Pergunta**

Onde posso ver as configurações de prova?

**Resposta**

Para ver as configurações de prova em uma prova existente, siga este caminho: Guia Documentos > Selecione a prova > Clique em &quot;Detalhes da prova&quot; > Na janela Detalhes da prova que é aberta, é desejável expandir a área &quot;Configurações&quot;.

**Pergunta**

Você pode marcar alguém no palco privado?

**Resposta**

Se você for um recipient de prova no estágio privado, poderá marcar qualquer pessoa nesse estágio privado. Se você não estiver no estágio privado, não será possível marcar alguém no estágio privado.

**Pergunta**

Depois de ativar um estágio, você pode desativá-lo?

**Resposta**

Você não poderá desativar um estágio ativo, no entanto, poderá &quot;Bloquear&quot; o estágio, o que impedirá que as pessoas dentro dele façam comentários e tomem decisões.

**Pergunta**

O que acontece nos bastidores quando um ou mais revisores em um estágio dizem que as alterações são necessárias? Quem é notificado a fazer upload de uma nova versão?

**Resposta**

Isso dependerá da configuração &quot;Alerta de email&quot; do criador e/ou dos recipients da prova na prova. Recomendo que os Criadores/proprietários de provas sejam definidos com o Alerta por email de &quot;Decisões&quot; para que sejam notificados por email sempre que uma decisão for tomada sobre a prova.
