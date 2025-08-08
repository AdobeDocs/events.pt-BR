---
title: Marketo & Mochas - Sincronização com o Salesforce
description: Domine a sincronização Marketo-Salesforce com a orientação de especialistas sobre permissões, visibilidade de campo, colaboração de administradores e práticas recomendadas para garantir uma integração perfeita e otimizada.
feature: Salesforce Integration
topic: Integrations
role: Admin, Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 3547
last-substantial-update: 2025-08-07T00:00:00Z
jira: KT-18706
source-git-commit: bc5752512fb1bc50cefe0180c308574e821888a2
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# Marketo &amp; Mochas: sincronização com o Salesforce

O Marketo tem poucas integrações nativas, mas o Salesforce é o mais eficiente de todas. Com cerca de 90% dos clientes do Marketo também utilizando o Salesforce, a Adobe tem o compromisso de orientar os clientes sobre como teorizar, diagnosticar e otimizar a sincronização entre os dois. A sincronização do Marketo com o SFDC é baseada principalmente nas permissões no SFDC fornecidas ao usuário de sincronização do Marketo. Isso pode ser difícil para os clientes devido a vários administradores ou equipes diferentes que criam silos de comunicação em torno de atualizações no sistema.

Esse webinário aborda os itens a seguir, relacionados à sincronização do Marketo &lt;-> SFDC:

· Explicar a visão geral de como a sincronização funciona
· Ocultar campos e objetos do usuário do Marketo Sync no SFDC
· Como se comunicar com o administrador do SFDC
· Como trabalhar de forma eficiente com o suporte da Marketo
· O que evitar ao sincronizar o Marketo com o SFDC

>[!VIDEO](https://video.tv.adobe.com/v/3470624/?learn=on&enablevpops)

## Práticas recomendadas para usar o Salesforce Sync

Para usar o Salesforce Sync com o Marketo de maneira eficaz, siga estas práticas recomendadas, explicadas passo a passo em termos simples:

1. **Entender o Processo de Sincronização**

   A sincronização conecta o Marketo e o Salesforce, permitindo que os dados fluam entre os dois sistemas. Pense no &quot;Usuário de sincronização do Marketo&quot; como uma ponte entre as duas plataformas. Este usuário tem permissão para ler e gravar determinados dados:

   * **Clientes potenciais e contatos do Write Access** (a Marketo pode atualizá-los no Salesforce).
   * **Acesso de Leitura** Contas, oportunidades, objetos personalizados e atividades (a Marketo pode visualizá-los, mas não pode alterá-los).

   Quando os dados são alterados no Salesforce ou no Marketo, a sincronização atualiza o outro sistema a cada cinco minutos. No entanto, você pode priorizar atualizações urgentes usando etapas de fluxo como &quot;Sincronizar com o SFDC&quot;.

1. **Limpar Campos**

   Sincronizar apenas os campos usados ativamente. Por exemplo:

   * Se você tiver campos antigos como &quot;Notas da COVID-19&quot; que não são mais relevantes, remova-os da sincronização. Isso reduz a desordem e acelera o processo.
   * Evite sincronizar campos de fórmula (por exemplo, &quot;prazo de entrega em dias&quot;) porque eles não atualizam carimbos de data e hora, o que pode causar problemas.

1. **Impedir Backlogs**

   Uma lista de pendências acontece quando muitos dados estão aguardando sincronização. Para evitar isso:

   * Limitar atualizações desnecessárias: por exemplo, se uma pontuação de conta for ligeiramente alterada (por exemplo, de 60 para 61), ela poderá acionar atualizações para todos os contatos relacionados. Em vez disso, agrupe as pontuações em intervalos (por exemplo, 0-25, 26-50) para reduzir as atualizações.
   * Campanhas em lote: use campanhas em lote em vez de campanhas de acionador para processar dados com mais eficiência.

1. **Gerenciar erros**

   Podem ocorrer erros quando o Marketo tenta atualizar um campo no Salesforce, mas não tem permissão. Para solucionar problemas:

   * Faça logon no Salesforce como o Usuário de sincronização do Marketo e tente executar a mesma ação. Isso ajuda a identificar problemas de permissão ou dados inválidos.
   * Configure campanhas recorrentes no Marketo para corrigir erros comuns, como padronizar valores de país/estado (por exemplo, &quot;CA&quot; para &quot;Califórnia&quot;).

1. **Usar Filtros De Sincronização Personalizados**

   Filtros personalizados ajudam você a controlar quais registros são sincronizados entre o Salesforce e o Marketo. Por exemplo, crie um campo chamado &quot;Não sincronizar com o Marketo&quot;. Se esse campo estiver marcado como &quot;true&quot; para um registro, ele não será sincronizado com o Marketo. Isso é útil para excluir endereços de email inválidos ou contatos desatualizados.

1. **Limitar criação de tarefa**

   Salesforce. Concentre-se em atividades relevantes, como &quot;formulário preenchido&quot; ou &quot;link clicado no email&quot;.

1. **Colaborar com o administrador do Salesforce**

   Como a sincronização envolve ambos os sistemas, trabalhe em conjunto com o administrador do Salesforce para:

   * Gerenciar permissões para o usuário do Marketo Sync.
   * Limpe campos desnecessários no Salesforce.
   * Solucionar problemas de sincronização juntos.

1. **Monitorar Desempenho de Sincronização**

   Verifique regularmente o status de sincronização na seção de administrador do Marketo:

   Procure picos nos painéis &quot;Tendência de backlog de sincronização&quot; ou &quot;Throughput de sincronização&quot;. Isso indica atrasos ou atualizações excessivas.
Se você notar problemas, investigue quais campos ou registros estão causando o problema.

1. **Usar Objetos Personalizados De Forma Inteligente**

   Os objetos personalizados são estruturas de dados especiais que podem armazenar informações adicionais (por exemplo, detalhes do produto). Sincronize somente objetos personalizados necessários para suas campanhas a fim de evitar sobrecarga do banco de dados.

1. **Plano de escalabilidade**

   Ao configurar a sincronização, pense em longo prazo:

   * Mantenha um dicionário de dados para rastrear quais campos são sincronizados e o porquê.
   * Evite sincronizar campos ou registros desnecessários para manter o sistema eficiente.

Ao seguir essas etapas, você pode garantir uma integração perfeita e eficiente entre o Marketo e o Salesforce, minimizando erros e maximizando o valor dos seus dados.
