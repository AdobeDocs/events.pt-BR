---
title: GEMs do AEM - Introdução ao CDN gerenciado pela Adobe
description: Saiba como configurar o Adobe Managed CDN no AEM Cloud Service para aprimorar o desempenho e a segurança com novos recursos de configuração de CDN.
role: Developer, User
level: Intermediate
feature: Edge Delivery Services
doc-type: Event
duration: 3438
last-substantial-update: 2025-01-30T00:00:00Z
jira: KT-17227
exl-id: 4cd0332f-95bf-45f4-a765-aba020c0d7b0
source-git-commit: 91f20c3e9ee5ae5b259d5cb3da476974acdc6585
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# GEMs do AEM - Introdução ao CDN gerenciado pela Adobe

Saiba mais sobre o Adobe Managed CDN no AEM Cloud Service e como ele pode ser configurado. Junte-se a nós para explorar os novos recursos de configuração de CDN que podem ser usados para aprimorar o desempenho e a segurança de seus aplicativos do AEM as a Cloud Service. Nesta sessão, você descobrirá:

* O que é a CDN do Adobe
* Topologias relevantes para o AEMaaCS e o Edge Delivery Services
* Casos de uso típicos que podem ser implementados com regras CDN
* Como usar RDEs para testar e implantar rapidamente configurações de CDN

>[!VIDEO](https://video.tv.adobe.com/v/3443168/?learn=on&enablevpops)

*Gravado em 22 de janeiro de 2025*

Você tem uma pergunta, talvez um comentário?  Participe da discussão nas [Comunidades Experience League](https://adobe.ly/4haufPK)!

## Principais pontos

### Principais recursos da CDN gerenciada pela Adobe

* **Domínios e Certificados Personalizados** Essenciais para hospedar domínios e certificados personalizados para estabelecer conexões seguras.
* **O armazenamento em cache** da entrega de respostas HTTP do cache é significativamente mais rápido (menos de 10 milissegundos) em comparação à busca da origem (centenas de milissegundos).
* **A Adobe pronta para uso e a CDN personalizada** fornece uma CDN gerenciada pronta para uso, mas os usuários também podem trazer sua própria CDN.

### Opções de configuração

* **Solicitar transformações** Modificar cabeçalhos, regravar caminhos, bloquear tráfego e redirecionar solicitações.
* **Filtros de Tráfego** Bloqueiam ou permitem tráfego com base em regras específicas.
* **Autenticação** Suporte para chave de borda, chave de perfuração e autenticação básica.
* **Seletores de Origem** Solicitações de proxy para origens diferentes com base em regras definidas.
* **Transformações de Resposta** Modifique os cabeçalhos e o status da resposta.

### Implantação e personalização

* **Pipeline de Configuração** Implante arquivos YAML para configurar as regras CDN.
* **Proteção de tráfego** Use as regras de filtro de tráfego para bloquear, registrar e alertar o tráfego com base nos padrões.
* **Limitação de taxa** Proteja-se contra ataques de DDoS limitando o número de solicitações por IP.

### Ferramentas e análise

* **Pilha de Kibana do Elasticsearch** Analise o uso e o tráfego com os painéis fornecidos.
* **Encaminhamento de Log** Encaminha logs para uma instância do Splunk para análise.

### Destaques da demonstração

* **Implantando configurações** Demonstrada a implantação de regras de filtro de tráfego e redirecionamentos.
* **Seleção de Autenticação e Origem** Mostrou como configurar a autenticação básica e o tráfego de proxy para origens diferentes.

### Práticas recomendadas

* **Respostas rápidas** Garanta respostas rápidas das origens para evitar vulnerabilidades.
* **Bom armazenamento em cache** Aproveite esse armazenamento para lidar com o tráfego com eficiência.
* **Use Painéis**. Analise o tráfego e o uso para definir limites de taxa apropriados.
* **Combinar estratégias** Use estratégias de limitação de taxa diferentes para obter melhor proteção.
* **Definir alertas** Receba notificações quando o site estiver sob ataque.
* **Testar regras** Comece com ações de registro antes de bloquear para garantir que as regras funcionem conforme esperado.

### Contato e feedback

* **Feedback e casos de uso** Entre em contato com a equipe para obter casos de uso avançados e feedback.
* **Sessões Futuras** Participe de pesquisas para sugerir tópicos para sessões futuras.
