# Vperts Multi WG — canal de download

Este repositório existe **só para distribuir os instaladores** do Vperts Multi WG e
alimentar o auto-update do app. Não há código-fonte aqui — ele fica em repositório
privado.

## Baixar

Sempre a versão mais recente, link fixo:

**[VpertsMultiWG-Setup.exe](https://github.com/ekooll/vperts-multi-wg-releases/releases/latest/download/VpertsMultiWG-Setup.exe)**

Duplo-clique instala e abre. Instala para o usuário, sem pedir admin.

## O que é o app

Ferramenta multi-conta para o [Poke Web Games](https://pokewg.com) — mostra num card o
que o jogo já mostra: HP e nível do pokémon, bolas, poções, derrotados, capturas, shiny e
profit da sessão.

**A ferramenta apenas lê, soma e exibe. Não automatiza nada** — quem joga é você. O
limite de 2 contas foi acordado com os desenvolvedores do jogo.

## Auto-update

O app checa este repositório e se atualiza sozinho. Se você tem uma versão instalada de
um canal antigo (`ekooll/vperts-multi-wg`), ela **não** migra sozinha: o canal fica
gravado dentro do `.exe`. Instale uma vez pelo link acima e a partir daí as atualizações
chegam automaticamente.

## Releases

Cada release traz 4 arquivos:

| arquivo | para quê |
|---|---|
| `VpertsMultiWG-Setup-<versão>.exe` | instalador versionado |
| `VpertsMultiWG-Setup.exe` | cópia de nome fixo, para o link acima não quebrar a cada versão |
| `latest.yml` | **obrigatório** — é o que o auto-update lê para achar versão nova |
| `.blockmap` | download diferencial da atualização |
