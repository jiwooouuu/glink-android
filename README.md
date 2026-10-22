# FoldRemote

갤럭시 폴드7에서 회사 PC·집 PC를 원격제어하기 위한 Android 앱입니다. [RustDesk](https://github.com/rustdesk/rustdesk) 1.5.0을 수정해 회사 PC·집 PC 카드(ID 등록, 화면 연결, 파일 전송)를 홈 화면에 추가했습니다. 원격 화면·입력·파일 전송은 RustDesk 엔진이 처리합니다.

**FoldRemote는 RustDesk 공식 앱이 아닙니다.**

## 내려받기

- Android(arm64): [FoldRemote-arm64.apk](https://github.com/jiwooouuu/foldremote-android/releases/latest/download/FoldRemote-arm64.apk)
- 회사·집 Windows PC: 공식 [RustDesk 1.5.0](https://github.com/rustdesk/rustdesk/releases/tag/1.5.0) `rustdesk-1.5.0-x86_64.exe`
- 수정 소스·해시: [릴리스 페이지](https://github.com/jiwooouuu/foldremote-android/releases/latest)

## 사용

1. 회사·집 PC에서 RustDesk를 실행하고 표시되는 ID를 확인합니다.
2. 폰의 FoldRemote에서 **회사 PC** 또는 **집 PC → PC 등록**에 그 ID를 저장합니다.
3. **화면 연결**을 누르고 PC에서 승인하거나 PC의 암호를 입력합니다. 폴더 아이콘은 파일 전송입니다.
4. PC에서 폰을 조작하려면 폰의 **화면 공유** 탭에서 서비스를 시작하고 Android 화면공유·접근성 권한을 허용합니다.

앱은 PC ID만 폰에 저장합니다. 접속에는 상대 기기의 승인 또는 암호가 필요하며, 원본 RustDesk의 인증·화면공유 동의·사기 경고 절차를 바꾸지 않았습니다. 기본 연결 서버는 RustDesk 공개 서버입니다.

## 확인 상태 (1.0.0)

- 확인함: APK 빌드·서명 검증, Android 36 에뮬레이터에서 실행·원격 엔진 로딩, PC ID 저장·재시작 후 유지·해제, 세로/2열 화면, 어두운 테마
- **아직 확인 안 함:** 실제 폴드7 ↔ 회사·집 PC 원격 연결, PC ↔ PC, PC → 폰, 접힘·펼침 중 연결 유지

## 라이선스

GNU AGPL v3 (RustDesk 원본과 동일). 각 릴리스의 `FoldRemote-1.0.0-source.zip`에 그 APK에 대응하는 수정 소스·변경 고지·빌드 방법이 들어 있습니다. 원저작권은 RustDesk 개발자들에게 있습니다.
