---
title: Práticas recomendadas para entrega eficiente
description: Otimize a entrega de mídia e o desempenho com o Dynamic Media aproveitando o fluxo adaptável, os perfis de vídeo personalizados, as práticas recomendadas de SEO, a otimização de imagens, o gerenciamento de conteúdo em massa, as predefinições do visualizador, a invalidação de cache e a geração inteligente de imagens.
feature: Dynamic Media, Video, SEO Optimization, Smart Imaging, Viewer Presets, Best Practices
topic: Content Management
solution: Experience Manager, Experience Manager Assets
role: Developer
level: Beginner, Intermediate
doc-type: Event
duration: 1596
last-substantial-update: 2024-11-26T00:00:00Z
jira: KT-16572
exl-id: a1920020-b9ce-43be-8f9e-e52aac68da7b
source-git-commit: 946d7cd484e8c5d4358d4099b3518705cab8d4a3
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Práticas recomendadas para entrega eficiente

Junte-se a Riya Midha, Gerente sênior de produtos da Adobe, para explorar as práticas recomendadas para a configuração do Adobe Experience Manager Assets Dynamic Media. Saiba como otimizar a entrega de ativos, aprimorar a transmissão de vídeo, configurar visualizadores e medir e melhorar o desempenho.

>[!VIDEO](https://video.tv.adobe.com/v/3440399/?learn=on&enablevpops)

## Discussão da comunidade

Continue a conversa na [discussão](https://adobe.ly/3YGedpb) da Comunidade do Adobe Developers Live.

## Principais pontos

* **Os Recursos do Dynamic Media** Dynamic Media permitem a entrega rápida e flexível de mídia personalizada e de alta qualidade em vários dispositivos, lidando com mais de 9 trilhões de entregas de mídia anualmente e com volumes máximos diários de até 69 bilhões de ativos.
* **Transmissão adaptável** Usar a transmissão adaptável para entrega de vídeo reduz significativamente o buffer. Um teste mostrou uma redução na contagem de buffer de 50 para 5 em um vídeo de 60 segundos com uma largura de banda restrita de 5 Mbps.
* **Perfis de vídeo** A criação de perfis de vídeo personalizados com diversas codificações de qualidade garante um desempenho de vídeo ideal em várias condições de rede.
* **Práticas recomendadas da SEO**
   * Use conjuntos de regras para criar URLs descritivos para SEO melhor.
   * Adicionar texto alternativo e atributos de título a imagens.
   * Utilize imagens inteligentes e os formatos de imagem mais recentes, como WebP, para obter melhores classificações de pesquisa.
* **Otimização da imagem**
   * Use parâmetros de escala para ajustar a resolução da imagem com base no tamanho da tela.
   * Evite usar 100% de qualidade para imagens; em vez disso, use um intervalo de 80 a 90% para reduzir o tamanho do arquivo sem perda de qualidade notável.
   * Aplique parâmetros de nitidez para melhorar a clareza do texto em imagens.
* **Gerenciamento de conteúdo em massa**
   * Segmente o conteúdo destinado à entrega de mídia dinâmica a partir de outro conteúdo.
   * Use a sincronização seletiva para otimizar os tempos de processamento e melhorar o tempo de comercialização.
* **Predefinições do visualizador** Personalize a aparência e o comportamento do visualizador usando predefinições do visualizador sem alterações de código. Os exemplos incluem editar botões de reprodução/pausa, ativar a reprodução automática e o loop e adicionar sobreposições de imagem.
* **Invalidação de cache** Use a invalidação de cache para refletir imediatamente as alterações feitas em ativos já publicados, ignorando o TTL padrão de 10 horas.
* **Monitoramento e depuração** Use ferramentas como o aplicativo de desktop AEM e a página do depurador de consultas para rastrear trabalhos de processamento e identificar ativos não processados.
* **Smart Imaging** A Smart Imaging é ativada por padrão em todos os domínios, reduzindo o tamanho dos arquivos de imagem e melhorando os tempos de carregamento.
