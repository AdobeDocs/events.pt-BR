---
title: Eficiência da AEM Sites - otimização de desempenho, configuração e solução de problemas
description: O webinário sobre eficiência do site de AMP abordou otimização de desempenho, configuração do dispatcher, práticas recomendadas de gerenciamento de direitos e estratégias para resolver problemas de desempenho.
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
exl-id: 55f7c1d8-7c2c-4392-894a-2aa9b3cc0e4a
source-git-commit: 32060a6a0d2cc24b8dc09c8f5e9f9d9c679e6d3e
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Eficiência da AEM Sites: otimização de desempenho, configuração e solução de problemas

Neste webinário, analisaremos os fundamentos para a solução de problemas do Adobe Experience Manager (AEM) Sites. Esteja você enfrentando problemas de desempenho ou lidando com configurações complexas, esta sessão fornecerá habilidades práticas para manter e otimizar seu ambiente do AEM. Priorizaremos demonstrações ao vivo em vez de slides, oferecendo experiência prática para enfrentar desafios do mundo real&#x200B;

>[!VIDEO](https://video.tv.adobe.com/v/3435114/?learn=on)

## Pontos principais

O webinário se concentrou na eficiência do site de AMP, incluindo otimização de desempenho, configuração e solução de problemas.

### Configuração do Dispatcher

* Importância do dispatcher no delivery de sites com desempenho.
* Aspectos principais da configuração do dispatcher: configuração do host virtual, mapeamento de domínio com estrutura de cache e relatórios e redirecionamentos regulares.

### Rights Management

* Práticas recomendadas: aplique direitos a grupos, evite declarações de negação e evite a engenharia excessiva.
* Uso da ferramenta Netcentric ACL para gerenciar direitos por meio de um arquivo Yaml, garantindo fácil implantação e rastreabilidade.

### Problemas de desempenho

* Importância de identificar deltas em operações de sincronização para evitar liberações totais de cache.
* Evite operações de página grande durante o horário comercial.
* Simplifique os fluxos de trabalho de acordo com as etapas necessárias.
* Tenha cuidado com processos de sistemas de terceiros em sistemas de criação, especialmente com ferramentas como o ImageMagick.
* Evite solicitações sincronizadas para sistemas de terceiros que não podem lidar com a carga.
* Gerencie componentes personalizados pesados para evitar a degradação do desempenho.
* Monitore sessões de longa duração para evitar exceções de segmentos não encontrados.
