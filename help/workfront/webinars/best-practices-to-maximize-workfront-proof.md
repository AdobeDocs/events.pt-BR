---
title: Pergunte a um especialista - Práticas recomendadas para maximizar a prova do Workfront
description: Saiba como definir configurações, habilitar ótimos relatórios e evitar armadilhas comuns no Proof. Esse webinário foi gravado em 26 de fevereiro de 2020.
activity: use
doc-type: feature video
team: Technical Marketing
kt: 9916
exl-id: 7d3e437d-4a6e-44b8-9eff-eabb8284c391
source-git-commit: 1792dc318643aec2c12613f621361d72a7a918b1
workflow-type: tm+mt
source-wordcount: '5566'
ht-degree: 2%

---

# Pergunte a um especialista - Práticas recomendadas para maximizar a prova do Workfront

Saiba como definir configurações para sucesso, acessar visualizações (e outros truques) para permitir excelentes relatórios e entender como evitar armadilhas comuns no Proof. Esse webinário foi gravado em 26 de fevereiro de 2020.

>[!VIDEO](https://video.tv.adobe.com/v/341122/?quality=12)

## P&amp;R

**Pergunta**

Atualmente, para dar a um recipient a capacidade de compartilhar uma prova que foi compartilhada com ele, você precisa marcar manualmente a caixa &quot;subscrição&quot; nas configurações de prova. Há planos para tornar essa caixa de seleção automática por padrão?

**Resposta**

Isso pode ser ativado/desativado como padrão para usuários individuais por um administrador seguindo este caminho: PHQ Logon > Configurações da conta > Usuários > Clique no Nome do usuário > Configurações de prova padrão.

**Pergunta**

Se você não selecionar &quot;Nova prova&quot; e carregar um documento e o usuário estiver definido como &quot;gerar prova automaticamente&quot;. Você pode modificar essas configurações depois que os arquivos já tiverem sido carregados?

**Resposta**

Sim. É possível ajustar todas as configurações de prova selecionando a prova na guia Documentos e clicando em Detalhes da prova.

**Pergunta**

Esta apresentação é aplicável à ferramenta independente?

**Resposta**

O Recommendations em funções de prova, alertas de email, opções de decisão, encaminhamento de emails e agrupamento/compartilhamento/configurações de modelo de fluxo de trabalho são relevantes para prova independente.

**Pergunta**

Para que você usaria um modelo de prova?

**Resposta**

Se o processo de revisão de conteúdo da sua organização for repetido com frequência ou o conteúdo for revisado com frequência pelas mesmas pessoas, você poderá criar modelos de fluxo de trabalho que contenham esses revisores com funções de prova e configurações de notificação especificadas.

**Pergunta**

O que é um modelo de fluxo de trabalho de prova?

**Resposta**

Um modelo de fluxo de trabalho de prova é um modelo com um fluxo de trabalho de roteamento de prova predeterminado que pode ser aplicado a provas. Eles permitem padronizar e automatizar processos de aprovação de prova.

**Pergunta**

Como você pode criar um template de prova?

**Resposta**

Como Administrador, você deverá seguir este caminho: PHQ Login > Workflows > New > New Template.

**Pergunta**

Essa funcionalidade de Compartilhamento de modelo permite o compartilhamento com Grupos e Equipes ou apenas usuários individuais?

**Resposta**

No momento, não é possível compartilhar modelos de fluxo de trabalho com Grupos, Equipes, Funções de trabalho ou Empresas da Workfront. No entanto, você pode compartilhá-los com indivíduos e compartilhar com Grupos de prova. Para criar um Grupo de prova, siga este caminho: PHQ Login > Groups > New Group.

**Pergunta**

Ao enviar uma prova - em Organização - há um meio de limpar as pastas que cada usuário vê para que ele veja apenas as pastas que são aplicáveis a ele? Em vez de todas as pastas que foram feitas na conta das empresas?

**Resposta**

Essa pergunta está relacionada ao Workfront Proof Standalone. No Workfront Proof independente, é possível utilizar Pastas privadas para ocultar pastas de usuários específicos. Isso permitirá uma lista mais simplificada de pastas para escolher. Observe que você também pode usar a lógica de digitação antecipada para localizar a pasta à qual deseja adicionar uma prova também.

**Pergunta**

Os revisores e aprovadores têm a opção de alterar essas configurações de notificação?

**Resposta**

Os administradores do Workfront podem alterar as configurações padrão de alerta por email para usuários e contatos. Os criadores de prova podem alterar a configuração de notificação ao criar uma prova, bem como em suas provas existentes.

Os recipients nas provas sempre podem alterar o alerta por email para provas específicas no nível de prova na ferramenta Visualizador de prova selecionando o ícone Configurações no menu esquerdo.

**Pergunta**

Os alertas de email substituem as notificações globais?

**Resposta**

Os alertas de email de prova são completamente independentes das configurações globais de notificação.

**Pergunta**

Se os revisores estiverem definidos como &quot;desativados&quot;, como eles saberão se há uma nova prova para que revisem se rejeitaram uma anterior?

**Resposta**

Os Alertas por email são independentes do Novo email de prova, Novo email de versão, Email de risco, Email tardio e Email @Mentions. Se você escolher &quot;Desativado&quot; como o Alerta por email, apenas desativará as notificações sobre atividades, como comentários, respostas e decisões na prova (com exceção de emails @Mention de comentários).

**Pergunta**

A configuração Desativar emails está definida para toda a Empresa? ou é por Portfolio?

**Resposta**

A configuração localizada em Configuração > Email > Revisar e aprovar que ativa/desativa o envio de emails quando os recipients de prova fazem comentários é empresarial (é uma configuração global).

**Pergunta**

Tenho um usuário &quot;Convidado&quot; que foi adicionado à Prova e não pode revisá-la. E o usuário não tem acesso ao Workfront.

**Resposta**

Se o Convidado puder acessar a prova, mas não fizer comentários/decisões, verifique sua Função de prova na prova. Nesse caso, elas podem ter sido adicionadas à prova com a função de prova &quot;Somente leitura&quot;. Se eles estiverem configurados como Revisor ou Revisor e Aprovador na prova e ainda não puderem fazer comentários/marcações/decisões, envie um tíquete de suporte.

**Pergunta**

Os usuários convidados exigem uma licença?

**Resposta**

Os usuários convidados não exigem uma licença.

**Pergunta**

Não vejo a caixa de decisão da prova?

**Resposta**

Se não vir a caixa de decisão da prova em uma prova, você pode estar configurado na prova com a função de prova Somente leitura ou Revisor, ou o estágio em que você está na prova ainda não começou.

**Pergunta**

Você pode esclarecer a configuração em WF>Configuração - se você tiver a opção de enviar email para cada comentário - eles são enviados mesmo se o email no PHQ estiver Desativado? e quem recebe os emails?

**Resposta**

A opção Workfront Setup > Email > Review and Approval notification é independente das opções de Alerta de email no nível de prova. Se isso estiver ativado, todos em cada prova receberão um email sempre que alguém na prova em que estão fizer um comentário.

**Pergunta**

Anteriormente, você recomendava &quot;desativado&quot; para alertas de email fora do proprietário da prova. Os recipients ainda receberão uma notificação por email informando que uma prova foi atribuída a eles nesse caso?

**Resposta**

Sim. Os Alertas de email (que podem ser definidos como Todas as atividades, Desativados, Decisões etc.) são independentes dos Emails de notificação de prova (Nova prova, Nova versão, À prova de risco, Prova atrasada, @Mentions).

**Pergunta**

E se você tiver uma instância em que alguém é adicionado a uma prova e ela achar que não deve estar lá? Remover &quot;Não Relevante&quot; não daria a eles uma opção de escolha?

**Resposta**

Essa é uma boa utilização para a opção Not Relevant Decision. No entanto, se alguém não deve estar na prova, eu recomendaria que @Mention o proprietário da prova em um comentário sobre a prova e peça para ser removido. Se alguém que deve tomar uma decisão sobre a prova tomar a decisão de &quot;Não relevante&quot; quando deve tomar uma decisão de Aprovado ou Alterações exigidas, isso pode alterar a forma como o fluxo de trabalho aplicado a essa prova funciona.

**Pergunta**

Onde posso encontrar a caixa de seleção para &quot;exigir logon&quot; para usuários convidados?

**Resposta**

Ele estará localizado nas Configurações de prova na página Criação de prova ao criar uma prova. Se a prova já tiver sido criada, acesse essa configuração selecionando a prova na guia Documentos e clicando em Detalhes da prova > Configurações. Observe que você só pode compartilhar provas de logon necessário com pessoas que tenham uma licença de revisão.

**Pergunta**

Alguém pode remover a si mesmo de uma prova se tiver sido adicionado por outra pessoa?

**Resposta**

Se a pessoa tiver direitos de edição para a prova de que foi adicionada a ela, ela poderá remover a si mesma. As pessoas com direitos de edição serão usuários do Workfront com uma licença de revisão de nível de administrador ou supervisor, bem como pessoas adicionadas à prova com funções de prova de Autor ou Moderador. Qualquer outra pessoa precisará ser removida por alguém com direitos de edição.

**Pergunta**

Por que usar aprovação de documento vs. aprovação de prova ou vice-versa?

**Resposta**

A Aprovação de documento pode ser usada para um documento que não requer comentários e marcações alinhadas com o documento que está sendo aprovado. Por exemplo, eu só preciso que você veja este documento e aprove-o ou rejeite-o. A prova permitirá comentários e marcações no documento na ferramenta Visualizador de prova. Por exemplo, preciso que você veja essa prova, adicione comentários, adicione marcações e tome uma decisão. No futuro, o plano é unificar as duas funcionalidades, pois são muito semelhantes.

**Pergunta**

Somos um departamento de marketing e fazemos uma aprovação de prova interna e precisamos enviar externamente para o solicitante. Não damos acesso aos Solicitantes aos nossos projetos. Também não queremos que eles vejam todos os nossos comentários na prova interna. Agora estamos fazendo uma nova prova limpa e baixando-a e enviando-a por email para eles. Queremos fazer com que eles usem o Proof HQ, mas não temos certeza de como fazer isso sem ele também dá acesso ao nosso projeto. Alguma sugestão?

**Resposta**

Eu recomendaria usar Modelos de fluxo de trabalho automatizados que permitirão utilizar &quot;Estágios privados&quot;. Estágios privados permitem ocultar comentários, marcações e decisões de Revisores convidados em outros estágios. Isso permitiria que a Revisão de prova interna ficasse completamente oculta do solicitante externo.

**Pergunta**

Depois que uma prova é criada por outra pessoa, qual é a melhor maneira de se adicionar como revisor e aprovador?

**Resposta**

Se você for um usuário do Workfront com a Permissão de Prova de Administrador ou Supervisor, poderá adicionar a si mesmo como Revisor e Aprovador a qualquer prova à qual tenha acesso. Caso contrário, você deverá adicionar o proprietário da prova (ou outra pessoa com direitos de edição à prova).

**Pergunta**

Tentamos marcar os usuários em uma prova, mas eles não recebem uma notificação por email. Há algo nas configurações da conta para garantir que um email seja enviado?

**Resposta**

Eu recomendaria verificar os Filtros de email / Pasta de spam para ver se as notificações foram lá e, em seguida, fazer os ajustes necessários no aplicativo de email para adicionar esses emails à lista de permissões. Você também pode entrar em contato com nossa equipe de suporte para obter assistência.

**Pergunta**

Você só pode @ alguém se eles têm uma licença de prova, correto? Como no, essa pessoa nunca esteve na prova e você deseja marcá-la (@).

**Resposta**

Se você for um convidado ou um usuário do Workfront com uma licença de comprovação do gerente, é possível @Mention qualquer pessoa que esteja na prova (independentemente de essa pessoa ter ou não uma licença). Se você for um usuário do Workfront com uma licença de revisão do supervisor ou administrador ou se for o proprietário da prova, poderá @Mention qualquer pessoa na Lista de contatos na plataforma de prova.

**Pergunta**

Maior problema aqui: endereçamento de email %2B (endereços de email duplicados). Por que e como isso acontece e como isso pode ser remediado?

**Resposta**

Isso pode acontecer se alguém adicionar alguém a uma prova manualmente usando o endereço de email errado. Se você encontrar isso, um administrador poderá remover o endereço de email incorreto da conta do Proof seguindo este caminho: PHQ Login > Contatos > Selecione o email incorreto / instância do convidado > Excluir. Se você estiver com problemas com usuários adicionados com endereços de email duplicados, entre em contato com a equipe de suporte para obter assistência.

**Pergunta**

Depois que uma decisão é tomada e você precisa alterar a prova para produção. Que tipo de acesso você precisa dar à equipe de produção para que ela possa usar a ação do comentário se a prova estiver bloqueada?

**Resposta**

Se uma prova estiver bloqueada, será necessário desbloqueá-la para que as pessoas façam comentários ou respondam aos comentários. As pessoas com as seguintes permissões podem desbloquear a prova: O proprietário da prova, usuários do Workfront com nível de licença de prova de administrador ou supervisor.

**Pergunta**

Qual é a melhor solução para que as equipes conheçam provas que já estão na fila de pessoas?

**Resposta**

Você pode criar um relatório Aprovações de provas dentro do Workfront. É possível aplicar filtros para exibir provas apenas para usuários específicos que ainda exigem que uma decisão seja tomada.

**Pergunta**

Há uma maneira de baixar provas com suas aprovações associadas em uma pasta?

**Resposta**

É possível acessar e baixar um relatório de Resumo de impressão para suas provas, que incluirá todos os comentários, respostas, marcações, ações e decisões em todas as versões.

**Pergunta**

Ao solicitar que os usuários tenham acesso ao ProofHQ de relatórios, isso também dará a eles acesso à seção à esquerda (ou seja, fluxos de trabalho, contatos, configurações de conta etc.)?

**Resposta**

Isso dependerá do Nível de licença de prova. Se estiverem configurados com a licença de Gerente ou Supervisor, eles poderão acessar os Contatos, mas não poderão acessar as Configurações de conta e os Fluxos de trabalho. Se configurado com a licença de Administrador, ele terá acesso a Configurações de conta e Fluxos de trabalho.

**Pergunta**

Na minha organização, o Gerente de projetos envia uma solicitação de aprovação às partes interessadas para revisão/comentários. Você mencionou que não devemos Adicionar nomes aos campos de Aprovação, como o PM compartilha a prova criativa com as partes interessadas?

**Resposta**

O campo Aprovação é para Aprovações de documentos, que é útil se você precisar apenas de uma aprovação de documento simples. Se desejar uma Aprovação de prova (com comentários, marcações e uma decisão de prova), adicione as Partes interessadas à prova com a função de Revisor e Aprovador.

**Pergunta**

Como você adiciona pessoas como novas funções em qualquer prova que já foi criada?

**Resposta**

Para adicionar recipients de prova e selecionar sua função de prova em uma prova existente, siga este caminho: selecione a prova na guia Documentos > e clique em Detalhes da prova. Quando a janela de detalhes da prova for aberta, clique no botão Elipses no canto superior direito do estágio e selecione &quot;Compartilhar&quot;. É possível adicionar os recipients e selecionar a função de prova e o alerta de email.

**Pergunta**

Se concedermos acesso ao Proof HQ a gerentes/criadores de prova, podemos bloquear as áreas de administração, como workflows, grupos etc.?

**Resposta**

Sim, isso é determinado pela Permissão de prova do usuário. Os usuários com a permissão de prova de gerente ou supervisor não terão acesso às configurações da conta e aos modelos de fluxo de trabalho. Os usuários com a permissão de prova de administrador terão acesso às configurações da conta e aos modelos de fluxo de trabalho. Todos os usuários com acesso poderão acessar a área Grupos.

**Pergunta**

Como os usuários podem ver todas as provas às quais estão atribuídos sem serem gerentes de prova?

**Resposta**

Se um usuário quiser ver todas as provas de que ainda precisa tomar uma decisão, ele poderá usar a área Página inicial ou Minhas atualizações no Workfront (dependendo de seu nível de acesso). Você também pode criar um relatório Aprovação de prova e aplicar filtros para mostrar apenas provas de que o usuário conectado é um Revisor e Aprovador na.

**Pergunta**

Olá, você pode ver os workflows de comprovação automatizada para situações em que há 3 rodadas de design e feedback e como acomodar quando o feedback é fornecido tardiamente e como isso pode ser melhor vinculado às tarefas no WF para cada rodada (feedback do design e do gerente de projeto)?

**Resposta**

Ao mesmo tempo em que você pode usar várias abordagens diferentes para utilizar tarefas com Revisão e aprovação. Uma abordagem que gosto de fazer é ter uma tarefa para &quot;Roteamento de prova&quot; e uso o fluxo de trabalho de prova para gerenciar as notificações para os recipients (em vez de atribuir uma tarefa a eles). Você poderia criar uma tarefa para a &quot;Rodada de roteamento de prova 2&quot; e a &quot;Rodada de roteamento de prova 3&quot;, que pode ajudá-lo a rastrear quantas rodadas ocorreram. Você também poderá acompanhar o progresso das provas usando o Painel de prova (PHQ Login > Painel > Provas para gerenciar). Essa visualização indicará o número de provas atrasadas (bem como provas de risco) que você está gerenciando.

**Pergunta**

Quando uma prova é excluída, uma cópia dessa prova ainda está nos servidores?

**Resposta**

Sim. Se você excluir uma prova de que ela reside na área Lixeira da Conta de prova associada, ela poderá ser restaurada se necessário e permanecerá lá até e a menos que a lixeira seja esvaziada.

**Pergunta**

Há uma maneira de acionar uma nova decisão se outro usuário rejeitar ou aprovar com alterações. i.e. O departamento de provas vê algo, o gerente de projeto terá que tomar uma nova decisão... mesmo que já tenha olhado para ele e aprovado. (tentando não fazer com que o gerente de projeto não tenha que esperar no departamento de revisão para fazer sua revisão)?

**Resposta**

Embora isso não possa ser automatizado, você pode definir o Gerenciador de projetos com o Alerta por email de decisões. Assim, quando o departamento de revisão tomar a decisão, o Gerente de projetos será notificado da decisão tomada e poderá voltar para a prova, revisar os comentários feitos pelo departamento de revisão e alterar a decisão, se necessário.

**Pergunta**

Por que, quando marco a opção &quot;Solicitar aprovação&quot;, quando envio uma atualização na seção de detalhes Prova, vejo somente o status SOC, e não SOCD. Devemos evitar usar essa caixa de seleção? Qual é a prática recomendada para enviar uma atualização em uma prova.

**Resposta**

Ao usar a função &quot;Solicitar aprovação&quot;, você está trabalhando com a funcionalidade Aprovação de documento, que será independente da Prova e da Barra de progresso SOCD. Se precisar atualizar a função de prova de um recipient, o que desejará fazer é seguir este caminho: Na guia Documentos, selecione a prova > e clique em Detalhes da prova. Quando a janela de detalhes da prova for aberta, você verá a lista de recipients e a opção de função de prova (bem como Alerta por email) poderá ser ajustada na linha. Isso permitiria (por exemplo) alterar a função de prova de Revisor para Revisor e Aprovador.

**Pergunta**

É possível garantir que os aprovadores finais não tenham acesso às versões anteriores (e comentários) se houver no mesmo documento de prova? Um novo documento de prova precisa ser criado ou há uma maneira de manter todas as versões e comentários em um e designar o acesso às versões?

**Resposta**

Nas Configurações da conta dentro da prova, é possível controlar o acesso de compartilhamento/visibilidade às provas. Para atualizar essa configuração para que os recipients de prova vejam apenas as versões das provas que você designar (em vez de ver todas as versões da prova), siga este caminho: PHQ Login > Account Settings > Settings > Sharing > Recipients pode visualizar todas as versões = Disabled.

**Pergunta**

É possível adicionar a tela do painel de prova como uma página externa a um painel WF? Os não administradores verão o painel?

**Resposta**

É possível adicionar o Painel de prova como uma página externa em um Painel. Observe que isso só seria visível por usuários com uma licença de prova.

**Pergunta**

Os recursos de Painel e Relatórios no ProofHQ só estão disponíveis para administradores que têm acesso ao Proof, certo? Não são Planejadores gerais que não têm acesso de administrador?

**Resposta**

Isso está correto. Embora, você possa enviar um caso de suporte com o Workfront para solicitar que todos os usuários da Licença de revisão tenham acesso ao sistema de prova.

**Pergunta**

Olá, uma pergunta sobre a flexibilidade de propriedade da prova: se um novo upload de versão de prova for necessário na ausência do proprietário original, a prática recomendada é que eles adicionem um colega ao fluxo de trabalho como um Autor e decidam &quot;Não relevante&quot;? (Delegar a propriedade parece funcionar somente para uma única versão).

**Resposta**

Esse caso de uso e fluxo de trabalho funcionariam perfeitamente. Outra coisa que você pode considerar, no entanto, é ter usuários que talvez precisem fazer upload de novas versões para provas de que não são os proprietários configurados com o Nível de Permissão de Prova de Supervisor ou Administrador. Esse nível de permissão permitirá que eles façam upload de novas versões para provas de que não são os proprietários do, sem precisar adicioná-las à prova como Autor ou Moderador (o que exigiria uma decisão).

**Pergunta**

Pelo que entendo, você não pode adicionar o mesmo usuário em estágios subsequentes em um fluxo de trabalho automatizado, e isso é problemático para nós. Isso é algo que você pode alterar para permitir que o mesmo usuário esteja em vários estágios?

**Resposta**

Embora não seja possível adicionar um recipient de prova a mais de um estágio da revisão em uma prova, uma vez que o estágio da revisão em que estão esteja esteja ativado, ele estará na prova pelos estágios restantes dessa versão. Isso permitiria que eles continuassem a comentar e responder a comentários mesmo que outras etapas tenham começado. A chave para garantir que isso funcione é garantir que você não tenha estágios bloqueados quando novos estágios forem iniciados.

**Pergunta**

Você pode explicar o roteamento de provas entre estágios? Como fechar um e passar para o próximo estágio?

**Resposta**

Há algumas opções disponíveis nos templates de workflow automatizado que permitirão mover de um estágio para o próximo. As opções que podem ser usadas incluem &quot;Criação na prova&quot;, &quot;Quando todas as decisões são aprovadas em um estágio principal&quot;, &quot;Quando todas as decisões são aprovadas ou aprovadas com alterações em um estágio principal&quot;, &quot;Quando todas as decisões são tomadas em um estágio principal&quot;, bem como algumas outras opções.

**Pergunta**

Você pode remover uma prova de um documento que foi gerado automaticamente, mas não queria que fosse uma prova?

**Resposta**

Se a configuração &quot;Gerar provas automaticamente ao carregar documentos&quot; estiver ativada, você não poderá remover uma prova de um documento. Em vez disso, faça upload novamente por meio do botão Adicionar novo > Documentos.

**Pergunta**

Um usuário pode dizer que no estágio 3 do fluxo de prova é possível adicionar outra pessoa como Revisar e aprovar?

**Resposta**

Se esse usuário tiver direitos de Edição na prova que puder. Pessoas com direitos de edição serão: o proprietário da prova, recipients da prova adicionados à prova com a função de prova de autor ou moderador, usuários da licença de prova com o nível de permissão de prova de supervisor ou administrador.

**Pergunta**

Se um usuário for designado como um autor, é possível fazer upload de uma nova versão da prova? Seria alguém diferente do originador da prova.

**Resposta**

Os recipients de prova com a função de prova de Autor e Moderador podem adicionar novas versões às provas em que estão com essa função de prova.

**Pergunta**

Os usuários externos recebem um email por prova para revisão. Isso pode ser desafiador para eles rastrearem o status de todas as provas que eles têm em andamento. Existem opções de painéis, lista de status de email ou recursos futuros para que os usuários externos rastreiem seus status em várias provas?

**Resposta**

Eu recomendaria adicionar esses Usuários externos ao Workfront com uma licença gratuita de Revisor. Isso lhes dará acesso a uma página Minhas atualizações que incluirá uma lista de todas as provas pendentes sobre as quais eles precisam tomar uma decisão.

**Pergunta**

Você pode explicar mais sobre as notificações de Decisões? Receberei apenas notificações com comentários de prova de Revisores e Aprovações ou também receberei os comentários dos Revisores e quando devo recebê-los?

**Resposta**

As notificações de alerta por email de decisão são enviadas somente quando são tomadas decisões na prova. Eles não serão enviados quando forem feitos comentários. No entanto, se você receber um alerta por email de Decisão que indica que um recipient na prova tomou a decisão de Alterações necessárias, você saberá que é um bom momento para revisar os comentários adicionados (que estarão na prova).

**Pergunta**

Em relação ao problema com o encaminhamento de emails, você está realmente fazendo logon como proprietário do email? E isso aconteceria com ambientes bloqueados? Isso aconteceria com um ambiente SSO?

**Resposta**

Isso conectaria você na prova como a pessoa que encaminhou o email para você. Usar o logon necessário nas provas e usar o SSO impedirá que você acesse a prova como a pessoa que encaminhou o email.

**Pergunta**

Onde faço para acessar o painel e os relatórios na prova?

**Resposta**

Se você tiver um ícone de caixa de seleção à direita da barra de pesquisa no Workfront, significa que tem uma conta integrada do Workfront e do Proof. Ao clicar nessa caixa de seleção, você será direcionado ao Workfront Proof e a tela inicial será o painel. Os relatórios podem ser criados usando a opção Exibições no painel esquerdo.

**Pergunta**

Na seção &quot;Função&quot;, há duas marcas de seleção na parte inferior que mencionam estar prestes a adicionar alguém usando um @mention etc. Nas configurações de Prova, é possível definir funções padrão para cada pessoa, mas não há a opção de marcar essas marcas de seleção automaticamente, portanto, é necessário fazer isso sempre que criar uma prova. Como você pode tornar isso padrão para um usuário?

**Resposta**

No momento, não há uma maneira de tornar essa uma configuração padrão para recipients de prova. No entanto, é possível salvá-las como configurações padrão para destinatários em Modelos de fluxo de trabalho automatizados.

**Pergunta**

Como trocar um proprietário de prova?

**Resposta**

Para alternar o proprietário de uma prova, siga este caminho: na guia Documentos, selecione a prova e clique em &quot;Detalhes da prova&quot;. A guia de detalhes da prova será aberta. Se a pessoa que você deseja tornar o proprietário da prova ainda não estiver na prova, adicione-a como um recipient clicando no botão Elipses e selecionando Compartilhar. Depois que a pessoa for adicionada à prova (ou se já estiver na prova), você selecionará o botão de Elipses correspondente para selecionar &quot;Tornar proprietário&quot;. Eles agora serão o proprietário da prova.

**Pergunta**

Em termos de novas versões de provas... a única maneira que entendo de fazer isso é arrastar e soltar o arquivo sobre o arquivo existente. Esta é a maneira correta de fazer isso?

**Resposta**

Eu recomendaria criar novas versões dessa maneira: selecione a prova na guia Documentos e clique no botão Mais, escolha Nova versão > Prova. Isso o levará à página Nova versão, que transportará o workflow e permitirá fazer os ajustes necessários antes de rotear a nova versão.

**Pergunta**

Você pode desativar comentários sobre provas para compartilhar com um cliente para que ele não veja todo o feedback interno da equipe? Para que não seja necessário gerar novamente uma nova prova.

**Resposta**

Eu recomendaria usar Modelos de fluxo de trabalho automatizados que permitirão utilizar &quot;Estágios privados&quot;. Estágios privados permitem ocultar comentários, marcações e decisões de Revisores convidados em outros estágios. Isso permitiria que a Revisão de prova interna ficasse completamente oculta do solicitante externo.

**Pergunta**

O estágio de Prova do Workfront é adicionado somente quando os Fluxos de trabalho automatizados são usados e alguém não adicionado ao fluxo de trabalho abre a prova?

**Resposta**

O estágio &quot;Workfront Proof&quot; será adicionado às provas se um usuário que não seja recipient clicar na prova. Ele também será aplicado se alguém converter uma Prova de fluxo de trabalho básica em uma Prova automatizada do Workfront.

**Pergunta**

Temos a capacidade de configurar um fluxo de trabalho de prova em que mais de uma decisão pode ser tomada?

Estamos tentando fornecer relatórios à nossa equipe jurídica interna sobre quando o serviço jurídico externo concluiu as revisões das provas (quantos dias, em média, são necessários para concluir a revisão, quem a conclui etc.)

Começamos adicionando uma nova decisão ao fluxo de trabalho de prova chamada &quot;Análise do OC concluída&quot; e imaginamos que poderíamos criar um relatório para rastreá-los.

O problema é que parece que somente uma decisão pode ser tomada no workflow.

**Resposta**

Mais de uma decisão pode ser tomada em relação a uma prova - no entanto, haverá apenas um status geral em uma prova que virá da decisão do pior cenário sobre a prova - ou a decisão tomada por um Tomador de decisão principal.

Devido aos seus requisitos de relatórios, o que eu recomendaria é que todos na prova usem as mesmas opções de decisão (Aprovado, Aprovado com alterações, Alterações necessárias) e, em seguida, usem os Relatórios no Painel de prova (Logon PHQ > Relatórios) e apliquem a opção de filtro para filtrar por recipients (incluir os recipients de consultoria jurídica externos no filtro), você poderá ver o tempo médio de inversão em suas provas.

**Pergunta**

Depois que uma nova versão é arrastada e solta em uma prova existente, por que TODAS as funções mudam ou desaparecem especificamente?

**Resposta**

Ao arrastar e soltar um documento como uma nova versão, você está certo de que o fluxo de trabalho será removido da nova versão. Se quiser reter o fluxo de trabalho da versão anterior para a próxima versão, selecione a prova na guia Documentos e clique no botão Mais, escolha Nova versão > Prova. Isso o levará à página Nova versão, que transportará o workflow e permitirá fazer os ajustes necessários antes de rotear a nova versão.

**Pergunta**

Cenário - Encaminhamento de provas: um cliente externo que revisa uma prova pode querer circular internamente em sua organização antes de aprovar nossa prova. As outras que revisam não estarão necessariamente no sistema, portanto, não parece que @ nos comentários funcionasse. Como eles devem compartilhar melhor - encaminhar o email e destacar para o recipient que nenhum comentário não seria exibido como seu nome?

**Resposta**

Você gostaria de usar a funcionalidade Assinaturas de prova. Isso pode ser ativado nas configurações da prova e permite que os recipients na prova encaminhem um link público genérico para a prova e, em seguida, permitam que as pessoas assinem a prova (essencialmente adicionando a si mesmas).

**Pergunta**

Qual é a prática recomendada para usar as pastas nos documentos?

**Resposta**

Isso dependerá da natureza do projeto, mas algo que você pode considerar é uma Pasta de provas ativa que contém todas as provas/versões que estão sendo encaminhadas ativamente e uma Pasta de provas aprovadas que contém todas as provas que estão finalizadas e aprovadas. Depois que uma prova é totalmente aprovada, você a move da Pasta Provas ativas para a Pasta Provas aprovadas.

**Pergunta**

Se eu tiver 3 pessoas em um grupo de avaliações, posso definir que preciso de aprovações de 2 delas de 3?

**Resposta**

Sim. Você desejará adicionar as duas pessoas das quais precisa uma decisão como Revisores e Aprovadores e a terceira pessoa como Revisor.

**Pergunta**

Gostaríamos de enviar uma prova para um cliente externo (usuário que não seja da Workfront) para analisar e comentar. Queremos enviar a eles uma prova simples (em outras palavras, uma prova sem comentários internos). Quais são as etapas corretas para fazer isso acontecer para garantir que o cliente externo receba a prova (apenas a prova, sem acesso ao próprio projeto) e como os clientes externos nos &quot;enviam&quot; de volta sua prova marcada? Atualmente, não usamos modelos de prova/fluxos de trabalho automatizados.

**Resposta**

Eu recomendaria usar o fluxo de trabalho automatizado / templates de fluxo de trabalho automatizado para isso, pois permitirá usar a funcionalidade &quot;Estágio privado&quot;. Ao usar a funcionalidade Estágio privado, é possível fazer com que os comentários/decisões e os recipients de determinados estágios de revisão permaneçam ocultos das pessoas em outros estágios. Como exemplo, você pode ter um Estágio interno como um Estágio privado e um Estágio do cliente. Os Clientes não poderão ver nada a ver com o Estágio interno enquanto você puder ver a atividade no Estágio do cliente.

**Pergunta**

É possível manter usuários específicos (também conhecido como proofreader) em um estágio inicial sem que eles sejam repetidos em estágios posteriores?

**Resposta**

Depois que alguém é adicionado a uma versão de uma prova em um estágio, ele permanecerá nessa versão da prova pelos estágios restantes. Você tem a opção de bloquear o estágio deles quando o próximo estágio começar (ou manualmente), o que impedirá que eles possam fazer mais comentários.

**Pergunta**

Onde podemos visualizar uma lista de todos que revisaram e/ou aprovaram uma prova, em que dia e a que horas? Para fins de auditoria, etc. Também há um local em que possamos ver todas as revisões e aprovações de todas as versões de uma prova?

**Resposta**

Para ver uma lista de atividades, como quando os comentários e as decisões foram feitos, é necessário clicar no Histórico de atividades na tela Detalhes da prova. Para acessar, siga este caminho: selecione a prova na guia Documentos > Clique em Detalhes da prova > Expanda a seção Atividade. Se quiser ver essas informações no nível da versão, siga este caminho: Selecione a Prova na guia Documentos > Clique na guia Detalhes > Na parte inferior da tela, você verá uma seção Versões. Aqui, você pode acessar os detalhes da prova no nível da versão.

**Pergunta**

Você pode falar um pouco sobre etapas privadas em provas.

**Resposta**

Quando um estágio é tornado privado, os comentários e as decisões não ficam visíveis para as pessoas que não são adicionadas a esse estágio ou que não são Supervisores, Administradores ou Administradores de Faturamento na conta. Além disso, os revisores adicionados a um estágio privado podem ver somente o estágio ao qual são adicionados na prova e nos comentários feitos nesse estágio.
