---
title: Configurações do Dispatcher no Adobe Experience Manager as a Cloud Service
description: Explore as práticas recomendadas do AEM Dispatcher para armazenamento em cache, segurança e desempenho para maximizar a escalabilidade e a eficiência do AEM as a Cloud Service.
solution: Experience Manager as a Cloud Service
version: Experience Manager as a Cloud Service
feature: Dispatcher
role: Developer, Leader, User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 4200
last-substantial-update: 2025-05-07T00:00:00Z
jira: KT-17903
source-git-commit: cfc7b54ae4360779ca2c41f88fc08089bae99165
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---


# Sessões técnicas: configurações do Dispatcher no Adobe Experience Manager as a Cloud Service

O **Adobe Experience Manager (AEM) as a Cloud Service** oferece escalabilidade, flexibilidade e melhor desempenho para plataformas de experiência digital modernas. No coração dessa arquitetura está a **AEM Dispatcher**, um componente vital responsável pelo armazenamento em cache, segurança e gerenciamento de solicitações. Quando configurado corretamente, o Dispatcher acelera a entrega de conteúdo, protege sistemas de back-end e melhora o desempenho geral do site.

Esta visão geral destaca as principais configurações do Dispatcher, incluindo estratégias de armazenamento em cache, mecanismos de controle de acesso e filtragem de solicitações. Ele também descreve as práticas recomendadas para manter uma implantação segura e de alto desempenho do AEM na nuvem. Seja você um desenvolvedor, um arquiteto ou um tomador de decisão de negócios, uma sólida compreensão das configurações do Dispatcher é fundamental para explorar todo o potencial do AEM as a Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/3457891/?learn=on&enablevpops)

## Principais aprendizados

* **Dispatcher SDK para validação** O AEM Dispatcher SDK é uma ferramenta poderosa para análise estática de configurações. Ele permite a validação rápida de configurações, verifica a imutabilidade e identifica erros, economizando tempo significativo em comparação às implantações completas de pipeline.

* **Ambiente de desenvolvimento rápido (RDE)** O RDE fornece um ambiente de tempo de execução interativo para configurações de teste e depuração além da análise estática. Ele permite validação e depuração mais rápidas, reduzindo o tempo necessário para implantação e teste.

* **Rede Avançada com Proxy Mod** Configurações avançadas de rede, como VPN e IPs de saída dedicados, podem ser configuradas usando o Cloud Manager. O módulo proxy mod permite o descarregamento de transações do AEM para serviços externos, otimizando o desempenho e reduzindo a carga na JVM.

* **As práticas recomendadas para as configurações do Dispatcher** incluem o uso de caminhos relativos, cabeçalhos x-vhost exclusivos, cabeçalhos de cliente adequados e o uso de cabeçalhos de controle de cache para gerenciar o armazenamento em cache com eficiência. Essas práticas ajudam a evitar falhas de pipeline e melhorar a eficiência de depuração.

* **Pipeline de Camada da Web para Implantação** O pipeline de camada da Web é um utilitário para implantar configurações isoladas de dispatcher. Ele inclui testes adicionais, como invalidação de cache, garantindo que as atualizações de conteúdo sejam refletidas de forma rápida e precisa nos ambientes de produção.