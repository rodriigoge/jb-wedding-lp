# J&B Wedding Landing Page

Landing page responsiva para o site de casamento de Jamila & Bruno.

## Stack

- React.js
- Next.js
- TypeScript
- Vite

## Como rodar

Instale as dependências:

```bash
pnpm install
```

Rode o projeto com Next.js:

```bash
pnpm dev
```

A aplicação ficará disponível em:

```text
http://localhost:3000
```

Também existe uma entrada Vite para desenvolvimento:

```bash
pnpm dev:vite
```

## Seções

- Hero com boas-vindas.
- Contagem regressiva para o casamento.
- Cerimônia.
- Local da Festa com mapa incorporado.
- Lista de Presentes com modal Pix.
- Confirmação de Presença com formulário.

## Assets

Todos os assets usados pela aplicação ficam em `public/assets/`, pois essa é a pasta servida publicamente pelo Next.js.

No código, as imagens são referenciadas com caminhos como `/assets/nome-do-arquivo.webp`.

## Supabase

O formulário de confirmação de presença salva dados na tabela `rsvp_confirmations`.

Variáveis usadas pela landing:

```env
NEXT_PUBLIC_SUPABASE_URL=https://ziyjazqtbxnumvqhlnte.supabase.co
NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=sua-publishable-key
```

O envio público usa apenas a publishable key. A secret key não deve ser usada na landing page.

## Observações

- O site ainda não processa pagamentos.
- O modal de presentes apenas exibe dados Pix e permite copiar a chave.
- O formulário de presença envia os dados para o Supabase.
