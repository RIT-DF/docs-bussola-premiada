---
title: "Novidades"
nav_order: 8
permalink: /novidades/
source_docs: [CHANGELOG.md]
last_verified: 2026-07-05
status: publicado
---

# Novidades

O que há de novo no Bússola Premiada, em linguagem simples. Cada item indica a **versão** do plugin em que a novidade chegou. Você vê a versão instalada no topo do painel, ao lado da logo (ex.: *Bússola Premiada · v1.2.1*).

> Esta é uma versão amigável do histórico técnico. O registro completo para desenvolvedores fica no `CHANGELOG.md` do projeto.

---

## Versão 1.5.0 — Blocos e shortcodes para montar sua página

- **Monte a página da campanha no seu construtor.** Agora você pode compor a página da campanha no editor de blocos do WordPress (Gutenberg) ou em construtores como o Elementor, usando **8 componentes** prontos: seleção de cartões, painel de transparência, barra de progresso, resultado do sorteio, botão comprar, compartilhamento, regulamento e a rifa completa. Cada um funciona como **bloco** (categoria “Bússola Premiada”) e como **shortcode**. Veja [Montar a página no construtor](/guias/montar-pagina-construtor/) e [Blocos e Shortcodes](/modulos/blocos-shortcodes/).
- **Nova página de referência.** No menu do plugin, a página **Blocos e Shortcodes** lista todos os componentes com exemplos prontos para copiar.

## Versão 1.4.1 — Correção na tela de Auditoria

- **Tabela de auditoria visível no computador.** Corrigido um problema em que a lista de auditoria não aparecia no desktop.

## Versão 1.4.0 — Mais proteção contra abusos

- **Reservas ainda mais protegidas.** Novas barreiras de segurança nas reservas públicas (limite por campanha e um desafio automático sob picos de acesso) reforçam a proteção contra uso abusivo — sem atrapalhar quem participa de verdade.

## Versão 1.3.0 — Trilha de auditoria consultável

- **Nova tela de Auditoria.** O plugin já registrava as ações sensíveis nos bastidores; agora há uma **tela de consulta** para elas: filtre por ação, tipo, origem, usuário e período, expanda cada registro e exporte em CSV. Ideal para o conselho fiscal e para a prestação de contas. Veja [Auditoria](/modulos/auditoria/).

## Versão 1.2.2 — Ajuste técnico

- Correção interna no carregamento do plugin (empacotamento), sem mudança visível no uso.

## Versão 1.2.1 — Mais segurança

- **Reservas públicas mais protegidas.** A página pública ficou mais resistente a abusos: há um limite de cartões que um mesmo visitante pode manter reservados ao mesmo tempo, evitando que alguém "trave" a rifa sem comprar.
- **Descadastro de e-mail à prova de engano.** O link de descadastro passou a pedir uma confirmação, para que verificadores automáticos de link (comuns em provedores de e-mail) não descadastrem ninguém por engano.
- **Confirmação de compra sem duplicidade.** Ajustes internos garantem que o e-mail de confirmação de compra não seja enviado duas vezes, mesmo se o pagamento notificar o sistema mais de uma vez.

## Versão 1.2.0 — Painel geral e apoio à RIT

- **Novo Painel com indicadores.** A tela inicial agora traz uma visão geral: valor apurado, resultado líquido, ranking de campanhas, ticket médio, próximos sorteios com contagem regressiva e um filtro de período. Tudo em números agregados, sem expor dados pessoais. Veja [Painel](/modulos/painel/).
- **Doação voluntária à RIT.** Um recurso opcional para destinar parte da margem ao projeto que mantém o plugin — com valor sugerido e registro das doações feitas. Totalmente opcional. Veja [Apoiar a RIT](/guias/apoiar-a-rit/).

## Versão 1.1.0 — Listas de cartões prontas

- **9 listas temáticas embarcadas.** Para você não precisar montar tudo do zero, o plugin passou a vir com listas prontas de cartões: Animais do Brasil, Artistas, Cidades do Brasil, Clássicos da literatura, Especialidades escoteiras, Ficção científica, Heróis dos quadrinhos, Músicas K-pop e Pessoas históricas. Veja [Montar os cartões](/guias/montar-cartoes/).

## Versão 1.0.0 — Primeira versão completa

A primeira versão formal do Bússola Premiada, reunindo todo o ciclo de uma campanha premiada:

- **Configurações da organização** como fonte única de dados institucionais.
- **Campanhas** de ponta a ponta, com produto oculto no WooCommerce e formulário em etapas.
- **Templates e cartões** (números ou listas), com reserva anti-duplicidade.
- **Regulamento obrigatório e semi-automático**, versionado e carimbado.
- **Página pública mobile-first** com 5 templates visuais, transparência e compartilhamento.
- **Checkout, pedidos e descontos** integrados ao WooCommerce.
- **E-mails automáticos** e consentimento conforme a LGPD.
- **Apuração auditável** (interno reproduzível, Loteria Federal ou manual) e resultado público.
- **Prestação de contas** com checklist e relatórios em CSV, PDF e JSON.

---

Quer detalhes de como usar cada novidade? Comece pelos [Guias por tarefa](/guias/) ou explore os [Módulos](/modulos/).
