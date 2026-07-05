---
title: "Configurar a organização"
nav_order: 1
parent: "Guias por tarefa"
permalink: /guias/configurar-organizacao/
task: configurar-organizacao
role: admin
routes: ["#/organizacao"]
screenshots: [bp-15-config-organizacao, bp-16-config-identidade, bp-17-config-bancario]
source_docs: [PRD_Bussola_Premiada.md#8.1]
last_verified: 2026-07-05
status: publicado
---

# Configurar a organização

Os dados da sua organização são a **fonte única** que alimenta o regulamento, os e-mails e a página pública de todas as campanhas. Configure uma vez, com calma, e não precisará repetir a cada campanha.

## Onde fica

No menu **Bússola Premiada**, abra **Configurações**. A tela tem várias abas no topo.

## Passo a passo

1. Abra **Configurações** e fique na aba **Configurações da Organização**.
   ![Aba Configurações da Organização](/assets/screenshots/bp-15-config-organizacao.png)
2. Preencha os **dados institucionais**: razão social, CNPJ, endereço e e-mail. Razão social, CNPJ e e-mail são obrigatórios — o plugin valida o CNPJ (aceita o formato numérico e o novo alfanumérico da Receita Federal).
3. Vá para a aba **Identidade visual** e envie a **logomarca** e o **favicon** pela Biblioteca de Mídia do WordPress. Ajuste as **cores da marca** — você pode escolher no seletor de cor ou digitar o valor hexadecimal (ex.: `#192444`). Essas cores personalizam a página pública das campanhas.
   ![Aba Identidade visual](/assets/screenshots/bp-16-config-identidade.png)
4. Na aba **Bancário e contato**, informe os dados de contato e bancários da organização. Alguns desses dados são sensíveis e **nunca** aparecem na página pública — ficam disponíveis só internamente e nos documentos.
   ![Aba Bancário e contato](/assets/screenshots/bp-17-config-bancario.png)
5. **Salve** cada aba. O salvamento é por aba, então confirme antes de trocar de seção.

## As outras abas

A tela de Configurações também guarda ajustes que você vai usar depois:

- **Banco de Cláusulas de Regulamento** — a biblioteca de cláusulas prontas que alimenta o regulamento das campanhas.
- **Apuração** — os padrões globais de sorteio (método, política do contemplado reembolsado).
- **PDF / Relatórios** — o motor de geração de PDF dos documentos.

> 💡 **Dica**
>
> Quando você publica o regulamento de uma campanha, o plugin tira uma **"foto" (snapshot)** dos dados da organização naquele instante. Ou seja: mudar os dados depois **não** altera regulamentos já publicados — cada documento preserva o que valia quando foi emitido. Por isso, preencha tudo corretamente **antes** de publicar campanhas.

> ✅ **Boas práticas**
>
> Confira o CNPJ e a razão social com o cartão CNPJ oficial. Esses dados vão para documentos legais e para o regulamento — um erro aqui se propaga para tudo.
