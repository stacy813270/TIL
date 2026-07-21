## Git
분산 버전 관리 시스템. 코드의 ‘변경 이력’을 기록하고 ‘협업’을 원활하게 하는 도구

<br>

### Git의 3가지 영역

**Working Directory** - 눈으로 보고 있는 영역. 빨간색🔴 글씨로 표시됨.

실제 작업 중인 파일들이 위치하는 영역

⬇️ git add

**Staging Area** - 중간 영역. 초록색🟢 글씨로 표시됨

Working Directory에서 변경된 파일 중 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역

⬇️ git commit -m

**Repository** - 버전 영역. 파란색🔵 글씨로 표시됨

버전 이력과 파일들이 영구적으로 저장되는 영역. 모든 버전과 변경 이력이 기록됨

<br>

**Commit**

변경된 파일들을 저장하는 행위. ‘snapshot’ 이라고도 함

<br>

### Git의 동작

- git init: 초기화하고 시작한다. 시작 선언(깃의 관리를 받을 것이다)
    - (master) 표시가 뜨면 git의 관리를 받는 폴더라는 것(그 폴더부터 하위의 모든 폴더)
    - 주의사항
      - Git 내부에  Git 저장소 만들면 안됨. Git 저장소 안의 하위 Git 저장소 git init을 인식 못 함. 바탕화면에서 Git init을 하는 순간 파멸. 바탕화면에 있는 모든 폴더의 git 저장소가 작동 안 하는 문제 발생함.
      - → 복구방법: 폴더 상단 ‘…’ 안에 ‘폴더 옵션-보기’에  들어가서 숨김 파일, 드라이브 표시 활성화 하면 생기는 폴더(.git) 삭제
- git add: 변경사항이 있는 파일을 staging area에 추가
- git commit: staging area에 있는 파일들을 저장소에 기록. 해당 시점의 버전을 생성하고 변경 이력을 남기는 것.

- git status: 현재 로컬 저장소의 파일 상태 보기. 계속 확인하기
- git log:  Commit history  보기
- git log --online: Commit 목록 한 줄로 보기
- git config --global -l: Git global 설정 정보 보기
  - Commit 작성자(author) 정보 설정; Global로 설정 후 앞으로 재입력하지 않음
  - git config --global user.email "메일주소"
  - git config --global user.name "유저네임"                                                                 
> q누르면 해당 명령어 결과 부분에서 나와서 다음 입력창으로 이동 가능

