# Como colocar o app no seu celular

O app está pronto na pasta `pwa`. Para instalar no celular ele precisa estar publicado em um endereço HTTPS — abrir o arquivo direto não funciona. O GitHub Pages faz isso de graça.

---

## Passo 0 — gerar os ícones (2 minutos, faça uma vez)

1. Abra `gerar-icones.html` no navegador do computador.
2. Clique em **Baixar os 3 ícones**.
3. Mova os três arquivos da pasta Downloads para dentro da pasta `pwa`:
   - `icon-192.png`
   - `icon-512.png`
   - `icon-512-maskable.png`

Sem esses arquivos o app ainda funciona, mas o ícone na tela inicial pode sair genérico.

---

## Passo 1 — criar a conta e o repositório

1. Acesse **github.com** e crie uma conta (se ainda não tiver).
2. Clique no **+** no canto superior direito → **New repository**.
3. Preencha:
   - **Repository name:** `meu-ingles`
   - Marque **Public**
   - Não marque nenhuma das caixas de "Initialize this repository"
4. Clique em **Create repository**.

---

## Passo 2 — enviar os arquivos

1. Na página do repositório recém-criado, clique em **uploading an existing file** (link azul no meio da tela).
2. Arraste para a área de upload **o conteúdo da pasta `pwa`** — os arquivos soltos, não a pasta:
   - `index.html`
   - `manifest.webmanifest`
   - `sw.js`
   - `icon.svg`
   - `icon-192.png`
   - `icon-512.png`
   - `icon-512-maskable.png`
3. Clique em **Commit changes** no fim da página.

---

## Passo 3 — ligar o GitHub Pages

1. No repositório, vá em **Settings** (aba superior) → **Pages** (menu da esquerda).
2. Em **Source**, escolha **Deploy from a branch**.
3. Em **Branch**, selecione **main** e a pasta **/ (root)**. Clique em **Save**.
4. Espere de 1 a 3 minutos e recarregue a página. Vai aparecer o endereço:

   `https://SEU-USUARIO.github.io/meu-ingles/`

---

## Passo 4 — instalar no celular

**Android (Chrome):**

1. Abra o endereço no Chrome.
2. Toque no menu **⋮** → **Adicionar à tela inicial** (ou aparece um aviso "Instalar app").
3. Confirme. O ícone aparece na tela inicial e o app abre em tela cheia.

**iPhone (Safari — precisa ser o Safari):**

1. Abra o endereço no Safari.
2. Toque no botão **compartilhar** (quadrado com seta para cima).
3. Role e toque em **Adicionar à Tela de Início** → **Adicionar**.

Depois de instalado, abra o app uma vez com internet. A partir daí ele funciona offline — no avião, no metrô, sem sinal.

---

## Atualizar o conteúdo depois

Quando quiser adicionar um DECK 5 ou corrigir uma frase:

1. Substitua o `index.html` no GitHub (abra o arquivo → ícone de lápis → cole o novo conteúdo → Commit).
2. Abra `sw.js` e mude `my-english-v1` para `my-english-v2` — isso força o celular a baixar a versão nova.
3. Feche e reabra o app no celular.

---

## Como usar o app

- **Tela inicial:** escolha um deck ou "Todas as 200 frases".
- **Chips no topo:** filtram por categoria dentro do deck.
- **Toque no cartão:** vira e mostra tradução, pronúncia e a estrutura.
- **Deslize para os lados:** próxima ou anterior.
- **Botão 🔊:** lê a frase em inglês.
- **⚙ Configurações:** escolha a voz, a velocidade e ative "falar ao virar".

A voz vem do próprio celular. No Android, vozes melhores em Configurações → Idiomas → Saída de conversão de texto em voz → instalar o pacote de inglês. No iPhone, Ajustes → Acessibilidade → Conteúdo Falado → Vozes → English.
