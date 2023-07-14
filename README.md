## 인터페이스의 종류
**GUI** Graphic User Interface (ex: window)

**CLI(TUI)** Command Line Interface (ex: GITHUB, GITBASH)

### 자료 전송

클라이언트 > *REQUEST* > 서버 (API: 요청하는 규칙)

서버 > *RESPONSE* > 클라이언트 (JSON)


## CLI 기초문법
- TOUCH : 파일생성
- mkdir : 새 디렉토리 생성
- ls : 현재 위치
- cd : 작업중인 디렉토리 위치 이동
- start : 폴더/파일 열기
- rm : 삭제 

  [예시](https://drive.google.com/file/d/1KH7m2efpJ9FggD_xIWqpSOOHPIbhHp4-/view?usp=drive_link)


## GIT 이란?
**GIT** 분산버전관리시스템

**COMMIT** 분산버전 저장

### git의 3가지 영역
1. Working Directory
2. Staging Area
3. Repository

## GIT 사용법

**git 로컬 저장소 내에 또다른 git 저장소를 만들지 말 것**

1.  commit 작성자 설정

    - git config --global user.name 000
    - git config --global user.email 000@///.com

2. commit 작성자 확인
    - git config --global -l

1. git 실행(git 저장소 생성) / git 실행 취소
   - git init
   - rm -rf .git

1. git ignore
   - echo b.txt >> .gitignore
   - 파일중에 APi가 이쓰면 얘는 무조건 이그노얼해주야됨 

1. git add
   - git add .

4.  commit 준비가 되었는지 확인

    - git status

1. add 취소 (staging area에서 working directory로)
   - git reset

2. commit
   - git commit -m 'add a.txt'

5. commit 확인
   - git log

5.  commit 취소
    - rm -rf .git

6. commit 한줄로 보기
   - git log --online

## 원격저장소와 주고받기
**커밋 다 됐는지 확인하깅!!!!!!!! 커밋 이력이 없으면 push불가**

1. 로컬저장소에 원격저장소 등록하기

    $ git remote add origin https://github.com/printilikepenguin/FIRST.git

    *오리진은 그냥 내가 붙인 이름(원격저장소의), URL은 푸시할 저장소*


2. 추가된 목록 확인
    
    $ git remote -v

    *잘 됐는지 조회하기*


3. 푸시하는 법
   
    $ git push origin +master

    *오리진을 브랜치명(master)로 푸시하세용*

    *터미널 메세지 확인*

*git ignore 도 커밋파일로 올라가는데 그 안에 이그노얼된 파일명이 쓰여있*

### 내려받기(pull/clone)

- 풀 업데이트: 별칭과 브랜치명만 (변경사항있을때만 사용가능)

    - git pull origin master

- 클론 새프로젝트 시작할 때: url 필요 

    - git clone https://github.com/printilikepenguin/FIRST.git
    - 클론으로 받은건 이미 git init이 되어있음

## 코드업 파이썬 기초 100제를 풀고
논리연산 개못함 추가공부 必

리스트 정의내리는 법 좀 .......