## Hi there 👋

# Storytuning - AI Model Fine-tuning Platform

## 🎯 Project Overview
Storytuning is a platform that empowers creators to own and monetize AI models through content-based fine-tuning. It addresses the critical issue of intellectual property rights in the age of generative AI by allowing creators to maintain control over their style, content, and the AI models trained on them.

## 🛠️ Tech Stack
- Frontend: Next.js, React, Material-UI, wagmi
- Backend: Node.js, Express, Firebase
- AI: PyTorch, diffusers, transformers
- Storage: Pinata IPFS
- Blockchain: Story Protocol

## 📋 Key Features
1. Content Ownership: Creators fully own their fine-tuned models
2. IP Registration: Models can be registered as IP on-chain using Story Protocol
3. Licensing System: Users must purchase license tokens to use models
4. Royalty Distribution: Automatic revenue split (60% creator, 30% platform, 10% AI infrastructure)
5. Image Upload and IPFS Storage
6. Real-time Fine-tuning Processing via Google Colab
7. Image Generation using Fine-tuned Models

## 🚀 Getting Started

### 1. Environment Setup
Create a `.env` file in the project root with the following content:

```env
# Firebase Configuration
FIREBASE_DATABASE_URL=

# Pinata Configuration
PINATA_API_KEY=
PINATA_API_SECRET=
PINATA_JWT=

# API Configuration
NEXT_PUBLIC_API_URL=http://localhost:3001
```

### 2. Package Installation
```bash
# Install Backend Packages
cd backend
npm install

# Install Frontend Packages
cd ../frontend
npm install
```

### 3. Server Start
```bash
# Start Backend Server
cd backend
npm run dev

# Start Frontend Server (in a new terminal)
cd frontend
npm run dev
```

## 🔄 Fine-tuning Process
1. Creator uploads images to the platform
2. Images are registered as IP using Story Protocol
3. Creator selects images and requests fine-tuning
4. Model is trained via Colab-based pipeline
5. Fine-tuned model is published to the platform
6. Users can browse and purchase license tokens
7. Revenue is automatically distributed to all parties

## 📝 Important Notes
- Never commit `.env` file to GitHub
- Keep API keys secure
- Configure environment variables appropriately for production deployment

## 🗺️ Roadmap
1. Phase 1: Launch MVP and test revenue logic with real users
2. Phase 2: Automate fine-tuning backend and scale infrastructure
3. Phase 3: Improve model quality and study base model training data
4. Phase 4: Collaborate with AI infrastructure providers for high-performance models
