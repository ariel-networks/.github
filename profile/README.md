* Git 주요 명령어 정리

| 명령어 | 설명 | 비고 |
|--------|------|------|
| `git clone https://[유저이름]:[토큰]@[원격 저장소 주소]` | 원격 저장소 복제 | 최초 1회 실행 |
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

