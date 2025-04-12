## Hi there 👋

# Story IP - AI 모델 파인튜닝 플랫폼

## 🎯 프로젝트 개요
Story IP는 창작자의 콘텐츠(이미지)를 활용하여 AI 모델을 파인튜닝하고, 이를 통해 생성된 모델의 IP를 보호하고 수익을 창출할 수 있는 플랫폼입니다.

## 🛠️ 기술 스택
- Frontend: Next.js, React, Material-UI, wagmi
- Backend: Node.js, Express, Firebase
- AI: PyTorch, diffusers, transformers
- Storage: Pinata IPFS
- Blockchain: Story Protocol

## 📋 주요 기능
1. 이미지 업로드 및 IPFS 저장
2. Firebase를 통한 파인튜닝 요청 관리
3. Google Colab에서의 실시간 파인튜닝 처리
4. 파인튜닝된 모델을 활용한 이미지 생성
5. 생성된 이미지의 IPFS 저장 및 Firebase 업데이트

## 🚀 시작하기

### 1. 환경 설정
프로젝트 루트에 `.env` 파일을 생성하고 다음 내용을 입력하세요:

```env
# Firebase 설정
FIREBASE_DATABASE_URL=

# Pinata 설정
PINATA_API_KEY=
PINATA_API_SECRET=
PINATA_JWT=

# API 설정
NEXT_PUBLIC_API_URL=http://localhost:3001
```

### 2. 패키지 설치
```bash
# 백엔드 패키지 설치
cd backend
npm install

# 프론트엔드 패키지 설치
cd ../frontend
npm install
```

### 3. 서버 실행
```bash
# 백엔드 서버 실행
cd backend
npm run dev

# 프론트엔드 서버 실행 (새 터미널에서)
cd frontend
npm run dev
```

## 🔄 파인튜닝 프로세스
1. 사용자가 이미지를 업로드하고 파인튜닝 요청
2. Firebase에 요청 내역 저장
3. Colab에서 Firebase 실시간 폴링
4. Pinata에서 이미지 다운로드
5. 이미지 기반 파인튜닝 실행
6. 파인튜닝된 모델로 이미지 생성
7. 생성된 이미지를 Pinata에 업로드
8. Firebase에 결과 업데이트

## 📝 주의사항
- `.env` 파일은 절대 깃헙에 커밋하지 마세요
- API 키는 안전하게 보관하세요
- 실제 배포 시에는 환경 변수를 적절히 설정해주세요
