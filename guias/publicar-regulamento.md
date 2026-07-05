---
title: "Publicar o regulamento"
nav_order: 4
parent: "Guias por tarefa"
permalink: /guias/publicar-regulamento/
task: publicar-regulamento
role: admin
routes: ["#/campanhas/:id"]
screenshots: [bp-08-regulamento, bp-09-dados-legais]
source_docs: [PRD_Bussola_Premiada.md#8.10, PRD_Bussola_Premiada.md#8.11]
last_verified: 2026-07-05
status: publicado
---

# Publicar o regulamento

O regulamento é **obrigatório**: nenhuma campanha entra no ar sem um regulamento publicado. A boa notícia é que o Bússola Premiada monta a maior parte dele para você — a partir dos dados da organização, dos dados da campanha e de uma biblioteca de cláusulas prontas.

## Onde fica

Abra a campanha e clique na aba de topo **Regulamento**.

![Aba Regulamento](/assets/screenshots/bp-08-regulamento.png)

## Como funciona

O regulamento é montado de três fontes:

1. **Placeholders automáticos** — dados da organização e da campanha entram sozinhos (nome, CNPJ, prêmio, datas, quantidade, valor).
2. **Campos variáveis** — informações específicas que você preenche.
3. **Biblioteca de cláusulas** — você seleciona as cláusulas padrão que se aplicam (organizadas por categoria) e pode acrescentar texto livre.

## Passo a passo

1. Na aba **Regulamento**, revise os campos variáveis e preencha o que faltar.
2. Selecione as **cláusulas** aplicáveis à sua campanha, por categoria. Você pode editar o banco de cláusulas em **Configurações → Banco de Cláusulas de Regulamento**.
3. Use a **pré-visualização** para conferir o texto final, fiel ao que o público verá.
4. Clique em **Publicar** e confirme.

## O que acontece ao publicar

- O plugin tira um **snapshot** dos dados da organização — o regulamento fica "carimbado" com o que valia naquele momento.
- A primeira publicação vira a **versão 1**. Se você editar depois de publicado, uma nova versão (v2, v3…) é criada e a anterior é arquivada. Assim há **histórico** de tudo.
- O item "regulamento publicado" do checklist da campanha é atendido, liberando a abertura.

## Dados legais

Na aba **Dados legais** você registra número de autorização, processo e observações. São **opcionais**, mas se estiverem em branco o plugin **pede confirmação explícita** antes de publicar a campanha — um lembrete para você não esquecer.

![Aba Dados legais](/assets/screenshots/bp-09-dados-legais.png)

> ✅ **Boas práticas**
>
> Leia o regulamento inteiro na pré-visualização antes de publicar, como se fosse um participante. Ele é o documento que dá segurança jurídica à campanha e transmite seriedade ao público. Veja também [Requisitos legais de um sorteio](/boas-praticas/requisitos-legais/).

> 💡 **Dica**
>
> Se você duplicar uma campanha, o regulamento é copiado junto — ótimo para campanhas recorrentes que seguem o mesmo modelo.
