---
title: "Regulamento"
nav_order: 4
parent: "Módulos"
permalink: /modulos/regulamento/
role: admin
routes: ["#/campanhas/:id"]
screenshots: [bp-08-regulamento]
last_verified: 2026-07-05
status: publicado
---

# Regulamento

O regulamento é o documento que define as regras da campanha — e é **obrigatório**: nenhuma campanha abre sem um regulamento publicado. O módulo monta a maior parte do texto para você.

![Aba Regulamento](/assets/screenshots/bp-08-regulamento.png)

## Semi-automático

O regulamento combina três fontes:

1. **Dados automáticos** da organização e da campanha (nome, CNPJ, prêmio, datas, quantidade, valor).
2. **Campos variáveis** que você preenche.
3. **Biblioteca de cláusulas** selecionáveis por categoria, mais texto livre. A biblioteca é editável em **Configurações → Banco de Cláusulas de Regulamento**.

## Versionado e carimbado

- Ao publicar, o plugin tira um **snapshot** dos dados da organização — o documento fica fiel ao que valia naquele momento.
- A primeira publicação é a **v1**; editar depois cria **v2, v3…**, arquivando a anterior. Há **histórico** completo.
- É um **gate de publicação**: a campanha só abre com o regulamento publicado.

## Público

O regulamento publicado aparece na página da campanha, com o conteúdo sanitizado e seguro.

O passo a passo está em [Publicar o regulamento](/guias/publicar-regulamento/).

> ⚠️ **Importante**
>
> Descreva no regulamento o **método de apuração** que será usado e todas as regras relevantes **antes** de abrir a campanha. Um regulamento claro é a base da segurança jurídica e da confiança do público. Veja [Requisitos legais de um sorteio](/boas-praticas/requisitos-legais/).
