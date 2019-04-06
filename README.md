# 초간단 쿠버네티스 문서 한글화 시작 가이드

참고 : https://kubernetes.io/ko/docs/contribute/

## 1. CNCF 가입 및 CLA 서명

### 1-1. Individual 로 가입

- 위치 : https://identity.linuxfoundation.org/

> 주의사항 : Github과 동일한 이메일 계정으로 가입해야 합니다.

### 1-2. Contributor License Agreement (CLA) 서명
- 위치 : https://github.com/kubernetes/community/blob/master/CLA.md#how-do-i-sign

### 1-3. Kubernetes Slack 가입
- http://slack.k8s.io/
- #kubernetes-docs-ko 채널 참여

## 2. 일감 찾기

### 2-1. 한글화되지 않은 일감 찾기

- 위치 : https://kubernetes.io/ko/docs/

제목에 `(EN)`으로 되어 있는 것중, 번역할 일감 찾기

### 2-2. Github 이슈 등록

### 2-2-1. Github 이슈 등록
- 위치 : https://github.com/kubernetes/website/issues

### 2-2-2. Fork
- Fork 버튼 클릭
- (필요시) 내 repo에서 default branch 설정 : 현재 작업중인 ko 브랜치로

### 2-3. git clone
- 로컬PC에 git clone
```sh
git clone https://github.com/uncle-elephant/website.git
```

## 3. 한글화 번역 시작

### 3-1. Atom 에디터 설치
- https://atom.io/
- 추가 플러그인 설치 : language-mediawiki

### 3-2. 필요한 위치에 파일 생성
- 예 : content/ko/docs/concepts/overview/working-with-objects/`annotations.md`

### 3-3. 번역 시작
- 용어집 : https://docs.google.com/spreadsheets/d/1BWKq_HYmt_p1RKzQJoPfCb4ZgBgxH_q3_mf9ujCmniw/edit

필요시 용어 등록(제일 하단)


### 3-4. 커밋 & 푸시
```sh
git config --global user.email "jesang.myung2@gmail.com"
git config --global user.name "jmyung2"
git add .
git commit -m "Translate concepts/overview/working-with-objects/annotations in Korean"
git push
```

되도록 하나의 커밋으로 만들어줍니다.

## 4. Pull Request
- CLA 서명 안돼있는 경우, 거절됨
- (필요시) 리뷰어 의견 추가 반영

## 5. 이슈 닫기

### 참고 사이트

- https://kubernetes.io/docs/contribute/start/#sign-the-cla
- https://github.com/kubernetes-retired/kubernetes-docs-ko/issues/2
- https://github.com/kubernetes/website/blob/master/README-ko.md?fbclid=IwAR1CRXCAeaMGU0Jz13JUYT1jp6bx-5YIvuR4yI1yS2atLoj21MEfc2LDa6E
- https://kubernetes.io/ko/docs/contribute/localization_ko/
