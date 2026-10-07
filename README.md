# Prognexo — site comercial

Página estática de apresentação da visão Full, com glassmorphism, identidade Prognexo, imagem institucional do painel, comparação de planos e simulador de contribuição. Publicar a raiz do repositório; não há build ou dependências.

## Conexões preservadas

- Login: `https://app.prognexo.com.br/#/login`
- Cadastro: `https://app.prognexo.com.br/#/cadastro`
- Assinatura existente: `https://app.prognexo.com.br/#/meu-plano?modulo=vendas&periodicidade=mensal`
- Comercial: `https://wa.me/554430472098`
- Termos e privacidade: `/termos.html` e `/privacidade.html`

O formulário valida nome, clínica, e-mail e autorização; abre o WhatsApp com o diagnóstico preenchido. O visitante revisa e confirma o envio no WhatsApp. Se o navegador bloquear a aba, um link alternativo fica disponível. O site não registra dados, não envia mensagens automaticamente e não realiza cobranças.

Os planos Full são propostas sujeitas à validação e disponibilidade. O link da assinatura acessa a operação atual; não atribui planos Full nem altera preços no backend.

WhatsApp Cloud API, pagamentos, automações e webhooks do produto ficam no frontend/backend do Prognexo. Seus nomes nesta landing não representam novas implementações dessas integrações.

## Verificação desta atualização

- JavaScript validado com `node --check app.js`.
- Assets, páginas legais e links internos verificados.
- Abas, planos, simulador e composição da mensagem de WhatsApp verificados em execução JavaScript isolada, sem enviar mensagem.
- Aplicativo público respondeu HTTP 200; seu bundle contém as rotas de cadastro e assinatura, com login no fallback público.
- A execução em navegador não foi concluída: o download do navegador de teste falhou neste ambiente.
- Pagamento real, entrega da mensagem comercial, autenticação e webhooks internos não foram exercitados.

Manter as páginas legais existentes ao atualizar a landing. Não incluir credenciais ou dados clínicos neste repositório público.
