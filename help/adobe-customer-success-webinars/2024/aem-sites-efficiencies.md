---
title: Eficiência da AEM Sites - otimização de desempenho, configuração e solução de problemas
description: fundamentos para a solução de problemas do Adobe Experience Manager (AEM) Sites. Quer você esteja enfrentando problemas de desempenho ou lidando com configurações complexas, esta sessão fornecerá habilidades práticas para manter e otimizar seu ambiente AEM. Priorizaremos demonstrações ao vivo em vez de slides, oferecendo experiência prática para enfrentar desafios do mundo real​Principais pontos para discussão:- Configuração de host virtual e mapeamento de domínio- Problemas de desempenho- Autorização, identificação, permissões de usuário
solution: Experience Manager
version: Cloud Service
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3452
last-substantial-update: 2024-10-30T00:00:00Z
jira: KT-16353
source-git-commit: 3f245f71cd4db5097b5a9e712114112451d899e4
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---


# Eficiência da AEM Sites: otimização de desempenho, configuração e solução de problemas

Neste webinário, analisaremos os fundamentos para solucionar problemas dos sites do Adobe Experience Manager (AEM). Quer você esteja enfrentando problemas de desempenho ou lidando com configurações complexas, esta sessão fornecerá habilidades práticas para manter e otimizar seu ambiente AEM. Priorizaremos demonstrações ao vivo em vez de slides, oferecendo experiência prática para enfrentar desafios do mundo real&#x200B;

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