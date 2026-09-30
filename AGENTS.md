# Instruções do projeto de documentação

## Sobre este projeto

- Central de ajuda do CRM da Atto Corp, publicada com [Mintlify](https://mintlify.com)
- Público: cliente que usa o CRM no dia a dia (dono de negócio, atendente, vendedor, gestor). Não é desenvolvedor
- Páginas são arquivos MDX com frontmatter YAML (`title`, `description`)
- Menu e configuração ficam em `docs.json`
- Idioma: português do Brasil
- Prévia local exige Node LTS: `PATH=/opt/homebrew/opt/node@22/bin:$PATH mint dev`

## Fonte da verdade

- Código do CRM: repositório `atto-corp-crm`, branch `origin/main`
- Documente apenas o que existe na tela. Se o código não confirma, não escreva
- Nomes de menu, botão e campo devem ser idênticos aos da tela
- Texto da tela vem de `src/i18n/locales/pt-BR/*.json`. A tradução vence o texto reserva escrito no código

## Terminologia

- "conversas", nunca "créditos" nem "tokens"
- "Pipeline" para o funil de vendas (nome do menu)
- "etapa" no texto corrido para coluna do Pipeline. A tela mistura "Estágio" e "Etapa"; em negrito, repetir o rótulo exato da tela
- "lead" ou "contato" para a pessoa atendida
- "canal" para cada número de WhatsApp ou conta de Instagram conectada
- "Agente IA" (nome do menu) para o atendente automático; "Assistente IA" para o chat de ajuda interno
- Planos: Start, Prime, Ultra

## Estilo

- Trate o leitor por "você"
- Frases curtas, uma ideia por frase
- Sem jargão técnico: nada de API, webhook, banco de dados, token, endpoint
- Títulos em minúsculas, só a primeira letra maiúscula
- Negrito para elemento de tela: clique em **Salvar**
- Passo a passo numerado com o componente `<Steps>`
- Avisos com `<Note>`, `<Tip>` e `<Warning>`

## Limites de conteúdo

- Não documentar telas de administrador da Atto: Banco de Dados, Usuários, Logs
- Não citar preço. Para valores, apontar para https://attocorp.com/#planos
- Nunca usar dado real de cliente: nome, telefone, conversa, empresa
- Não citar fornecedores internos nem nomes de tecnologia por trás do produto
