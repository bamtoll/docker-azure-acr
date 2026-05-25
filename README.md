# Docker + GitHub Actions + Azure ACR 자동 배포

GitHub Actions를 통해 Docker 이미지를 빌드하고 Azure Container Registry(ACR)에 push한 후, Azure App Service에 자동 배포하는 CI/CD 파이프라인입니다.

## 🛠️ 기술 스택

- **언어**: Node.js (Express)
- **컨테이너**: Docker
- **CI/CD**: GitHub Actions
- **레지스트리**: Azure Container Registry (ACR)
- **클라우드**: Azure App Service

## 📁 프로젝트 구조

```
├── app.js
├── package.json
├── Dockerfile
└── .github/
    └── workflows/
        └── docker-build.yml
```

## 🚀 CI/CD 파이프라인

main 브랜치에 push 시 자동으로 아래 과정이 실행됩니다.

1. 소스코드 체크아웃
2. Azure Container Registry 로그인
3. Docker 이미지 빌드 & ACR push
4. Azure App Service 자동 배포

## 📦 ACR 이미지

bamtollacr.azurecr.io/my-docker-app:latest

## 🌐 배포 URL

https://bamtoll-acr-app-a5bphce7ewcgevaq.koreacentral-01.azurewebsites.net

## 📸 실행 결과

![서비스 화면](./service.png)
