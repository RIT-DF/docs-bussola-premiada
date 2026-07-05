---
title: "Blocos e Shortcodes"
nav_order: 12
parent: "Módulos"
permalink: /modulos/blocos-shortcodes/
role: admin
routes: ["#/blocos"]
screenshots: [bp-25-blocos-referencia, bp-26-blocos-editor]
source_docs: [PRD_Bussola_Premiada.md#8.24]
last_verified: 2026-07-05
status: publicado
---

# Blocos e Shortcodes

Além da página pública pronta (o hotsite da campanha), você pode **montar a sua própria página** no construtor de páginas do WordPress — o editor de **blocos (Gutenberg)** ou construtores como o **Elementor** — combinando os componentes da campanha do jeito que quiser. Novo na versão **1.5.0**.

## Onde encontrar a referência

No menu **Bússola Premiada**, abra **Blocos e Shortcodes**. Essa página lista cada componente com o nome do bloco, o shortcode e um exemplo pronto para copiar.

![Página Blocos e Shortcodes no admin](/assets/screenshots/bp-25-blocos-referencia.png)

## Os componentes disponíveis

Cada um funciona como **bloco** e como **shortcode**:

| Componente | O que mostra | Shortcode |
|---|---|---|
| **Seleção de cartões** | Grade para o participante escolher e comprar cartões | `[bussola_premiada_selecao id="ID"]` |
| **Painel de transparência** | Indicadores públicos (vendidos, disponíveis, sorteio…) | `[bussola_premiada_painel id="ID"]` |
| **Barra de progresso** | Barra compacta com o % de cartões vendidos | `[bussola_premiada_progresso id="ID"]` |
| **Resultado do sorteio** | Cartão contemplado e ganhador, após a apuração | `[bussola_premiada_resultado id="ID"]` |
| **Botão comprar** | Botão de destaque que leva à seleção de cartões | `[bussola_premiada_botao id="ID"]` |
| **Compartilhamento** | Botões de WhatsApp, redes sociais e copiar link | `[bussola_premiada_compartilhar id="ID"]` |
| **Regulamento** | Resumo do regulamento, com “ver completo” | `[bussola_premiada_regulamento id="ID"]` |
| **Rifa completa (página)** | A página inteira da campanha em um bloco | `[bussola_premiada_rifa id="ID"]` |

> Troque `ID` pelo número da campanha (você encontra o ID na lista de **Campanhas**).

## Usando os blocos (Gutenberg)

No editor de uma página ou post, clique em **adicionar bloco** (o “+”), procure por **“Bússola”** e escolha o componente na categoria **Bússola Premiada**. Com o bloco selecionado, abra o painel de configurações à direita e **escolha a campanha** no menu suspenso (ou informe o ID manualmente).

![Bloco da Bússola Premiada no editor do WordPress](/assets/screenshots/bp-26-blocos-editor.png)

> 💡 **Nota**
>
> No editor, o bloco aparece como um marcador (“Bússola Premiada · …”). A **aparência real** — a grade de cartões, o painel, a barra — aparece na **página publicada**, para quem visita o site.

## Usando os shortcodes (Elementor e outros)

Em construtores que aceitam shortcodes (como o Elementor, via o widget **Shortcode**), cole o shortcode do componente, ajustando o `id` da campanha. Também funciona direto no conteúdo de qualquer página/post.

## Segurança e privacidade

Os blocos e shortcodes usam exatamente a mesma proteção da página pública: só exibem campanhas **disponíveis publicamente** e nunca mostram dados privados. Se a campanha não estiver disponível (rascunho, cancelada, inexistente), o componente exibe uma **mensagem clara** no lugar.

> ✅ **Boas práticas**
>
> - Comece pela **Rifa completa** se quiser algo pronto rápido; use os componentes granulares quando quiser um layout próprio (por exemplo, a barra de progresso no topo da home e o botão comprar em vários pontos da página).
> - Sempre confira a página **no celular** antes de divulgar — a maioria dos participantes acessa pelo telefone.
