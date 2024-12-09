---
title: Autenticação simplificada - Migração da conta de serviço (JWT) para credenciais de servidor para servidor do OAuth
description: O webinário Adobe, liderado pelos engenheiros de campo sênior Jeff Homequest e Marco Lara, focou na migração do JWT da conta de serviço para credenciais de servidor para servidor OAuth, destacando o prazo de desativação de janeiro de 2025, as etapas de migração, os benefícios do OAuth e as considerações especiais para o AEM, com amplo suporte e documentação fornecidos para o processo.
role: Admin, Developer, Leader, User
level: Intermediate
doc-type: Event
duration: 3292
last-substantial-update: 2024-12-06T00:00:00Z
jira: KT-16629
source-git-commit: 47ae42d06ed311e60ebce194e0683bb95e8e5b69
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---


# Autenticação simplificada: migração de conta de serviço (JWT) para credenciais de servidor para servidor do OAuth

Este webinário guiará os participantes pela migração das credenciais obsoletas da Conta de serviço (JWT) para as novas credenciais de servidor para servidor do OAuth. Como as credenciais da Conta de serviço (JWT) deixarão de funcionar após 27 de janeiro de 2025, é crucial que os desenvolvedores e as organizações entendam o processo de migração para evitar possíveis interrupções do serviço. O webinário também destacará os benefícios das credenciais de servidor para servidor do OAuth e como garantir uma migração sem tempo de inatividade.

>[!VIDEO](https://video.tv.adobe.com/v/3440936/?learn=on&enablevpops)

## Principais pontos

* **Gravação da Reunião e Slides** A reunião foi gravada e um link para a gravação estará disponível no final.
* **Introdução aos palestrantes** Jeff Homequest e Marco Lara, ambos engenheiros sêniores de campo da Adobe, conduziram o webinário.
* **Foco do webinário** O webinário concentrou-se na migração do JWT da conta de serviço para credenciais de servidor para servidor OAuth.
* **Prazo de descontinuação** O Adobe está descontinuando as credenciais do JWT e elas devem ser migradas até o final de janeiro de 2025.
* **Público-alvo** O webinário foi destinado a desenvolvedores de aplicativos, líderes técnicos e arquitetos de integração usando credenciais JWT em aplicativos Adobe.
* **Etapas de migração** O webinário incluiu um guia de migração passo a passo e uma demonstração.
* **Sessão de perguntas e respostas** As perguntas foram feitas durante toda a reunião, com uma sessão de perguntas e respostas dedicada no final.
* **Vantagens do OAuth** O OAuth simplifica o desenvolvimento, melhora a segurança e simplifica a manutenção em comparação com o JWT.
* **Linha do tempo para migração**
   * 1 de maio de 2023 - Anúncio de descontinuação futura.
   * 2 de junho de 2024 - Última data para criar novas credenciais de conta de serviço.
   * 27 de janeiro de 2025 - O fim da vida útil das contas de serviço e as APIs que as utilizam deixarão de funcionar.
* **&#x200B;Considerações especiais sobre o AEM** O webinário abordou como a migração afeta a nuvem e os clientes locais do AEM, incluindo padrões e configurações de autorização específicos.
* **Integrações geradas automaticamente** As integrações geradas automaticamente serão migradas pelo Adobe antes do prazo.
* O Adobe **Suporte e documentação** fornece ampla documentação e suporte para o processo de migração. Os clientes podem entrar em contato com representantes da Adobe ou com serviços profissionais para obter assistência.
* **Teste e validação** É recomendável testar completamente as integrações após a migração e antes de excluir as credenciais JWT antigas.
* **Integrações personalizadas** Os clientes com integrações personalizadas devem identificar e planejar a migração o mais rápido possível, especialmente se houver fornecedores de terceiros envolvidos.