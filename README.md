# ApexPulse AI

A mobile-first Expo / React Native starter for AI-assisted market analysis across Forex, cryptocurrency, stocks, and indices.

## Source package

The complete original Expo source archive is committed at [source/ApexPulseAI-Expo-Project.zip](source/ApexPulseAI-Expo-Project.zip). It contains the original `App.tsx`, app configuration, package manifest, environment template, and project documentation.

To restore the original app source, download and extract that ZIP. The archive expands into an `ApexPulseAI/` directory.

## Features

- Dark, orange-accented mobile interface.
- Dashboard, Watchlist, Analyze, History, and Profile tabs.
- Instrument selection and sample candlestick chart.
- Screenshot selection from the device photo library.
- Demo signal cards with directional bias, confidence, entry zone, stop loss, take profits, support, and resistance.
- Onboarding for trading experience, preferred markets, and risk preference.

## Tech stack

- Expo SDK 54
- React 19
- React Native 0.81
- TypeScript
- expo-image-picker
- react-native-svg
- react-native-safe-area-context

## Run locally

After extracting the source archive:

1. Install Node.js (LTS).
2. Change into the extracted `ApexPulseAI` directory.
3. Install dependencies: `npm install`
4. Start Expo: `npx expo start`
5. Scan the QR code with Expo Go, or press `a` / `i` to launch an available simulator.

## Current implementation status

| Area | Status |
| --- | --- |
| Mobile UI and navigation | Implemented |
| Market data | SAMPLE / simulated only |
| Chart screenshot selection | Implemented |
| AI analysis | Demo response only; provider not connected |
| Authentication | Local UI demonstration only |
| Broker connection / order execution | Not implemented |

**Important:** Displayed market prices and signals are sample values. The app does not currently connect to a live market-data provider, does not perform a real GPT 5.6 Terra inference, and does not execute trades.

## GPT 5.6 Terra integration

The intended AI provider is GPT 5.6 Terra. The provider endpoint, authentication scheme, model identifier, and image-input format must be verified against the provider's actual documentation before integration.

Keep provider credentials on a server. Do not place API keys in the Expo application or commit real secrets. See [server integration contract](server/README.md) and use `.env.example` only as a template.

## Risk notice

Predictions are probabilistic analysis, not guaranteed outcomes or financial advice. Sample values are illustrative only. Always independently verify market information and risk before making trading decisions.
