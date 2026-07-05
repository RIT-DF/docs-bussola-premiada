---
title: "Apuração"
nav_order: 7
parent: "Módulos"
permalink: /modulos/apuracao/
role: admin
routes: ["#/campanhas/:id"]
screenshots: [bp-21-apuracao]
last_verified: 2026-07-05
status: publicado
---

# Apuração

O módulo de apuração define o **ganhador** de forma auditável. Ele oferece três métodos e cuida da imutabilidade do resultado.

![Aba Apuração](/assets/screenshots/bp-21-apuracao.png)

## Congelamento da base

Antes do sorteio, a lista de cartões vendidos é **congelada**: fica fixa, com uma "impressão digital" (hash). A partir daí, reembolsos e cancelamentos não devolvem mais o cartão ao pool — tudo fica registrado. No método interno, um **lacre** (`sha256` da semente) é publicado, provando que a semente foi definida antes do resultado (esquema *commit-reveal*).

## Três métodos

- **Interno (reproduzível)** — semente lacrada + revelação ao finalizar. Sorteia sobre a base congelada completa, pulando reembolsados de forma determinística. **Qualquer auditor refaz a conta** e chega ao mesmo cartão.
- **Loteria Federal** — extrai os últimos dígitos do número premiado de um concurso; aplica a **regra de não-bate** escolhida se o número não corresponder a um cartão vendido (superior, inferior, mais próximo, próximo prêmio ou manual). O plugin pode buscar a extração, mas **você confirma**.
- **Manual** — resultado feito fora do sistema, registrado com justificativa e anexos.

## Resultado imutável e público

Ao finalizar, o resultado **trava**. O ganhador aparece na página pública com o cartão **mascarado** por padrão (protege os dados do contemplado). São disparados os e-mails de **resultado** e de **ganhador**. Reprocessar cria uma **nova versão** e exige o papel de Administrador do plugin — nada é apagado.

O passo a passo está em [Realizar o sorteio](/guias/realizar-sorteio/).

> ✅ **Boas práticas**
>
> Escolha e **descreva o método no regulamento** antes de abrir a campanha. Mudar a regra de apuração depois de vender cartões mina a confiança — e pode ter implicações legais.
