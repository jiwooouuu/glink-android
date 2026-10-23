<p align="center"><img src="assets/logo.png" alt="지링크" width="420"></p>

<p align="center"><b>폰에서 회사·집 PC 원격 제어</b><br>갤럭시 폴드7용 Android 앱 · RustDesk 1.5.0 기반 · 비공식</p>

---

지링크는 [RustDesk](https://github.com/rustdesk/rustdesk) 1.5.0을 수정한 Android 앱입니다.

- 첫 화면에 회사 PC·집 PC를 등록해 두고, 한 번 눌러 원격 화면 연결이나 파일 전송을 합니다.
- 원격 화면·입력·파일 전송은 RustDesk 엔진이 처리합니다.
- 테마는 10종이고, 접힌 화면과 펼친 화면 모두에서 쓸 수 있습니다.

**지링크는 RustDesk 공식 앱이 아닙니다.** 1.0.0 때 이름은 FoldRemote였습니다.

## 내려받기

- **Android(arm64):** [GLink-arm64.apk](https://github.com/jiwooouuu/glink-android/releases/latest/download/GLink-arm64.apk)
- **회사·집 Windows PC:** 공식 [RustDesk 1.5.0](https://github.com/rustdesk/rustdesk/releases/tag/1.5.0)의 `rustdesk-1.5.0-x86_64.exe`
- **지링크 PC(Windows, 선택):** [설치 파일 GLink-PC-Setup.exe](https://github.com/jiwooouuu/glink-android/releases/latest/download/GLink-PC-Setup.exe)(내 계정에만 설치, 관리자 권한 불필요) 또는 [압축 파일 GLink-PC-win-x64.zip](https://github.com/jiwooouuu/glink-android/releases/latest/download/GLink-PC-win-x64.zip)(압축을 풀고 `GLink.exe` 실행). 「내 PC」 목록에서 한 번에 연결·파일 전송, 이 PC의 ID 보기·복사. 원격 화면은 같은 PC의 공식 RustDesk가 띄웁니다.
- **수정 소스·해시:** [릴리스 페이지](https://github.com/jiwooouuu/glink-android/releases/latest)

Play 프로텍트가 설치를 막을 수 있습니다. PC → 폰 조작에 쓰는 접근성 권한 때문입니다. 이때는 USB 디버깅으로 설치하거나, 앱 스캔을 잠깐 끄고 설치한 뒤 바로 다시 켭니다.

## 사용

1. 회사·집 PC에서 RustDesk를 실행하고, 표시되는 ID를 확인합니다.
2. 지링크의 **내 PC**에서 **등록**을 눌러 그 ID를 저장합니다.
3. 처음 한 번은 **로그인**합니다. RustDesk 공개 서버의 규칙이며, Google·GitHub 계정으로 무료입니다.
4. **연결**을 누르고, PC에서 승인하거나 PC의 암호를 입력합니다. 폴더 단추는 파일 전송입니다.
5. PC에서 폰을 조작하려면 **화면 공유** 탭에서 서비스를 시작하고, Android 화면공유·접근성 권한을 허용합니다.

앱은 PC ID만 폰에 저장합니다. 접속에는 상대 기기의 승인이나 암호가 필요합니다. 원본 RustDesk의 인증·화면공유 동의·사기 경고 절차는 바꾸지 않았습니다.

## 확인 상태 (1.0.1)

- **확인함:**
  - APK 빌드·서명 검증
  - 에뮬레이터에서 실행·원격 엔진 로딩
  - PC ID 저장·유지·해제, 테마 전환·유지
  - 실제 폴드7에서 공개 서버까지 연결 시도가 도달함
- **아직 확인 안 함:**
  - 로그인한 뒤 실제 폴드7 ↔ 회사·집 PC 원격 연결
  - PC ↔ PC 연결, PC → 폰 조작

## 라이선스

GNU AGPL v3(RustDesk 원본과 같음). 원저작권은 RustDesk 개발자들에게 있습니다.

각 릴리스의 `GLink-x.y.z-source.zip`에 그 APK에 대응하는 수정 소스, 변경 고지, 빌드 방법이 들어 있습니다. 앱 글꼴 Pretendard는 OFL 1.1입니다.
