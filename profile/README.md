# 레포지토리
## 레포지토리 생성 권한 
  - github를 담당하고 있는 담당자
## 최초 브랜치
  * 2025/09/26 이전부터 존재한 레포지토리 -> master 브랜치
  * 2025/09/26 이후부터 생성 레포지토리 -> main 브랜치
    * 이유 : 레거시 장비의 경우 기본 생성 레포지토리가 master이고 최신 장비의 경우 main
## 레포지토리 생성 갯수 
  - 한 장비당 1개의 레포지토리
    * GUI의 경우 용량이 크므로 별도 레포지토리로 관리
  * 예) : EMG, GMG, EMG 국방망 -> KT_EMG 레포지토리 관리
    * EMG와 GMG, EMG 국방망은 같은 성격의 장비이므로 KT_EMG에서 관리하며 같은 장비 다른 버전은 브랜치 머지 전략 등 다양한 방법으로 해당 프로젝트 팀에서 관리
## 레포지토리 생성 컨벤션 : `고객사_장비[_GUI]`
  * ex1) KT_EMG
  * ex2) KT_EMG_GUI
## Q & A
### 레포지토리 관리
  * Q : GUI의 경우 같은 장비지만 다른 성격의 파일이 있는데 어떻게 하나요? ex) KT_EMG_GUI, KT_EMG_RULE_GUI
  * A : KT_EMG_GUI 레포지토리로 묶고 폴더로 구분해서 관리하는 방법과 브랜치로 구분해서 관리하는 방법이 있습니다.
# 참고
* [관리 레포지토리 목록](https://docs.google.com/spreadsheets/d/1JK8IRUI7yCxIeYydr1r_LyKSFzNtajCdduuyxfkxOGE/edit?gid=804040885#gid=804040885)
* [협업 방법](https://heyday2024.tistory.com/35)
* `레포지토리 생성이 필요할 경우, 하주영 사원에게 알려주세요.`

---

# Git 주요 명령어 정리

| 명령어 | 설명 | 비고 |
|--------|------|------|
| `git clone https://[유저이름]:[엑세스 토큰]@[원격 저장소 주소]` | 원격 저장소 복제 |  |
| `git config user.email "본인 이메일"` | 커밋 시 사용할 이메일·이름 설정 | clone 후 해당 폴더에서 1회 실행 |
| `git config user.name "본인 이름"` | 커밋 시 사용할 이메일·이름 설정 | clone 후 해당 폴더에서 1회 실행 |
| `git config --global push.default simple` | 로컬 브랜치를 대응하는 원격 브랜치로 push | 전역 설정, 최초 1회 실행 |
| `git branch` | 로컬 저장소의 모든 브랜치 확인 |  |
| `git branch -r` | 원격 저장소의 모든 브랜치 확인 |  |
| `git pull` | 원격 저장소의 변경 내용 가져오기 |  |
| `git checkout -b [브랜치 이름]` | 새로운 브랜치 생성 후 해당 브랜치로 이동 |  |
| `git checkout [브랜치 이름]` | 기존 브랜치로 이동 |  |
| `git log` | 커밋 로그 확인 |  |
| `git add [파일명, …]` | 스테이징 영역에 파일 추가 |  |
| `git commit -m "커밋 메시지"` | 커밋 생성 | `-m` 옵션 미사용 시 에디터 실행 |
| `git push --set-upstream origin [브랜치 이름]` | 로컬 브랜치와 원격 브랜치 연결 후 최초 push | 최초 push 시 |
| `git push` | 로컬 커밋을 원격 저장소에 업로드 |  |
| `git merge [브랜치 이름]` | 현재 브랜치에 지정 브랜치의 변경 내용 합치기 | 합치려는 브랜치로 이동 후 사용 |

