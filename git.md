# Git
### 분산 버전 관리 시스템

> 버전관리란?
> 변화를 기록하고 출력하는 것

예)
Google Drive - 새 문서 - Google Docs - 버전 기록

.

**버전관리는 `변경사항 + 최종파일` 의 형태로 이루어짐**

.

## 중앙 vs 분산

### 중앙 집중식
- 버전은 중앙 서버에 저장되고 중앙 서버에서 파일을 가져와 다시 중앙에 업로드

### 분산식
-  버전을 여러 개의 복제된 저장소에 저장 및 관리 (Git 해당)

.

**분산구조에서의 장점**
- 중앙서버에 의존할 필요 X
- 중앙서버의 장애나 손실에 대비하여 백업과 복구가 용이
- 인터넷이 연결되지 않아도 작업 가능(나중에 중앙 서버와 동기화)

---
### git의 역할
- 코드의 버전(히스토리)관리
    - 개발되어 온 과정 파악
- 이전 버전과의 변경사항 비교


### git의 3가지 영역

- Working Directory
- Staging Area
- Repository

> **※ 위 영역들은 가상의 영역임 ※**

**Working Directory**
- 실제 작업 중인 파일들이 위치하는 영역 (수정, 생성, 삭제 등)

**Staging Area**
- WD에서 변경된 파일 중, 다음 버전에 포함시킬 파일들을 선택적으로 추가하거나 제외할 수 있는 중간 준비 영역
- 실질적으로 버전 관리할 파일을 선별하는 공간

**Repository**
- 버전(commit) 이력들과 파일들이 영구적으로 저장되는 영역
- 모든 버전과 변경 이력이 기록됨

> **commit: 변경된 파일을 저장하는 행위**


## git init

- git 설정
- 해당 폴더를 git으로 관리할 준비
- 로컬 저장소 설정(초기화)
- git의 버전관리를 시작할 디렉토리에서 진행
- 기능 단위로 실행하게 됨

```bash
git init
```
![alt text](image-11.png)

-  `.git/` 폴더 생성됨\
- git으로 관리되는 폴더는 (master) 표시가 뜸 (branch)

## git add

- 변경사항에 있는 파일을 staging area 에 추가
- 버전을 관리할 파일만 남김
- commit은 항상 staging area에 올라온 파일들만을 대상으로 함

## git commit

- Staging Area에 있는 파일들을 저장소에 기록
- 해당 시점의 버전을 생성하고 변경 이력을 남김


--- 
.

`WD에서 작업 → SA에 파일 올림 (git add) → Repo에 commit (git commit)`

.

> git status 확인
```bash
git status
```
- 빨간색: WD 영역에 있으나 버전 이력이 없음\


`git add` 시 SA에 포함됨
> git add
```bash
git add README.md
git status
```
- README.md만 초록색으로 바뀜 (SA에 추가됨)


> Commit
```bash
git commit -m '메시지 내용'
```
- commit 찍을 때 이력내용을 남겨야함 (title로 요약)


> 작성자 명시
```bash
git config --global user.email "메일주소"
git config --global user.name "유저이름"
```
- git은 협업 툴이기 때문에 작성자가 누군지 명시해주어야 함(최초 1회만)
- 깃헙 잔디 → repo 사용자와 commit 사용자 일치해야 함

```bash
$ git config --global --list
```
- 작성자 정보 확인
> commit 기록 확인
```bash
git log
```
![alt text](image-12.png)

