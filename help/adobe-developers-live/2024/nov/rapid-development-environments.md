---
title: Ambientes de desenvolvimento rápido da Adobe Experience Manager
description: Facilite o rápido desenvolvimento e a implantação em ambientes de nuvem com o novo SDK da Adobe, reduzindo significativamente o tempo de implantação e oferecendo suporte a atualizações rápidas, registros em tempo real e opções avançadas de configuração, conforme discutido no DevOps Life 2024.
solution: Experience Manager as a Cloud Service, Experience Manager
feature: Developer Tools
topic: Development
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2427
last-substantial-update: 2024-11-27T00:00:00Z
jira: KT-16570
exl-id: 330d8be1-14a0-488a-aae0-ee90e1f7621e
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# Ambientes de desenvolvimento rápido da Adobe Experience Manager

Explore as práticas recomendadas para os ambientes de desenvolvimento rápido (RDEs) e o console do desenvolvedor atualizado. Natalia Angulo Herrera, engenheira de desenvolvimento de software da Adobe, e Remo Liechtenstein, engenheiro de desenvolvimento de software da Adobe, abordam desafios de migração, configuração, implantação, teste, registro e gerenciamento de configuração da CLI AIO para um fluxo de trabalho de Adobe Experience Manager mais suave.

>[!VIDEO](https://video.tv.adobe.com/v/3440397/?learn=on&enablevpops)


## Discussão da comunidade

Continue a conversa na [discussão](https://adobe.ly/3UJluDo) da Comunidade do Adobe Developers Live.

## Principais pontos

* **Introdução ao DevOps Life 2024** A sessão é hospedada por Natalia e Remo da Adobe, com foco em ambientes de desenvolvimento rápido.
* **Declaração de problemas** O desafio de ambientes de desenvolvimento locais funcionarem bem localmente, mas falharem ao serem implantados na nuvem.
* **Solução** Criação de uma nova SDK na nuvem para facilitar o desenvolvimento e a implantação rápidos, reduzindo o tempo de 30 minutos para segundos ou alguns minutos.
* **Processo de implantação** O novo ambiente permite atualizações e validações rápidas por meio de um novo plug-in de API e CLI, permitindo feedback e implantação mais rápidos.
* **Diferenças de Infraestrutura** O ambiente de nuvem usa uma única instância de autor e publicação sem alta disponibilidade e não usa MongoDB.
* **Instalação e uso** Os desenvolvedores podem configurar um ambiente de desenvolvimento rápido por meio da interface de nuvem, usando npm e Adobe IO CLI para instalação e configuração.
* **Comandos Básicos** Os comandos principais incluem io amd —help, io login, io status, io install, io history, io delete e io reset.
* **Logs e depuração** O novo ambiente oferece suporte a logs dinâmicos e à alteração dos níveis de log sem reimplantação, usando comandos como logs io am ou d.
* **Tópicos avançados** Suporte para pacotes front-end e pipelines de configuração, permitindo implantação e iteração rápidas.
* **Recursos futuros** planeja introduzir a funcionalidade de instantâneo para facilitar as redefinições do ambiente e as atualizações automáticas sem perda de conteúdo.
* **Perguntas e respostas e comentários** a sessão incentiva os participantes a ingressarem no canal Discord para uma interação ao vivo e feedback com a equipe de desenvolvimento.
