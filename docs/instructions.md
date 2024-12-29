# Project Overview
You are building a mobile and web application about family medical record management called "FunLifeCare". This MVP version focuses on helping users manage their family's health records and make informed dietary decisions.
You will be using Turbo for build orchestration, Next.js (web), React Native (mobile), TailwindCSS, TypeScript, React, and other tools.

# Core functionalities

1. Family Member Medical Record Management
   - Add new family members to the system
   - Create, edit, and delete medical records for each family member
   - Organize records by categories (medications, diagnoses, lab results, etc.)
   - View medical history timeline for each family member

2. Document Processing and Storage
   - Upload medical documents via image capture or file upload
   - Extract key information from medical documents using OCR
   - Automatically categorize and store extracted information
   - Maintain a searchable archive of all uploaded documents

3. Smart Food Scanner and Advisor
   - Scan food items using device camera
   - Analyze ingredients list from scanned products
   - Cross-reference ingredients with family members' medical histories
   - Provide personalized recommendations and warnings based on medical conditions
   - Display alternative food suggestions when necessary

# User flow

1. Medical Record Management Flow:
   - User logs in → Selects family member → Views/Edits medical records
   - Add new record → Choose record type → Fill details/Upload documents
   - View timeline → Filter by date/category → Access detailed records

2. Document Processing Flow:
   - Select family member → Choose document upload
   - Take photo/Select file → Preview → Confirm
   - Review extracted information → Edit if needed → Save
   - Access saved records through member's profile

3. Food Scanner Flow:
   - Select family member → Access scanner
   - Scan food item → View ingredients analysis
   - See recommendations → View alternatives if warnings present
   - Save food preferences/restrictions

# Doc
## Documentation of how to add new page or new view for a feature

### Example code



### Example Prompt
```
Help me add a new page to the mobile application, using the code example from @instructions
```


# Current file structure
```
├── apps/
│   └── web/          # Next.js web application
│   └── mobile/          # React Native mobile application
├── packages/
│   ├── ui/           # Shared React component library
│   ├── lib/          # Shared utility functions
│   ├── eslint-config/# Shared ESLint configurations
│   └── typescript-config/ # Shared TypeScript configurations
```

- `apps/web`: FunLifeCare app
- `apps/mobile`: FunLifeCare app
- `packages/ui`: a stub React component library shared by both `web` and `mobile` applications
- `packages/eslint-config`: `eslint` configurations (includes `eslint-config-next` and `eslint-config-prettier`)
- `packages/typescript-config`: `tsconfig.json`s used throughout the monorepo
- `packages/lib`: A library of utility functions shared across the monorepo