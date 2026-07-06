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

## Versão 1.13.0 — Loteria Federal para qualquer campanha

Agora dá para apurar pela **Loteria Federal** também as campanhas de **lista temática** (cartões que são nomes, não números).

- Cada cartão ganha um **número de sorteio** (a posição na lista, ex.: *Duna · 07*), que casa com o resultado oficial da Loteria Federal.
- Você liga isso na aba **Dados legais** da campanha, em **"Apuração oficial pela Loteria Federal"**. A partir daí o número aparece em todos os lugares onde o cartão é mostrado (compra, e-mail, pedido, "Meus cartões") — o participante sabe com que número concorre.
- Há também um sinalizador **"depende de autorização (SPA/MF)"**, que recomenda a Loteria e oferece uma **cláusula de regulamento** pronta.

Veja em [Realizar o sorteio](/guias/realizar-sorteio/).

---

## Versão 1.12.0 — Painel de gestão da campanha

Cada campanha ganhou um **Painel** — a primeira aba ao abrir a campanha — com a sua visão de gestão num relance:

- **Vendas** (vendidos, % da barra, reservados, disponíveis, pedidos), **Financeiro** (arrecadado, descontos, líquido, ticket médio), **Ritmo** (vendas dos últimos 7 dias, média por dia e uma **projeção de quando deve esgotar**) e **dias até o sorteio**.
- **Meta** e **conversão de reservas**; e, na fase de encerramento, um resumo das **pendências da prestação de contas**.
- Funciona bem no celular e não exige nenhuma configuração — está pronto em toda campanha.

Veja em [Painel da campanha](/guias/painel-da-campanha/).

---

## Versão 1.11.0 — Painel "Meus cartões" para o comprador

Agora o participante consulta **sem precisar de login** os cartões que comprou e o resultado do sorteio.

- Todo **e-mail de confirmação de compra** passa a trazer um link pessoal *"meus cartões"*. Quem perdeu o e-mail pode pedir o link de novo pelo formulário **"Receber o link por e-mail"** na própria página.
- O painel agrupa tudo **por campanha**: os **números** comprados, a **situação do pedido** e, depois do sorteio, o **resultado** — com destaque **"🎉 Você foi contemplado!"** e link para conferir a apuração.
- Sua organização publica esse painel no endereço pronto **`/meus-cartoes`**, ou embute em qualquer página pelo bloco/shortcode **Meus cartões**.
- Feito com privacidade em primeiro lugar: o link é pessoal e não adivinhável, e o formulário nunca revela se um e-mail comprou ou não.

Veja em [Painel "Meus cartões" do comprador](/guias/painel-meus-cartoes/).

---

## Versão 1.10.0 — Modelos radicais da página pública

Sua campanha ganha **6 modelos** de página que transformam de verdade o visual — não é só trocar a cor:

- **Moderno** (foco em conversão), **Sofisticado** (elegante, com a foto do prêmio no topo), **Clássico** (estilo jornal, duas colunas), **Emotivo** (a causa em primeiro plano, com contagem regressiva para o sorteio), **Divertido** (colorido e leve) e **Simples** (direto ao ponto).
- **As cores da sua organização** são aplicadas automaticamente sobre o modelo escolhido, e o sistema **ajusta o contraste** do texto para ficar sempre legível — inclusive colocando a sua logo numa moldura clara para não sumir no fundo.
- O seletor de modelos agora mostra uma **miniatura** de cada um (clique para ampliar), em **Editar campanha → Página pública → Template visual**.
- Novos elementos de engajamento: **contagem regressiva** até o sorteio e um resumo em **cards de fatos** (data, valor do cartão, prêmio, vendidos).

Veja em [Personalizar a página pública](/guias/personalizar-pagina-publica/).

---

## Versão 1.9.0 — Página pública mais envolvente e transparente

Quatro novidades para engajar quem visita a campanha e provar a lisura do sorteio. Cada uma funciona como **bloco** (Gutenberg) e como **shortcode**.

- **Termômetro de meta.** Defina uma meta de **cartões** e/ou de **arrecadação (R$)** e a página passa a exibir um termômetro com o progresso e um aviso de **meta atingida**. Configure na aba **Página pública** da campanha. (A meta em R$ só aparece se você não estiver ocultando os valores financeiros.)
- **Verificação pública do sorteio.** Um painel "Como conferir o sorteio" que qualquer pessoa pode usar para confirmar, no próprio navegador, que o resultado é honesto: o **lacre** é publicado antes, a **semente** é revelada depois, e o cálculo é refeito na hora. Um diferencial de confiança para a sua causa.
- **Vídeos de divulgação.** Cole um link do **YouTube** ou do **Vimeo** e o vídeo aparece embutido na página da campanha. Também dá para anexar um **link de vídeo** como evidência na prestação de contas.
- **Vitrine de campanhas.** Um endereço único (**`/campanhas`**) que lista todas as suas campanhas ativas em cards — ótimo para divulgar tudo de uma vez. Também embutível em qualquer página do seu site pelo bloco/shortcode **Vitrine**.

Veja como usar em [Personalizar a página pública](/guias/personalizar-pagina-publica/) e [Blocos e Shortcodes](/modulos/blocos-shortcodes/).

> **Correção 1.9.1** — ajuste para a **vitrine** carregar corretamente também quando o site usa o formato de links "Padrão" do WordPress.

---

## Versão 1.8.0 — Privacidade, minimização de dados e organização das telas

- **Ferramentas de privacidade (LGPD).** O plugin agora conversa com as ferramentas nativas do WordPress em **Ferramentas → Exportar dados pessoais** e **Apagar dados pessoais**: ao atender a um pedido de um titular por e-mail, o sistema **exporta** o consentimento de comunicações e a situação de contemplado, e **apaga** o consentimento quando solicitado. Os **documentos pessoais do contemplado são mantidos** por obrigação legal de prestação de contas do sorteio. (Os dados de compra ficam a cargo do WooCommerce.)
- **Menos dados guardados.** O campo de **dados bancários** da organização foi **removido** — não era usado em nenhum documento e guardar dado sensível sem necessidade é um risco desnecessário. Ele volta no futuro, junto da funcionalidade de recibos/repasse.
- **Aba renomeada e mais clara.** A antiga aba "Bancário e contato" virou **"Configurações Globais da Campanha"**, reunindo o contato de dúvidas e os padrões de reserva. O campo técnico "TTL" agora se chama **"Tempo de reserva do cartão (minutos)"**, com explicação.
- **Menu mais organizado.** No menu do plugin, **Configurações** passou para depois de **Auditoria**; e a aba **Usuários** ficou logo após **Identidade visual**.

## Versão 1.7.0 — Convide sua equipe e defina papéis

- **Nova aba Usuários, em Configurações.** Agora dá para **atribuir papéis pela tela**, sem depender de configuração técnica. O Administrador da organização abre **Configurações → Usuários**, encontra a pessoa (busca por nome, login ou e-mail) e marca o que ela pode fazer: **Administrador da campanha**, **Auditor** e/ou **Operador**. A alteração é salva na hora e fica registrada na auditoria. Veja [Gerenciar usuários e papéis](/guias/gerenciar-usuarios/).
- **Uma pessoa pode ter mais de um papel.** Os acessos se somam — útil para quem, por exemplo, opera as vendas e também acompanha as contas.
- **Responsáveis pela campanha mais fáceis de achar.** No formulário da campanha, a escolha dos responsáveis subiu para o **topo** da aba **Configurações**. E, com os papéis agora atribuíveis pela tela, a lista de responsáveis deixa de aparecer vazia.

## Versão 1.6.0 — Vários prêmios na mesma campanha

- **1º, 2º, 3º lugar na mesma rifa.** Agora uma campanha pode ter **mais de um prêmio**. Na etapa **Dados do Prêmio**, use **+ Adicionar prêmio** para incluir cada um na ordem em que serão sorteados. Todos são sorteados **da mesma base de cartões vendidos, sem repetir número** — cada prêmio vai para um cartão diferente. O regulamento lista todos os prêmios, o resultado público e os e-mails mostram um ganhador por prêmio, e a prestação de contas soma os custos de todos. Quem quiser um prêmio só não muda nada. Veja [Criar a primeira campanha](/guias/criar-primeira-campanha/) e [Realizar o sorteio](/guias/realizar-sorteio/).

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
