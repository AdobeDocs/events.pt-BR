---
title: Configuração de CDN e WAF no Adobe Experience Manager as a Cloud Service
description: Melhore o desempenho e a segurança dos aplicativos do Adobe Experience Manager as a Cloud Service com regras de CDN personalizáveis, proteção do WAF e o Pipeline de configuração, conforme compartilhado pelos especialistas da Adobe.
solution: Experience Manager as a Cloud Service
feature: Security
topic: Performance, Security
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 2211
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16574
exl-id: a9f38e79-c707-443d-8b2f-e534ce4dd43d
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 0%

---

# Configuração de CDN e WAF no Adobe Experience Manager as a Cloud Service

Libere todo o potencial da CDN gerenciada pela Adobe com regras de CDN personalizáveis, proteção da WAF e o pipeline de configuração. Marius Petria, cientista da computação sênior da Adobe, Quentin Vecchio, engenheiro de desenvolvimento de software da Adobe, e Florian Froese, engenheiro de desenvolvimento de software da Adobe, compartilham estratégias para melhorar o desempenho e a segurança dos aplicativos da Adobe Experience Manager as a Cloud Service.

>[!VIDEO](https://video.tv.adobe.com/v/3440607/?learn=on&enablevpops&captions=por_br)

## Discussão da comunidade

Continue a conversa na [discussão](https://adobe.ly/3O0TyYa) da Comunidade do Adobe Developers Live.

## Pontos principais

* **Introdução a Novos Recursos de Configuração** A apresentação apresenta novos recursos de configuração para a CDN em um serviço na nuvem, com foco na capacidade de configurar a CDN para vários casos de uso.
* **Opções de Configuração da CDN** As novas opções permitem a interação com solicitações e respostas HTTP, como adicionar/remover cabeçalhos, regravar caminhos de solicitação, bloquear tráfego, redirecionar clientes e usar proxy para origens diferentes.
* **Aprimoramentos de segurança** Os novos recursos incluem regras de filtro de tráfego para bloquear ou registrar tráfego com base em padrões de solicitação e a introdução do M WAF para proteção avançada contra ataques da Web, como injeção de SQL e XSS.
* **Configuração Declarativa** A configuração é feita usando arquivos YAML e implantada por meio de um pipeline de configuração no Cloud Manager, tornando-o um processo rápido e direto.
* **Transformações de Solicitação e Resposta** Os novos recursos permitem transformações de solicitação para normalizar URLs e remover parâmetros de consulta desnecessários, além de transformações de resposta para definir cabeçalhos antes de enviar respostas aos clientes.
* **Filtros de Tráfego e Limitação de Taxa** Os filtros de tráfego podem bloquear IPs ou países específicos e implementar a limitação de taxa para proteger contra ataques de DDoS. A limitação de taxa pode ser configurada com base em vários critérios, como IP do cliente, agente do usuário e caminho da solicitação.
* **Ferramentas de Monitoramento e Análise** O Adobe fornece ferramentas, como painéis do Elasticsearch/Kibana e do Splunk, para analisar o tráfego e o uso, ajudando a identificar e mitigar possíveis ameaças à segurança.
* **Demonstração prática** A apresentação inclui uma demonstração sobre como implantar configurações de CDN usando o Cloud Manager e como lidar com erros e validar configurações localmente usando o AEM.
