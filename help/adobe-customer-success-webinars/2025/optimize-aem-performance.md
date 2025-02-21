---
title: Otimização do desempenho do AEM - Estratégias e técnicas de armazenamento em cache
description: A sessão abordou estratégias e técnicas de armazenamento em cache, mecanismos e camadas de armazenamento em cache, tratamento de conteúdo dinâmico, depuração de problemas de armazenamento em cache e sincronização da invalidação de cache entre o Dispatcher e o CDN.
topic: Performance
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3764
last-substantial-update: 2025-02-21T00:00:00Z
jira: KT-17373
source-git-commit: e7bf8b79ad4920b303fc3afbdfb4adee60614c88
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 0%

---


# Otimização do desempenho do AEM: estratégias e técnicas de armazenamento em cache

Nesta sessão, exploramos vários mecanismos de armazenamento em cache — como armazenamento em cache de página, ativo e dispatcher — e também como implementar o armazenamento em cache no nível de CDN para otimizar a entrega de conteúdo e reduzir os tempos de carregamento. A discussão abordará as práticas recomendadas para cada camada de armazenamento em cache, a solução de problemas comuns e como aproveitar os recursos de CDN para obter o máximo de eficiência.

## Pontos principais de discussão

* Introdução ao cache
* Tipos de armazenamento em cache, práticas recomendadas de armazenamento em cache, invalidação e atualização de cache
* Técnicas de depuração

>[!VIDEO](https://video.tv.adobe.com/v/3444452/?learn=on&enablevpops)

## Principais pontos

* **Estratégias e técnicas de armazenamento em cache** A sessão focou várias estratégias e técnicas de armazenamento em cache para otimizar o desempenho, incluindo armazenamento em cache em diferentes camadas, como navegador, CDN e dispatcher.

* **Mecanismos e camadas de armazenamento em cache** A discussão abordou diferentes mecanismos e camadas de armazenamento em cache, incluindo armazenamento em cache do navegador, armazenamento em cache do CDN e armazenamento em cache do dispatcher, e como eles podem ser configurados e gerenciados.

* **Manipulação de conteúdo dinâmico** As técnicas de manipulação de conteúdo dinâmico em uma página foram discutidas, incluindo o uso de Sling Dynamic Include (SDI) e Edge Side Includes (ESI) para garantir que o conteúdo dinâmico não seja armazenado em cache enquanto o conteúdo estático estiver sendo armazenado.

* **Depuração de problemas de cache** Foram explicadas várias técnicas para depurar problemas de cache em diferentes níveis (navegador, CDN, dispatcher), incluindo o uso de cabeçalhos, logs e configurações específicas para identificar e resolver problemas de cache.

* **Sincronização da Invalidação de Cache** A sessão abordou o desafio de sincronizar a invalidação do cache entre o Dispatcher e o CDN, recomendando o uso de valores max-age mais curtos e APIs de limpeza do CDN para garantir que ambos os caches sejam invalidados simultaneamente após a ativação da página.