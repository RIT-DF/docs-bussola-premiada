---
title: "Política de Privacidade"
nav_order: 2
parent: "Jurídico"
permalink: /legal/privacidade/
last_verified: 2026-07-05
status: publicado
---

# Política de Privacidade

Esta política descreve como o **plugin Bússola Premiada** trata dados pessoais. Ela trata da **ferramenta**; a política que os participantes das suas campanhas leem é a que a **sua organização** publica no próprio site.

> ⚠️ **Importante**
>
> Ao usar o Bússola Premiada, a **organização** atua como **controladora** dos dados pessoais dos participantes das suas campanhas, nos termos da **LGPD (Lei nº 13.709/2018)**. A RIT e a V3RTECH fornecem o software; não são controladoras dos dados tratados no site da organização.

## Onde os dados ficam

O Bússola Premiada roda **dentro do WordPress da própria organização**. Os dados das campanhas e dos participantes são armazenados no **banco de dados do site da organização**, sob o controle dela. O plugin não envia esses dados para servidores da RIT ou da V3RTECH.

## Que dados o plugin trata

No curso normal de uma campanha, o plugin pode tratar:

- **Dados de participantes/compradores**: nome, e-mail e demais dados fornecidos no checkout do WooCommerce, além dos cartões adquiridos.
- **Dados do contemplado**: as informações necessárias para identificar o ganhador e comprovar a entrega do prêmio (mantidas como **privadas**).
- **Consentimento de comunicação**: registro de quem aceitou (ou não) receber e-mails promocionais, com data e versão do texto de consentimento.
- **Metadados de e-mail**: destinatário, assunto e status de envio (o **corpo** do e-mail não é guardado no log).
- **Trilha de auditoria**: registro de ações sensíveis (quem fez o quê e quando), para governança.

## Princípios adotados (privacy-by-design)

- **Mascaramento por padrão**: relatórios exportados saem com os dados pessoais **mascarados**; desmascarar exige permissão específica e **toda exportação é registrada**.
- **Documento do contemplado sempre privado**: forçado pelo sistema.
- **Página pública com exposição mínima**: nunca expõe identificadores internos nem dados pessoais; o resultado do sorteio mostra o cartão ganhador **mascarado** por padrão.
- **Consentimento explícito** para comunicações promocionais, com **descadastro** de um clique. E-mails transacionais (confirmação de compra) são enviados como parte da execução da compra.
- **Menor privilégio**: papéis e permissões limitam quem acessa o quê; o Auditor vê sem alterar.
- **Arquivos sensíveis protegidos**: PDFs que podem conter dados pessoais são gravados em área **não acessível pela web**.

## Direitos dos titulares

Os direitos dos participantes (acesso, correção, eliminação etc.) são exercidos perante a **organização controladora**, conforme a política de privacidade que ela publica. A organização é responsável por atender a esses pedidos — o Bússola Premiada oferece os meios para localizar e exportar os dados quando necessário.

Na prática, o administrador usa as ferramentas nativas do WordPress em **Ferramentas → Exportar dados pessoais** e **Ferramentas → Apagar dados pessoais** (por e-mail). O plugin contribui com esses pedidos: **exporta** o consentimento de comunicações e a situação de contemplado e **apaga** o consentimento quando solicitado. Os **documentos pessoais do contemplado** (como cópia de identidade) são **mantidos** enquanto durar a obrigação legal de prestação de contas do sorteio (base legal — LGPD art. 16); a organização os remove manualmente quando essa obrigação não se aplicar mais. Os dados de compra são tratados pelo WooCommerce, que tem suas próprias ferramentas de exportação/eliminação.

## Responsabilidade da organização

Cabe à organização: definir as bases legais e finalidades do tratamento, informar os participantes por meio da sua própria política de privacidade, manter os dados seguros e atualizados e cumprir as obrigações da LGPD.

## Contato

Dúvidas sobre a ferramenta podem ser encaminhadas à [RIT](https://rit.org.br). Dúvidas sobre o tratamento de dados de uma campanha específica devem ser dirigidas à **organização** que a promoveu.

> 📌 Esta política trata do plugin. Veja também o [Aviso legal](/legal/aviso/) e os [Termos de Uso](/legal/termos/).
