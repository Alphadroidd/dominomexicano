# 🎲 Dominó Mexicano PWA

App de placar em tempo real para Dominó Mexicano (dupla-12).

## Arquivos
- `index.html` — App principal
- `logo.svg` — Ícone PWA (512×512, escalável)
- `manifest.json` — Manifesto PWA
- `sw.js` — Service worker (suporte offline)

## Como hospedar

### Opção 1 — Netlify Drop (mais fácil)
1. Acesse https://app.netlify.com/drop
2. Arraste esta pasta inteira
3. Pronto — link compartilhável gerado!

### Opção 2 — Firebase Hosting
```bash
npm install -g firebase-tools
firebase login
firebase init hosting
firebase deploy
```

### Opção 3 — GitHub Pages
1. Crie um repositório público
2. Faça upload dos arquivos
3. Ative GitHub Pages nas configurações

## Firebase Realtime Database
O app já está configurado com o banco:
`https://domino-mexicano-74864-default-rtdb.firebaseio.com`

Regras necessárias (Firebase Console → Realtime Database → Regras):
```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
```

## Funcionalidades
- ✅ Ranking em tempo real (todos os celulares sincronizados)
- ✅ Seletor visual de peças com pips coloridos por número
- ✅ 13 rodadas com histórico completo
- ✅ Edição de rodadas (botão ✏️)
- ✅ Link compartilhável por partida
- ✅ Histórico de partidas finalizadas
- ✅ Instalável como app (PWA)
