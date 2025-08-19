---
title: Desempenho de entrega do Adobe Campaign Classic - Solução de problemas
description: Esta sessão abordou as principais estratégias para melhorar o desempenho do delivery de emails e SMS usando o Adobe Campaign. Ele abordou desafios comuns, como atrasos de entrega, taxa de transferência baixa e lentidão transacional, oferecendo soluções como otimização de lotes, registro SQL e monitoramento do desempenho do servidor. As práticas recomendadas de capacidade de delivery incluíam autenticação de email adequada (SPF, DKIM, DMARC), monitoramento de blacklist e verificações de spam. Para melhorar o desempenho, os especialistas recomendam workflows limpos, regras de limitação e evitar contêineres compartilhados. Dicas de delivery de SMS com foco na configuração adequada de conta externa e análise de log. A sessão também enfatizou o rastreamento da validação, a manutenção do banco de dados usando relatórios de sobrecarga e a aplicação de regras de pressão/fadiga para aumentar o engajamento. Uma gravação de sessão será compartilhada por email e publicada no site da Adobe Experience.
solution: Campaign Classic v7
product: Adobe Campaign
feature: SMS, Deliverability, Troubleshooting
role: User
level: Beginner, Intermediate, Experienced
doc-type: Event
duration: 2257
last-substantial-update: 2025-04-25T00:00:00Z
jira: KT-17869
exl-id: a7e1e198-b63b-4a2a-9ffc-7f72bf4c61c1
source-git-commit: 3b54c46988da18248024d115997704d9881f5e68
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Sessões técnicas: desempenho de entrega do Adobe Campaign Classic - Solução de problemas

Nesta sessão, exploraremos os desafios comuns enfrentados ao fornecer o melhor desempenho com o Adobe Campaign Classic (ACC) e forneceremos estratégias acionáveis para solucionar problemas. Os participantes aprenderão a identificar gargalos de desempenho, solucionar inconsistências de preparação/configuração de delivery e implementar práticas recomendadas para garantir uma comunicação tranquila. Desde a otimização de deliveries até a superação de dificuldades técnicas, este webinário fornecerá aos participantes o conhecimento e as ferramentas necessárias para aprimorar a eficiência de suas campanhas de ACC, gerar melhores resultados e fornecer experiências de alta qualidade para o cliente.

>[!VIDEO](https://video.tv.adobe.com/v/3457826/?learn=on&enablevpops)

## Principais pontos

**Desafios e soluções de entrega**

* Problemas comuns incluem atrasos de entrega, falhas de preparação, entregas travadas, baixas taxas de sucesso, baixa taxa de transferência, baixo engajamento e lentidão de entrega transacional.
* As soluções envolvem a otimização do agrupamento de entregas, o monitoramento do desempenho do servidor, a ativação do registro de consultas SQL, a revisão de registros de auditoria e a garantia da configuração adequada de afinidades de MTA e IP.

**Práticas recomendadas de capacidade de entrega**

* Garantir a autenticação de email adequada (SPF, DKIM, DMARC).
* Monitore os status da blacklist e evite o conteúdo de acionamento de spam.
* Use verificações de spam para avaliar as pontuações de spam antes de enviar emails.

**Otimizando o Desempenho de Entrega**

* Use workflows para construção de target limpos e limite os campos de personalização.
* Implemente regras de limitação, processamento em lote e regras de topologia para exclusões e filtragem.
* Evite compartilhar contêineres em vários canais para evitar gargalos.

**Solução de problemas de entrega de SMS**

* Verifique se as contas externas estão configuradas de forma exclusiva e se os processos de SMS estão em execução.
* Verifique os logs SMS em busca de erros e verifique as expressões regulares nas configurações SMP.
* Envolva o provedor de serviços em caso de problemas de configuração incorreta.

**Lentidão De Entrega Transacional**

* Monitore os tempos de processamento interno e total.
* Verifique se o tamanho do delivery está dentro dos limites (60 GB para lote, 30 GB para evento).
* Revise as regras de tipologia e as configurações de personalização.

**Rastreamento e Participação**

* Validar workflows de rastreamento e logs do servidor.
* Teste fórmulas de rastreamento personalizadas em ambientes inferiores antes da produção.
* Verifique se os servidores de rastreamento estão em funcionamento.

**Manutenção de Banco de Dados**

* Use relatórios de aumento para identificar tabelas com aumento excessivo e justificar um vácuo de BD.

**Recomendações gerais**

* Use as regras de pressão e fadiga para limitar emails desnecessários.
* Segmente grandes deliveries em lotes menores para otimizar o desempenho.
