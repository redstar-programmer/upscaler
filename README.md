# redstar upscaler

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>ffmpeg, realesrgan, flowframes 기반의 동영상 업스케일링 툴</strong><br>
  <em>최신 GUI 기반, 프리셋 설정, 다중 파일 처리 지원</em>
</p>

---

다운로드 : [Release](https://github.com/redstarupscaler/upscaler/releases)

## ✨ redstar' upscaler를 후원해 주세요

이 프로젝트가 마음에 드시거나 개발을 응원하고 싶으신가요?  
작은 후원으로 더 나은 기능과 안정적인 업데이트를 도와주세요!  

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)  
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 서버 비용, 개발 시간, 커피 한 잔의 후원이 큰 힘이 됩니다. 감사합니다!

## Table of Contents

- [👋 소개](#소개)  
- [💾 설치 및 준비사항](#설치-및-준비사항)  
- [🔧 주요 기능](#주요-기능)  
- [🚀 사용 방법 (Quick Start)](#사용-방법-quick-start)  
- [⚙️ 상세 기능 설명](#상세-기능-설명)  
- [🙏 감사의 글](#감사의-글)  
- [📜 History](#history)

## 👋 소개
**redstar upscaler**는 `ffmpeg`, `Real-ESRGAN`, `Flowframes`를 이용하여 동영상을 자동으로 고해상도로 업스케일링하는 Python 기반의 GUI 도구입니다. 

- 영상 프레임 추출 → 업스케일링 → 영상 병합까지 한 번에 처리
- 다양한 realesrgan 모델 지원
- Flowframes를 통한 보간(Optional)
- 오디오 코덱 자동 추출 및 처리
- 원본 위치 또는 지정 경로에 작업 가능

> ⚠️ Windows 환경에서 개발 및 테스트되었습니다.

아래는 간단한 사용 데모화면입니다.<br>
[![미디어1](https://github.com/user-attachments/assets/ba601a08-6749-45fd-ae21-f1a2a52987f6)

## 💾 설치 및 준비사항

1. 다음 외부 도구 설치 및 위치 확인(단, 배포 파일에 ffmpeg, Real-ESRGAN 및 Flowframes 설치파일 포함되어 있음(경로 내 Programs 폴더 참조))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(선택)*
2. 압축 해제 후 readstar's upscaler.exe 실행

## 🔧 주요 기능

- ✅ 영상 다중 선택 및 순차 작업
- ✅ 프리셋 저장 및 자동 적용
- ✅ 오디오 코덱 자동 감지 및 비트레이트 설정
- ✅ realesrgan 모델 자동 탐지 및 선택
- ✅ 작업 완료 후 결과물 자동 정리 ([REDSTAR] 접두어 부여)
- ✅ 변경된 UI

## 🚀 사용 방법 (Quick Start)

1. 영상 파일 추가 (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV 지원)
2. 작업 위치 지정 또는 "원본파일 경로 사용" 체크
3. 추가된 영상에서 "설정" 버튼 클릭
4. ffmpeg, realESRGAN, Flowframes 상세 설정
5. 전체 파일에 일괄 적용 / 선택한 파일에만 적용 클릭
6. 작업확인 버튼 클릭
7. 실행할 명령어 확인 후 작업 시작 버튼 클릭

> ✨ 작업 결과는 업스케일링 된 영상 및 프레임 보간 된 영상 파일 두개가 선택한 폴더에 생성됩니다.
> ✨ 작업이 완료된 파일은 접두사 [REDSTAR]를 붙인 파일명으로 저장됩니다
---

## ⚙️ 상세 기능 설명

| 항목 | 설명 |
|------|------|
| **작업 경로 설정** | 기본 지정 경로 또는 "원본 파일 경로 사용" 옵션 제공 |
| **영상 포맷 지원** | MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV 등 대부분의 형식 지원 |
| **업스케일 모델** | realesr-animevideov3, realesr-general, 4xplus 등 자동 탐지 |
| **오디오 처리** | `aac`, `mp3`, `flac` 등 다양한 포맷 인코딩 지원 |
| **Flowframes 연동** | 보간 (FPS ×2, ×4, ×8) 설정 가능 |
| **디스크 절약 모드** | 중간 이미지 자동 삭제 기능 제공 |

## 🙏 감사의 글

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes by [n00mkrad](https://github.com/n00mkrad/flowframes)
- 이 프로젝트에 참여하거나 기능을 제안하고 싶으시다면 [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues)에 의견을 남겨주세요.

# 📜 History

v 1.0.0
 > 1. 전체 코드 재 작성
 > 2. UI 변경
 > 3. 처리 가능한 영상/오디오 범위 증가
 > 4. 디스크 절약모드 추가
 > 5. 주요 프로그램을 포함한 배포

v 0.1.92
 > 1. Flowframes 경로 변경 시 AI모델 콤보박스에 중복 입력되어 보간 실패하는 문제 해결
 > 2. 보간 작업 시 콤보박스의 선택 상태 확인코드 추가

v 0.1.91
 > 1. Flowframes 관련 일부 combobox refresh 기능 추가
 > 2. 배포파일 일부 조정

v 0.1.9
 > 1. Flowframes 모델 변경 적용
 > 2. Flowframes 1.36.0 신규 모델, 1.40.0 모델 구현
 > 3. 이제 더 이상 Flowframes 명령줄 실패가 발생하지 않음
 > 4. 드래그/드랍으로 파일 추가 가능
 > 5. Flowframes 설정값 적용되지 않는 문제 해결

v 0.1.8
 > 1. 버전 체크 시 신규 버전 확인 오류 수정
 > 2. flowframes가 기본 경로에 설치되었을 경우(ex. C:\Users\Administrator\AppData\Local\Flowframes\) 해당 경로를 기본으로 설정 후 시작
 > 3. 여러개 파일 선택 추가 시 오류로 인해 강제 종료되는 문제 
 > 4. 다중 파일을 추가한 후 작업 시작 시 오류 발생하는 부분 수정

v 0.1.7
 > 1. 프로그램 크기 변경 가능
 > 2. 음성이 없는 파일 작업 시 오류 발생하는 문제 해결
 > 3. 전체 UI 구성 변경(크기 변경에 맞게 재 구성함)

v 0.1.6
 > 1. 화면 해상도에 따라 글자 크기가 다른 문제 해결
 > 2. 프로그램 타이틀에 버전 정보가 신규 버전으로 보이지 않는 문제 해결
 > 3. config.ini파일이 다른 경로에 저장되는 문제 해결
 > 4. realesrgan 업스케일링 배수 변경 시 업스케일링 모델 콤보박스도 같이 변경
 > 5. 업데이트 체크 기능 추가
 > 6. 일부 로직 수정
 > 7. 해상도 및 fps등 테이블 표기 컬러 변경
 > 8. 해상도(전) 사용자 수정 가능(반드시 1024x768 형태로 입력해야 함)

v 0.1.5
 > 1. flowframes 보간 ai 선택 시 ai 모델이 자동 변경되지 않는 문제 해결
 > 2. flowframes 보간 시 선택된 옵션대로 보간되지 않는 문제 해결
 > 3. 일부 동영상의 FPS 계산 시 잘못된 FPS로 계산되는 경우를 방지하기 위해 "FPS 계산방식" 콤보박스 추가
        -> r_frame_rate / avg_frame_rate 중 선택 가능하며, 기본은 r_frame_rate로 계산합니다
 > 4. 동영상 파일을 선택했을 때 동영상 정보 가져오는 진행 현황을 표기 
 > 5. 파일 연 후 다시 파일 선택 시 마지막 선택한 폴더를 기본으로 열도록 변경

v 0.1.4
 > 1. config.ini 파일 읽기 방식 변경
 > 2. 동영상 정보 가저오는 방식을 파이썬 AV에서 ffmpeg로 변경
 > 3. 작업 종료 시 윈도우 종료기능 추가
 > 4. 작업 리스트에서 마우스 오버 시 전체 파일명을 툴팁으로 표시
 > 5. 작업 리스트에 각 파일별 해상도(전) / 해상도(후) / FPS(전) / FPS(후) 표기
 > 6. FPS 입력 상자 제거(위 각 파일별 표기로 인한 제거)
 > 7. 출력 FPS 예상 크기 제거(위 각 파일별 표기로 인한 제거)
 > 8. 진행 상태를 전체파일/작업별 두개의 Progressbar로 표기

v 0.1.3
 > 1. 파일 불러올 때 일부 FPS 정보가 틀린 파일 FPS 계산 오류 수정

v 0.1.2
 > 1. UI 구성 변경   
 > 2. 내부 로직 변경  
 > 3. realesrgan 모델 중 아래 두개 모델 선택 시 실행되지 않는 문제 해결  
 > 4. realesrgan 모델 사용방식 변경   
 >    -> realesrgan 설치폴더 내 models 폴더에 신규 모델 파일(*.param)을 복사하면 사용 가능합니다  
 > 5. 작업 대상 영상의 마지막 파일의 width, height 정보 및 예상 업스케일 크기 표시  
 > 6. config.ini 파일 마이그레이션 코드 작성  
 > 7. ffmpeg 분해 이미지 aac -> flac로 변경  
 > 8. 기타 버그 수정

v 0.1.1
 > 1. 최초 작성, ffmepg, realesrgan, flowframes를 연동한 동영상 업스케일링 프로그램 작성   
