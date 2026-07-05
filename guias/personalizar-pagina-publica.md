---
title: "Personalizar a página pública"
nav_order: 5
parent: "Guias por tarefa"
permalink: /guias/personalizar-pagina-publica/
task: personalizar-pagina-publica
role: admin
routes: ["#/campanhas/:id", "/campanha/:slug"]
screenshots: [bp-10-pagina-publica-admin, bp-11-pagina-publica-site, bp-29-config-meta-video, bp-30-publica-termometro, bp-31-publica-video]
source_docs: [PRD_Bussola_Premiada.md#8.7, PRD_Bussola_Premiada.md#8.8, PRD_Bussola_Premiada.md#8.9, CHANGELOG.md#1.9.0]
last_verified: 2026-07-05
status: publicado
---

# Personalizar a página pública

Cada campanha ganha uma **página pública própria** (um hotsite), com endereço em `/campanha/nome-da-campanha`. É mobile-first, pronta para compartilhar e é onde as pessoas veem o prêmio, leem o regulamento, escolhem os cartões e compram.

## Onde configura

Abra a campanha e clique na aba de topo **Página pública**.

![Aba Página pública (admin)](/assets/screenshots/bp-10-pagina-publica-admin.png)

## O que dá para ajustar

- **Template visual** — escolha entre 5 estilos prontos: *Sofisticado, Moderno, Clássico, Divertido, Emotivo*. Cada um combina com um tom de campanha diferente. As cores da sua organização são aplicadas por cima.
- **Painel de transparência** — escolha quais indicadores mostrar (total arrecadado, cartões vendidos, cartões restantes…). O financeiro fica **oculto por padrão** — ative só o que quiser expor.
- **Meta da campanha (termômetro)** — defina uma meta de **cartões** e/ou de **arrecadação (R$)** e a página mostra um termômetro com o progresso e um aviso quando a meta é atingida (veja abaixo).
- **Vídeo de divulgação** — cole um link do **YouTube** ou do **Vimeo** e o vídeo aparece embutido na página (veja abaixo).
- **Compartilhamento / Open Graph** — os botões de redes sociais e o card que aparece quando o link é compartilhado.

![Configuração da meta e do vídeo na aba Página pública](/assets/screenshots/bp-29-config-meta-video.png)

### Termômetro de meta

Na seção **Meta da campanha**, marque **Exibir termômetro de meta** e informe:

- **Meta de cartões** — quantos cartões você quer vender (opcional).
- **Meta em R$** — quanto você quer arrecadar (opcional).

Você pode preencher só uma das duas, ou as duas. A barra mostra o progresso com marcos em 25%, 50%, 75% e 100%, e exibe **🎯 Meta atingida!** quando chega lá.

> ⚠️ A **meta em R$** só aparece publicamente se os **indicadores financeiros não estiverem ocultos** (veja o Painel de transparência acima). Se você preferir não mostrar valores, deixe só a meta de cartões — o termômetro de cartões aparece normalmente.

![Termômetro de meta na página pública](/assets/screenshots/bp-30-publica-termometro.png)

### Vídeo de divulgação

Na seção **Vídeo de divulgação**, cole o endereço do vídeo (ex.: `https://youtu.be/...` ou `https://vimeo.com/...`). Só links do **YouTube** e do **Vimeo** são aceitos — não há upload de arquivo. O vídeo aparece embutido na página da campanha.

![Vídeo embutido na página pública](/assets/screenshots/bp-31-publica-video.png)

## Como fica para o público

A página reúne, em uma rolagem: o prêmio com as fotos, a história da causa, o progresso das vendas, a seleção de cartões, o regulamento e os botões de compartilhar.

![Página pública da campanha](/assets/screenshots/bp-11-pagina-publica-site.png)

## Compra: como o participante age

1. Escolhe os cartões — **manualmente** (clicando nos disponíveis) ou pedindo uma **seleção automática** (aleatória).
2. Os cartões ficam **reservados** por alguns minutos (o tempo que você definiu) enquanto ele finaliza.
3. Ele vai ao **checkout do WooCommerce** e paga pelo meio configurado (Pix, cartão, boleto).
4. Ao confirmar o pagamento, os cartões viram **vendidos** e ele recebe um **e-mail com os cartões**.

> 💡 **Dica**
>
> Quer inserir a seleção de cartões ou o regulamento em outra página do site (uma landing page, por exemplo)? Use os **shortcodes** do plugin, como `[bussola_premiada_rifa id="123"]`. Veja [Módulo Página pública](/modulos/pagina-publica/).

> ⚠️ **Atenção — permalinks**
>
> Se o endereço `/campanha/nome` abrir uma página "não encontrada" (404), normalmente é a configuração de **Links permanentes** do WordPress. O plugin tenta ajustar isso sozinho, mas se persistir, vá em **Configurações → Links permanentes** do WordPress e clique em **Salvar** (sem mudar nada) para regenerar as regras.

> ✅ **Boas práticas**
>
> Abra a página pública no **celular** antes de divulgar — a maioria dos seus compradores vai acessá-la assim. Confira se a foto do prêmio, o preço e o botão de comprar estão claros na primeira tela.
