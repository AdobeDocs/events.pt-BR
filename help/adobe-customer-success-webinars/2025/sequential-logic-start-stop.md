---
title: Dominar a lógica sequencial no Adobe Analytics e no Customer Journey Analytics - inicializações e interrupções
description: Domine a lógica sequencial no Adobe Analytics com segmentação avançada, controles de escopo e campos derivados para descobrir padrões de comportamento do cliente e melhorar a precisão dos dados.
solution: Analytics, Customer Journey Analytics
role: Developer
level: Intermediate
doc-type: Event
duration: 3370
last-substantial-update: 2025-05-08T00:00:00Z
jira: KT-18017
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---


# Dominar a lógica sequencial no Adobe Analytics e no Customer Journey Analytics: inicializações e interrupções

Nesta sessão, exploraremos como configurar sequências com o operador THEN no Adobe Analytics (AA) e no Customer Journey Analytics (CJA). Saiba como recuperar subconjuntos precisos de atividade combinando APENAS DEPOIS/APENAS ANTES DA SEQUÊNCIA com pontos de verificação EXCLUIR.

## Pontos de discussão

* Revisão rápida de operadores lógicos sequenciais independentes e estrutura visual.
* Descreva como EXCLUIR afeta os resultados de sequências que usam SOMENTE SEQUÊNCIA DEPOIS/ANTES.
* Apresentar casos de uso e demonstrações mostrando como você pode adotar os métodos para sua empresa.

>[!VIDEO](https://video.tv.adobe.com/v/3458040/?learn=on&enablevpops)

## Destaques


1. Lógica sequencial e segmentação no Analytics

   * A sessão se concentrou em técnicas avançadas de aplicação da lógica sequencial no Analytics, enfatizando a importância de entender os pontos de partida e de parada nas sequências de dados para analisar os comportamentos do cliente de maneira eficaz.
   * Os operadores sequenciais foram discutidos como ferramentas para identificar padrões como &quot;ocorrência na web seguida de ocorrência por email&quot; ou &quot;envio de aplicativo seguido de sessões subsequentes&quot;.
   * A natureza gananciosa da lógica de segmento foi destacada, explicando como ela retorna o maior conjunto de dados possível, a menos que seja restringida por condições adicionais.
   * Técnicas para definir o escopo, como as sequências &quot;somente antes&quot; e &quot;somente depois&quot;, foram introduzidas para estudar subconjuntos de dados com base em questões comerciais específicas.
   * O uso de pontos de verificação, condições de proximidade e critérios de exclusão foi explicado para refinar a análise de dados e responder a perguntas comerciais complexas.

2. Como lidar com vários pontos de interesse na análise de dados

   * Andy discutiu cenários em que os clientes têm vários envios de aplicativos e a necessidade de analisar comportamentos após cada envio, em vez de apenas o primeiro.
   * Foram solucionados desafios como a sobreposição de pedidos e a definição da inclusão ou exclusão de pontos de interesse originais.
   * Foi enfatizada a importância de esclarecer suposições e refinar a lógica para lidar com várias ocorrências de uma sequência, garantindo uma análise precisa dos comportamentos do cliente em todo o ciclo de vida.

3. Técnicas avançadas para interromper a correspondência de dados

   * A sessão introduziu métodos para interromper a correspondência de dados em pontos de verificação específicos usando critérios de exclusão, permitindo que os analistas estudem os dados entre os pontos inicial e final definidos.
   * Os exemplos incluíam analisar comportamentos entre &quot;ocorrência da web seguida de interação com o aplicativo móvel&quot; e parar em &quot;interação com email&quot;.
   * O uso das condições &quot;dentro&quot; e &quot;depois&quot; foi explicado para impor regras de proximidade mais rigorosas e evitar resultados não intencionais da lógica gananciosa.
   * Andy demonstrou como essas técnicas podem ser aplicadas para estudar os comportamentos dos clientes em relação a eventos específicos, como envios de aplicativos.

4. Validação e Refinamento da Lógica da Análise de Dados

   * Andy enfatizou a importância de validar as suposições e a lógica de testes para garantir resultados precisos, já que os erros na criação de segmentos ou nas suposições de dados são comuns.
   * Exemplos de resultados inesperados devido à lógica gananciosa foram compartilhados, destacando a necessidade de condições estritas como &quot;dentro de um evento&quot; ou &quot;dentro de uma sessão&quot;.
   * Foram recomendados parâmetros de validação, como pequenos conjuntos de dados com características conhecidas, para testar e refinar métodos de análise.

5. Aplicação da lógica sequencial a casos de uso reais

   * Andy forneceu exemplos de casos de uso reais, como analisar comportamentos do cliente após envios de aplicativos ou identificar ações comuns após compras ou revisões negativas.
   * A sessão demonstrou como a lógica sequencial pode ser aplicada a padrões de estudo como &quot;primeira sessão após a aplicação&quot; ou &quot;segunda sessão após a aplicação&quot; em várias ocorrências.
   * Foi discutida a importância de dimensionar a análise para conjuntos de dados mais amplos, mantendo a precisão, com exemplos de efeitos em cascata em dados de nível de sessão.

6. Uso de campos derivados para análise flexível

   * Andy apresentou o conceito de usar campos derivados no Adobe Customer Journey Analytics (CJA) para definir momentos de interesse dinamicamente, reduzindo a necessidade de editar vários filtros para cada análise.
   * Campos derivados permitem que os analistas criem filtros em relação a um único campo, permitindo ajustes rápidos para estudar diferentes pontos de interesse, como aplicativos específicos de produto ou outros eventos do cliente.

7. Aplicativos práticos e planos futuros

   * Andy compartilhou planos para a próxima sessão de webinário, que se concentrará em modelos, folhas de características e aplicações práticas dos conceitos discutidos, passando do treinamento para casos de uso acionáveis.
   * A sessão foi concluída com uma chamada para feedback por meio de uma pesquisa para determinar o interesse em tópicos futuros e garantir o alinhamento com os objetivos dos participantes.
   * Andy destacou os microengajamentos da equipe do Ultimate Success, oferecendo sessões de treinamento direcionadas para ajudar as empresas a aplicar esses conceitos a seus casos de uso específicos.

8. Compartilhamento de materiais e ações de acompanhamento

   * Andy confirmou que o material do webinário, incluindo gravações e posts em blogs, será compartilhado com os participantes, fornecendo uma forma documentada do conteúdo da sessão.
   * Os participantes foram incentivados a entrar em contato com seus TAMs ou CSMs para obter mais assistência e explorar o licenciamento da Ultimate Success para sessões de treinamento personalizadas.
