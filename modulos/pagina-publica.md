---
title: "Página pública"
nav_order: 5
parent: "Módulos"
permalink: /modulos/pagina-publica/
role: admin
routes: ["#/campanhas/:id", "/campanha/:slug"]
screenshots: [bp-10-pagina-publica-admin, bp-11-pagina-publica-site]
last_verified: 2026-07-05
status: publicado
---

# Página pública

Cada campanha tem um **hotsite próprio**, mobile-first, no endereço `/campanha/nome-da-campanha`. É a vitrine da sua rifa.

![Página pública da campanha](/assets/screenshots/bp-11-pagina-publica-site.png)

## O que a página traz

- O(s) **prêmio(s)** com galeria de fotos — quando a campanha tem vários prêmios, todos aparecem em ordem (1º, 2º, 3º…).
- A **história da causa** (texto rico).
- O **progresso das vendas** e o **painel de transparência** (indicadores que você escolhe).
- A **seleção de cartões** (manual ou automática).
- O **regulamento**.
- A **barra de compartilhamento** (WhatsApp, Facebook, X, LinkedIn, copiar link).
- O **resultado** do sorteio, quando a campanha é apurada — com um ganhador por prêmio, sempre mascarado por padrão.

## Configuração

Na aba **Página pública** da campanha você escolhe o **template visual** (Sofisticado, Moderno, Clássico, Divertido, Emotivo), os indicadores de **transparência** e as opções de **compartilhamento/Open Graph**.

![Aba Página pública no admin](/assets/screenshots/bp-10-pagina-publica-admin.png)

## Shortcodes para page builders

Quer usar partes da campanha em outra página do site? Há shortcodes prontos, por exemplo:

- `[bussola_premiada_rifa id="123"]` — a campanha completa.
- `[bussola_premiada_comprar id="123"]` — a seleção de cartões.
- `[bussola_premiada_regulamento id="123"]` — o regulamento.
- `[bussola_premiada_painel id="123"]` — o painel de transparência.

## Segurança e privacidade

A página pública usa uma **lista de exposição explícita**: nunca mostra identificadores internos, o token da página nem dados pessoais. O valor arrecadado só aparece se você **optar** por exibi-lo.

O passo a passo está em [Personalizar a página pública](/guias/personalizar-pagina-publica/).

> ⚠️ **Atenção — 404 no endereço da campanha**
>
> Se `/campanha/nome` retornar "não encontrado", vá em **Configurações → Links permanentes** do WordPress e clique em **Salvar** para regenerar as regras. O plugin tenta fazer isso automaticamente, mas o permalink "simples" do WordPress pode exigir o passo manual.
