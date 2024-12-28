## Structure
```
apps/
  web/     // Web application-specific files
    components/    // Reusable UI components
    pages/         // Next.js pages
    lib: utils, hooks...
    styles/        // TailwindCSS base styles or custom CSS modules
    modules: components, utils, hooks, types, views
          // Domain-specific features (e.g., authentication, dashboard)
```
### Modules

- Feature or domain-specific logic and views.
- Typical Structure:

```
modules/
  feature-name/
    views/          // Main container components (feature-specific pages or screens)
      FeatureView.tsx
    components/     // Feature-specific components (optional)
      FeatureButton.tsx
    hooks/          // Feature-specific hooks (optional)
      useFeatureData.ts
    utils/          // Utility functions specific to the feature (optional)
      featureHelper.ts
    types.ts        // Types and interfaces specific to the feature (optional)
```

- Example:

```
modules/chatbot/
  views/
    ChatBoxView.tsx
  components/
    ChatBubble.tsx
  hooks/
    useChat.ts
  utils/
    chatbotHelper.ts
  types.ts
```

### Components

- Reusable, shareable UI components across the application
- Typical Structure:

```
components/
  [category]/
    ComponentName.tsx
    index.ts          // Barrel file to streamline imports
```

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.


