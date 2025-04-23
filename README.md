# redstar upscaler
Powerful video upscaling tool using FFmpeg, Real-ESRGAN, Flowframes — now supports **multi-language UI**!

## 🌐 Language / 언어 설정
[한국어](https://github.com/redstar-programmer/upscaler/blob/main/README.md) | [English](https://github.com/redstar-programmer/upscaler/blob/main/README/README.en.md) | [日本語](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ja.md) | [中文](https://github.com/redstar-programmer/upscaler/blob/main/README/README.zh.md) |
[Français](https://github.com/redstar-programmer/upscaler/blob/main/README/README.fr.md) | [Deutsch](https://github.com/redstar-programmer/upscaler/blob/main/README/README.de.md) | [Español](https://github.com/redstar-programmer/upscaler/blob/main/README/README.es.md) | [Português](https://github.com/redstar-programmer/upscaler/blob/main/README/README.pt.md) |
[Русский](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ru.md) | [Italiano](https://github.com/redstar-programmer/upscaler/blob/main/README/README.it.md) | [Tiếng Việt](https://github.com/redstar-programmer/upscaler/blob/main/README/README.vi.md) | [Bahasa Indonesia](https://github.com/redstar-programmer/upscaler/blob/main/README/README.id.md) |
[ภาษาไทย](https://github.com/redstar-programmer/upscaler/blob/main/README/README.th.md) | [العربية](https://github.com/redstar-programmer/upscaler/blob/main/README/README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>ffmpeg, realesrgan, flowframes 기반의 동영상 업스케일링 툴</strong><br>
  <em>최신 GUI 기반, 프리셋 설정, 다중 파일 처리 지원</em>
</p>

---

다운로드 : [Release](https://github.com/redstar-programmer/upscaler/releases/)

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

아래는 간단한 사용 데모화면으로 클릭하시면 유튜브로 연결됩니다.<br>
[![시연 영상 보기](https://img.youtube.com/vi/G-JTWRws3co/0.jpg)](https://youtu.be/G-JTWRws3co "YouTube에서 보기")

## 💾 설치 및 준비사항

1. 다음 외부 도구 설치 및 위치 확인(단, 배포 파일에 ffmpeg, Real-ESRGAN 및 Flowframes 설치파일 포함되어 있음(경로 내 Programs 폴더 참조))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(선택)*
2. 압축 해제 후 readstar's upscaler.exe 실행
3. Flowframes의 경우, 사용자 환경에 따라 로드되는 모델이 다를 수 있으므로 반드시 Flowframes를 실행한 후<br>Interpolation 탭의 Interpolation AI 및 AI Model이 redstar upscaler의 resources/flowframes_models.ini 버전과 일치해야 합니다. <br>로드되지 않은 모델은 # 표시를 통해 주석처리하고 반드시 redstar upscaler의 설정 창의 모델 순서가 <br>Flowframes의 모델 순서와 일치하는지 확인하고 작업을 진행하시기 바랍니다.

## 🔧 주요 기능

![Image](https://github.com/user-attachments/assets/93dc232e-8742-4ae3-b335-9395c26a61f4)
- ✅ 영상 다중 선택 및 순차 작업
- ✅ 영상 드래그/드랍 추가
- ✅ 주요 프로그램 실행 가능여부 및 직접 선택
- ✅ 디스크 절약 모드
- ✅ 다국어 지원(15개 언어)
<br><br>
![Image](https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-484146dc6757)
- ✅ 프리셋 저장 및 자동 적용
- ✅ 오디오 코덱 자동 감지 및 비트레이트 설정
- ✅ realesrgan 모델 자동 탐지 및 선택
- ✅ FFMPEG, real-ESRGAN, Flowframes 상세 설정
- ✅ Flowframes 버전에 따른 옵션 설정 변경<br>(버전 변경은 메인 페이지의 flowframes에서 해당 버전 경로 지정시 변경 가능)
<br><br>
![Image](https://github.com/user-attachments/assets/25d60d82-53a2-4064-bbef-d439d9a9d3d6)
- ✅ 업스케일 실행명령 확인(cmd상에서 별도로 복사해 실행할 수 있음)
<br><br>
![Image](https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
- ✅ 업스케일 작업의 전반적인 진행 현황 모니터링
- ✅ 업스케일 로깅 확인(로그파일은 실생폴더 내 log폴더에 날짜로 생성)
- ✅ 작업 완료 후 결과물 자동 정리 ([REDSTAR] 접두어 부여)
- ✅ 작업 완료 후 동작 설정 가능<br>( 아무것도 하지 않음 / 프로그램 종료 / 슬립모드 / 하이버네이트 모드 / 윈도우 종료)
<br><br>
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

v 1.1.0
 > 1. 메뉴 구성(파일 열기, 닫기, 로그설정, 언어 설정)
 > 2. 다중 언어 설정 추가( 사용 가능 언어: 한국어, English, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. 언어 설정 추가에 따른 메시지 및 일부 코드 변경
 > 4. 일부 UI 구성 변경
 > 5. ffmpeg, real-ESRGAN, Flowframes 각 버전정보 표시(메인화면)
 > 6. Flowframes 1.41.0 버전 대응(현재 1.41.0 버전에 cmd 명령어 이슈가 있어서 1.40.0, 1.36.0 버전만 사용 가능)
 > 7. AI Models 항목이 소문자로 표시되는 문제 해결
 > 8. FFMPEG 옵션 추가(Pixel, video codec) - 사용자 PC에 맞는 옵션이 표시됨
 > 9. 사용자 PC별 CUDA 체크 강화 - 사용 가능 여부 및 GPU 종류 확인 가능(메인 화면)

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
