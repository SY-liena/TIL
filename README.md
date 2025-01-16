# About git

- git : 분산 버전 관리 시스템
- git : 로컬 저장소  
- github, gitlab : 원격 저장소

## git 명령어
- git init : git 시작
- rm -rf .git : git 삭제(git 종료)
- ~~git config --global user.name "이름"~~
- ~~git config --global user.email "이메일"~~
- git add . : staging area 에 올리기
- git status : staging area 작업 파일 확인
- git commit -m "메시지명" : repository에 올리기
- git log : repository 작업 파일 확인(커밋 되어 있는지 확인)
- git remote add origin(별칭) url : 로컬 저장소와 원격 저장소를 연결
- git remote -v : remote 목록 확인
- git remote rm origin(별칭) : 연결된 원격 저장소가 삭제됨(별칭 지정된 연결 해제제)
- git push origin +master : 최종적으로 commit 되어 있는것을 강제로 push(origin은 별칭, master는 브랜치명, +:강제로 진행)

## clone vs pull
  - **clone** : 새로운 환경에서 처음 다운로드
      - git clone url
  - **pull** : push나 clone을 전에 진행한 후에 다운로드 
    - git pull origin +master


## gitignore
    - gitignore 파일을 왜 만들까?
    - 용량이 크거나, 보안상 문제가 있거나 청구결제 관련된 api_key 같은 파일을 add 하지 않기 위해(staging area에 올리지 않기 위해)

- .gitignore 파일 생성 -> 내부에 add 하지 않을 파일명이나 디렉토리명 작성, 저장

---
(+) git push 이후 자리 옮겼을 때 제어판의 windows 자격 증명
-> 일반 자격 증명 에서 github 삭제하기