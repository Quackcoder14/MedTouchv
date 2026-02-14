# MedTouch.ai - AI Triage System

AI-powered emergency department triage system with multi-step patient intake.

## 🚀 Quick Start

### Local Development

```bash
# Install dependencies
npm install

# Run development server
npm run dev
```

Open [http://localhost:3000](http://localhost:3000)

## 📦 Deploy to Vercel

### Option 1: Deploy via Vercel Dashboard

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Click "Deploy"

### Option 2: Deploy via Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

Follow the prompts:
- Set up and deploy? **Y**
- Which scope? Select your account
- Link to existing project? **N**
- What's your project's name? **medtouch-ai**
- In which directory is your code? **./**
- Want to override settings? **N**

## 🔧 Environment Setup

No environment variables required - the app uses a built-in rule-based prediction system.

## 📁 Project Structure

```
medtouch-ai-triage/
├── app/
│   ├── api/
│   │   └── predict/
│   │       └── route.ts          # AI prediction API
│   ├── page.tsx                  # Main page with stepper
│   ├── StepVitals.tsx           # Step 1: Vitals input
│   ├── StepSymptoms.tsx         # Step 2: Symptoms selection
│   ├── StepHistory.tsx          # Step 3: Medical history
│   ├── StepReview.tsx           # Step 4: Results & analysis
│   ├── Stepper.tsx              # Progress indicator
│   ├── layout.tsx               # Root layout
│   └── globals.css              # Global styles
├── package.json
├── tsconfig.json
├── tailwind.config.ts
└── next.config.mjs
```

## 🎨 Features

- ✅ Multi-step patient intake (Vitals → Symptoms → History → Review)
- ✅ AI-powered risk classification (High/Medium/Low)
- ✅ Department recommendation
- ✅ Clinical recommendations based on risk level
- ✅ Explainability layer (contributing factors)
- ✅ Professional medical UI
- ✅ Fully responsive design
- ✅ TypeScript + Tailwind CSS

## 🏥 How It Works

### Step 1: Vitals
- Patient age, gender
- Blood pressure (systolic & diastolic)
- Heart rate
- Temperature

### Step 2: Symptoms
- Multi-select from 18 common symptoms
- Includes critical symptoms (chest pain, difficulty breathing, etc.)

### Step 3: Medical History
- Pre-existing conditions
- 13 condition categories

### Step 4: Review & Results
- AI risk classification with confidence score
- Department recommendation
- Clinical recommendations (ESI level-based)
- Contributing factors explanation
- Complete patient summary

## 🤖 AI Prediction System

The app uses a rule-based clinical decision system that evaluates:

1. **Age factors** - Elderly patients have higher baseline risk
2. **Vital signs** - BP, HR, Temperature thresholds
3. **Symptom severity** - Critical vs. routine symptoms
4. **Medical history** - High-risk conditions
5. **Combined score** - Weighted risk assessment

## 📊 Risk Classification

- **High Risk** (ESI 1): Immediate resuscitation needed
- **Medium Risk** (ESI 2-3): Urgent assessment required
- **Low Risk** (ESI 4-5): Routine processing

## 🔐 Security & Privacy

- No patient data is stored
- All processing happens in-memory
- HIPAA-compliant design principles
- For demonstration purposes only

## ⚕️ Medical Disclaimer

This tool is for demonstration and educational purposes only. It should NOT be used for actual medical decision-making. All medical decisions must be made by qualified healthcare professionals based on complete clinical assessment.

## 📝 License

© 2026 MedTouch.ai - Hackathon Edition

## 🛠️ Tech Stack

- **Framework**: Next.js 14
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Deployment**: Vercel
- **API**: Next.js API Routes

## 🎯 Deployment Checklist

- [x] All TypeScript files created
- [x] Tailwind CSS configured
- [x] API route implemented
- [x] Multi-step flow working
- [x] Responsive design
- [x] Professional UI
- [x] Ready for Vercel deployment

## 🚀 Deploy Now

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/yourusername/medtouch-ai)

---

**Built for healthcare innovation hackathon 2026** 🏥
