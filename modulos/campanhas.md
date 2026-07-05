---
title: "Campanhas"
nav_order: 2
parent: "Módulos"
permalink: /modulos/campanhas/
role: admin
routes: ["#/campanhas", "#/campanhas/nova", "#/campanhas/:id"]
screenshots: [bp-02-campanhas-lista, bp-03-campanha-nova-dados, bp-05-campanha-config]
last_verified: 2026-07-05
status: publicado
---

# Campanhas

É o coração do plugin. Aqui você cria, configura, publica e gerencia cada sorteio — do rascunho à conclusão.

![Lista de campanhas](/assets/screenshots/bp-02-campanhas-lista.png)

## O formulário em abas

Uma campanha se organiza em **abas de topo**:

- **Formulário** (3 etapas: Dados da Campanha · Dados do Prêmio · Configurações da Campanha). A etapa **Dados do Prêmio** aceita **um ou vários prêmios** (1º, 2º, 3º lugar…).
- **Regulamento** — obrigatório para publicar (veja [Regulamento](/modulos/regulamento/)).
- **Dados legais** — autorização, processo, observações.
- **Página pública** — template, transparência, compartilhamento (veja [Página pública](/modulos/pagina-publica/)).
- **Apuração** — o sorteio (veja [Apuração](/modulos/apuracao/)).
- **Prestação de contas** — documentos e relatórios (veja [Prestação de contas](/modulos/prestacao-contas/)).

O passo a passo de criação está em [Criar a primeira campanha](/guias/criar-primeira-campanha/).

## Estados da campanha

Cada campanha percorre uma **máquina de estados** que protege a integridade da rifa. Os principais:

- **Rascunho** — edição livre, geração de cartões.
- **Programada** — abre sozinha em uma data futura.
- **Aberta** — vendendo.
- **Aguardando apuração** — vendas encerradas, base congelada.
- **Sorteada** — resultado definido.
- **Concluída** — prestação de contas feita.
- **Cancelada / Arquivada** — encerradas sem sorteio ou guardadas.

O sistema só permite as transições válidas e mantém uma **trilha de auditoria** de tudo.

## Duplicar campanha

Campanhas recorrentes? **Duplique** uma existente — inclusive o regulamento é copiado. Você ajusta só o que muda e ganha tempo.

> 💡 **Exemplo**
>
> Uma associação faz a "Rifa do Dia das Mães" todo ano. Basta duplicar a do ano anterior, trocar prêmio, datas e valor, revisar o regulamento e publicar.

> ⚠️ **Atenção**
>
> Quantidade de cartões e valor unitário são definidos no rascunho e travam após a publicação com vendas. Planeje esses números antes de abrir — veja [Como planejar uma campanha que vende](/boas-praticas/campanha-vencedora/).
