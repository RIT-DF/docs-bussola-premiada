---
title: "Criar a primeira campanha"
nav_order: 3
parent: "Guias por tarefa"
permalink: /guias/criar-primeira-campanha/
task: criar-primeira-campanha
role: admin
routes: ["#/campanhas", "#/campanhas/nova"]
screenshots: [bp-02-campanhas-lista, bp-03-campanha-nova-dados, bp-04-campanha-premio, bp-05-campanha-config]
source_docs: [PRD_Bussola_Premiada.md#8.2, PRD_Bussola_Premiada.md#8.3]
last_verified: 2026-07-05
status: publicado
---

# Criar a primeira campanha

Com a organização configurada e (opcionalmente) os cartões planejados, é hora de criar a campanha. Ela é preenchida em um formulário de **três etapas**.

> 💡 Antes de começar, se ainda não fez a conta do prêmio, preço e quantidade, leia [Como planejar uma campanha que vende](/boas-praticas/campanha-vencedora/). Vale muito o tempo.

## Onde fica

No menu **Bússola Premiada**, abra **Campanhas** e clique em **Nova campanha**.

![Lista de campanhas](/assets/screenshots/bp-02-campanhas-lista.png)

## Etapa 1 — Dados da Campanha

Nome da campanha, descrição curta, descrição completa e a **causa beneficiada**. A descrição completa e a causa aceitam **texto formatado** (negrito, títulos, listas, links) — use isso para contar a história do projeto.

![Etapa Dados da Campanha](/assets/screenshots/bp-03-campanha-nova-dados.png)

## Etapa 2 — Dados do Prêmio

Cada prêmio tem título, descrição, **custo do prêmio** (não aparece ao público; ajuda no cálculo do resultado líquido) e as **fotos do prêmio**. Você pode enviar **várias fotos** por prêmio e definir a **principal** — ela é a que aparece no compartilhamento.

![Etapa Dados do Prêmio](/assets/screenshots/bp-04-campanha-premio.png)

### Um ou vários prêmios

A campanha pode ter **mais de um prêmio** (1º, 2º, 3º lugar…). Use o botão **+ Adicionar prêmio** para incluir cada um, na ordem em que serão sorteados. O primeiro é o **prêmio principal**. Para tirar um prêmio da lista, use **Remover**.

Todos os prêmios são sorteados **da mesma base de cartões vendidos, sem repetir número** — ou seja, cada prêmio vai para um cartão diferente. Se preferir um prêmio só, é só deixar apenas o primeiro; a campanha funciona exatamente como antes.

> 💡 O que muda com vários prêmios: o **regulamento** lista todos os prêmios na ordem; o **resultado público** e os **e-mails** mostram um ganhador por prêmio; e a **prestação de contas** soma os custos de todos os prêmios ao calcular a margem.

> ✅ Capriche nas fotos e no título do prêmio — é o que mais influencia as vendas. Veja [Como escolher um prêmio que vende](/boas-praticas/escolher-premio/).

## Etapa 3 — Configurações da Campanha

Aqui ficam os números e as regras:

- **Valor unitário do cartão** e **quantidade de cartões** (obrigatórios).
- **Datas** de início/fim das vendas e do **sorteio**.
- **Tempo de reserva do cartão** (em minutos) — quanto tempo um cartão fica "segurado" no carrinho antes de voltar ao pool se a compra não for concluída.
- **Método de apuração** (interno, Loteria Federal ou manual).
- **Descontos por quantidade** (opcional).

![Etapa Configurações da Campanha](/assets/screenshots/bp-05-campanha-config.png)

## Salvar e completar

O botão de salvar fica sempre visível. Se algum campo obrigatório faltar, o formulário te leva direto à aba do primeiro erro.

Depois de salvar o rascunho, complete o restante nas **abas de topo** da campanha:

- **Regulamento** — obrigatório para publicar. Veja [Publicar o regulamento](/guias/publicar-regulamento/).
- **Dados legais** — número de autorização, processo, observações (opcional, mas recomendado).
- **Página pública** — template visual, transparência e compartilhamento. Veja [Personalizar a página pública](/guias/personalizar-pagina-publica/).

## Publicar (abrir) a campanha

Quando tudo estiver pronto, use os botões de transição de estado para **Publicar (abrir)** — ou **Programar** para uma data futura. Um **checklist ao vivo** mostra o que ainda falta; o item "regulamento publicado" é **bloqueante**: sem ele, a campanha não abre.

> ⚠️ **Atenção**
>
> Enquanto a campanha está em **rascunho**, você pode ajustar quase tudo, inclusive regerar os cartões. Depois de publicada e com vendas, muitas coisas travam para proteger a integridade da rifa (quantidade de cartões, valor). Revise com cuidado antes de abrir.

Veja todos os estados possíveis em [Módulo Campanhas](/modulos/campanhas/).
