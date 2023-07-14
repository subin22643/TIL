# GIT
- git의 3가지 영역
1. 워킹 디렉토리 = 내 컴퓨터에서 임시공간으로 추가
2. 스테이징 에어리어 = 임시공간
3. 레포지토리 = 외부컴퓨터



- add > 내 컴퓨터에 임시공간으로 추가
- commit > 추가한 것에 변경사항 또는 메모를 추가 (쪽지)
- push > 임시공간 > 외부컴퓨터



```
## 기초문법
.. 현재의 상위 디렉토리
touch 파일생성
mkdir 새 디렉토리 생성
ls 현재 작업중인 디렉토리 내부의 폴더/파일 목록 출력
cd 디렉토리 변경 (위치 이동)
start 폴더/파일 열기
rm 파일 삭제
rm -r 폴더 삭제
cd .. 상위 폴더로 이동
git status 상태보기


## 초기설정
git init
git status

git config --global user.email "메일주소" #본체에서 한번만
git config --global user.name "유저네임" #본체에서 한번만

git remote add origin https://github.com/subin22643/test.git #원격저장소 추가/origin은 별칭임
git remote -v


## 파일 추가, 수정
git add 파일명
	git add . #추가안된 파일 전부추가
git commit -m "메모"
git log
git push -u origin master #최초push, origin은 별칭임(rmorigin, pmorigin...)
git push #두번째부터는 git push만 해도됨


## 컴퓨터에 git 파일 추가
1. git clone 파일링크 #저장소 전체를 복제 (clone으로 받은 프로젝트는 git init 필요X)
2. Download ZIP


## 수정된 부분만 가져오기
git pull #수정된 부분만 복제
``````