---
title: "Realizar o sorteio"
nav_order: 8
parent: "Guias por tarefa"
permalink: /guias/realizar-sorteio/
task: realizar-sorteio
role: admin
routes: ["#/campanhas/:id"]
screenshots: [bp-21-apuracao]
source_docs: [PRD_Bussola_Premiada.md#8.14, PRD_Bussola_Premiada.md#8.15]
last_verified: 2026-07-05
status: publicado
---

# Realizar o sorteio

Chegou a data. O Bússola Premiada faz a apuração de forma **auditável** — de um jeito que qualquer pessoa possa confiar no resultado. Você escolhe entre três métodos.

## Onde fica

Abra a campanha e clique na aba de topo **Apuração**.

![Aba Apuração](/assets/screenshots/bp-21-apuracao.png)

## Passo 1 — Congelar a base

Antes de sortear, você **congela** a lista de cartões vendidos. A partir daí:

- A base não muda mais — ninguém entra ou sai.
- Reembolsos e cancelamentos **não** devolvem mais o cartão ao pool (ficam registrados e auditados).
- No método interno, é publicado um **lacre** (um código `sha256` da semente do sorteio), provando que a semente foi definida **antes** do resultado.

## Passo 2 — Escolher o método

- **Interno (reproduzível)** — o plugin sorteia usando uma semente secreta lacrada no congelamento. Ao finalizar, a semente é revelada e **qualquer auditor pode refazer a conta** e chegar ao mesmo cartão. Transparência total, sem depender de terceiros.
- **Loteria Federal** — o resultado é definido pela extração da Loteria Federal. Você informa o concurso; o plugin extrai os últimos dígitos do número premiado e aplica a **regra de não-bate** que você definiu (caso o número não corresponda a um cartão vendido). O plugin pode buscar a extração automaticamente, mas **você confirma** — ele nunca decide sozinho.
- **Manual** — para sorteios feitos fora do sistema (uma live, um evento). Você registra o resultado com **justificativa e anexos**.

## Passo 3 — Finalizar e publicar

Ao finalizar, o resultado é **travado** (imutável). O(s) contemplado(s) é(são) definido(s) e:

- O **resultado público** aparece na página da campanha, com o cartão ganhador **mascarado** por padrão (protege os dados pessoais do ganhador).
- São enviados os e-mails de **resultado** (a todos) e de **ganhador** (ao contemplado).

### Campanha com vários prêmios

Se a campanha tem **mais de um prêmio**, a apuração sorteia **todos de uma vez**, sobre a mesma base congelada, **sem repetir cartão** — o 1º, o 2º, o 3º… saem em sequência. A aba Apuração mostra a lista dos contemplados por prêmio, e cada ganhador recebe seu e-mail. Nos métodos **interno** e **Loteria Federal** o plugin resolve os N contemplados automaticamente; no método **manual**, você informa um cartão para cada prêmio.

> ⚠️ **Atenção**
>
> Reprocessar um resultado já finalizado cria uma **nova versão** e exige o papel de **Administrador do plugin**. O resultado anterior não é apagado — fica registrado como substituído. Isso preserva a trilha de auditoria.

> ✅ **Boas práticas**
>
> Se a sua modalidade permite, o sorteio pela **Loteria Federal** é o método mais reconhecido e transparente para o público. O método **interno reproduzível** é uma excelente alternativa quando você quer autonomia mantendo a auditabilidade. Descreva no [regulamento](/guias/publicar-regulamento/) qual método será usado, **antes** de abrir a campanha.
