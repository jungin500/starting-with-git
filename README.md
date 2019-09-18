# SW융합프로그래밍(2019) Git 소개
## Git이란?
- 소스코드 관리를 위한 **분산 버전 관리** 시스템
- 각종 협업 작업을 위한 **코드 버전 관리** 도구
## Why Git?
- 소스코드 뿐만 아니라 각종 파일들의 이전 버전을 가지고 있다.
- 팀 단위 작업 시 실수로 파일이 누락되어도 이전 버전을 복구할 수 있다.
- 어느 누가 코드의 부분을 작성했는지 알 수 있다.

---
# 첫번째 과제
## 준비물
- Git for Windows: [다운로드](https://git-scm.com/)
- Atlassian Sourcetree: [다운로드](https://www.sourcetreeapp.com/)

## 과제 내용
1. 자신의 레포지토리를 Clone해보자.
2. Clone한 폴더 내에 `.git`이라는 이름의 폴더가 존재하는지 확인한다(기본적으로 숨겨져 있다).
3. 새로운 한글 파일을 만들어 아무 내용을 적고 `과제.hwp`라는 이름으로 저장한다  
(앞으로는 Clone한 폴더 내에서 계속 작업한다).
4. `cmd`나 `powershell` 등의 콘솔을 열고,  
저장된 파일을 `git add .`, `git commit`, `git push` 세 단계에 걸쳐서 GitHub 서버로 PUSH한다.
5. Push된 파일을 자신의 레포지토리(GitHub)에 들어가 확인한다.

# Troubleshooting
1. Git을 찾을 수 없을 때:
    ```
    'git'은(는) 내부 또는 외부 명령, 실행할 수 있는 프로그램, 또는
    배치 파일이 아닙니다.
    ```
    이 경우, Git for Windows을 여기서 다운로드한다: [Download Git](https://git-scm.com/)  
    다음으로, cmd 콘솔을 
2. 이메일 정보를 저장하지 않았을 때 (`commit`을 처음 했을 때):
    ```
    *** Please tell me who you are.

    Run

      git config --global user.email "you@example.com"
      git config --global user.name "Your Name"

    to set your account's default identity.
    Omit --global to set the identity only in this repository.

    fatal: unable to auto-detect email address (got 'jungin500@J-IPCVL-DESKTOP.(none)')
    ```
    이 경우는 위에서 말한 것처럼, 명령어 두개를 입력하면 된다:  
    `git config --global user.email "you@example.com"`  
    `git config --global user.name "Your Name"`  
    다음오르 다시 commit한다.
