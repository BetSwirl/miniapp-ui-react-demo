# BetSwirl UI React Demo

This Next.js demo shows how to bootstrap a Farcaster Mini App casino experience with **@betswirl/ui-react**, MiniKit, and OnchainKit so you can launch a fully themed dApp in minutes.

## 🎮 Live Demo

The public demo is coming soon.

## 📚 Documentation

Read the full guide: [https://docs.betswirl.com/developer-hub/demos/ui-react/miniapp](https://docs.betswirl.com/developer-hub/demos/ui-react/miniapp)

## 🚀 Installation

```bash
npm install
# or
yarn install
# or
pnpm install
# or
bun install
```

## ▶️ Run the app

```bash
npm run dev
```

The UI will be available at `http://localhost:3000`.

## ⚙️ Environment variables

Create a `.env.local` file at the project root and fill the variables below. They are generated when running `npx create-onchain --mini`, and you can regenerate the Farcaster account association via `npx create-onchain --manifest`.

### OnchainKit / MiniKit configuration

```bash
NEXT_PUBLIC_APP_PROJECT_NAME=
NEXT_PUBLIC_URL=
```

### Farcaster & Mini App metadata

```bash
FARCASTER_HEADER=
FARCASTER_PAYLOAD=
FARCASTER_SIGNATURE=
NEXT_PUBLIC_APP_ICON=
NEXT_PUBLIC_APP_SUBTITLE=
NEXT_PUBLIC_APP_DESCRIPTION=
NEXT_PUBLIC_APP_SPLASH_IMAGE=
NEXT_PUBLIC_SPLASH_BACKGROUND_COLOR=
NEXT_PUBLIC_APP_PRIMARY_CATEGORY=
NEXT_PUBLIC_APP_HERO_IMAGE=
NEXT_PUBLIC_APP_TAGLINE=
NEXT_PUBLIC_APP_OG_TITLE=
NEXT_PUBLIC_APP_OG_DESCRIPTION=
NEXT_PUBLIC_APP_OG_IMAGE=
```

### Affiliate address (optional)

```bash
NEXT_PUBLIC_AFFILIATE_ADDRESS=
```

### Custom RPCs (optional)

```bash
NEXT_PUBLIC_BASE_RPC_URL=
NEXT_PUBLIC_ARBITRUM_RPC_URL=
NEXT_PUBLIC_BSC_RPC_URL=
```

## 📦 Packages used

- **@betswirl/ui-react** React UI library to quickly integrate BetSwirl games into your application
- **@coinbase/onchainkit** Wallet connection + Farcaster integration
- **next** React framework

## ✨ Key features

- `.well-known/farcaster.json` ready for metadata and account association
- Mini App metadata automatically injected from `layout.tsx`
- Fully customizable theme via `gameProps` with dedicated backgrounds
- Token picker, balance management, freebets, and multichain support (Base, Arbitrum, BSC)
- `MiniKitProvider` (in `providers.tsx`) wires up wagmi connectors, Mini App context, and safe-area insets

## 🔧 Quick customization

1. Build your own Mini APp: edit `page.tsx`, tweak `gameProps`, and adjust the MiniKit config.
2. Publish your Mini App: cast it, associate it to your account, and share it with your community.

## 🔗 Useful links

- [BetSwirl Docs](https://docs.betswirl.com)
- [MiniKit Documentation](https://docs.base.org/builderkits/minikit/overview)
- [OnchainKit Documentation](https://docs.base.org/builderkits/onchainkit/getting-started)
- [Next.js Documentation](https://nextjs.org/docs)
