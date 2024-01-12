# Today I Learned (for myself)
## git - Remote Repository

> 원격 저장소.
> 코드와 버전 관리 이력을 온라인 상의 특정 위치에 저장하여 여러 개발자가 협업하고 코드를 공유할 수 있는 저장 공간

**주요 기능**
1. 원격 저장소 등록

        git remote -v  #원격 저장소 확인

        git remote add origin [url]  # origin이라는 이름의 저장소 등록

2. push
        
        git push -u origin master
        # origin이라는 저장소에 master 브랜치를 push.
        # 로컬 저장소의 commit 목록을 원격 저장소에 업로드

3. pull

        git pull [remote_repo_url]
        # 원격 저장소의 변경사항 다운로드

4. clone

        git clone [remote_repo_url]
        # 원격 저장소 전체 다운로드


---

### gitignore
> git에서 특정 파일이나 디렉토리를 추적하지 않도록 설정하는데 사용되는 텍스트 파일

**사용 순서**
1. .gitignore 파일 생성(확장자 없음)
2. a, b 이름 가진 텍스트 파일 생성
3. gitignore에 a.txt 작성 -> # a.txt 공유하지 않을 것
4. git init
5. git status