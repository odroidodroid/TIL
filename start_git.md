## git

> git은 소스코드 형상(버전) 관리 도구
>
> 마크다운 문법 Tip!  

## 기본명령어

1. 저장소(`repository`) 만들기	

   ```bash
   $git init
   Initialized empty Git repository in C:/Users/user/TIL/.git/
   
   user@pc6 MINGW64 ~/TIL (master)
   $
   ```

   내가 원하는 폴더를 저장소로 초기화한다

   `(master)`라는 표기를 통해 해당 폴더가 git repository 라는 것을 확인할 수 있다

더 정확하게는 해당 폴더에 숨김폴더로 `.git` 이 있다

2. `git add`-커밋할 목록에 추가하기

   ```
   $git add . 
   On branch master
   
   No commits yet
   
   Changes to be committed:
     (use "git rm --cached <file>..." to unstage)
   
           new file:   a.txt
           new file:   start_git.md
   
   ```

   `git add . `에서 `.`은 현재 디렉토리를 뜻하는 리눅스 표기법이다. 현재 디렉토리의 변경사항들을 모두 커밋할 목록에 담아둔다는 뜻이다.

   `git add git.md`라고 하면, 특정 파일만 담아둘 수도 있고, `git add my folder/`라고 하면 특정 폴더를 모두 담아둘 수도 있다.

3.  커밋

   ```
   $git commit -m 'git 기초명령어 정리'	
   [master (root-commit) 529690b] git 기초명령어 정리
    2 files changed, 26 insertions(+)
    create mode 100644 a.txt
    create mode 100644 start_git.md
   ```

   커밋은 버전의 이력을 남기는 것이다. 커밋할 목록에 있는 내용들을 버전에 포함시킨다. (untracked / 목록에 없는 것은 포함 안됨.)

4. 커밋 이력 확인하기

   ```
   $git log
   commit 529690bd1c0ed4d81130757c3d651a9c67c38edd (HEAD -> master)
   Author: odroidodroid <zjzlem200@gmail.com>
   Date:   Tue May 21 12:39:01 2019 +0900
   
       git 기초명령어 정리
   
   ```

   

5.  **git 상태 확인하기**

   ```bash
   $git status
   On branch master
   Changes not staged for commit:
     (use "git add <file>..." to update what will be committed)
     (use "git checkout -- <file>..." to discard changes in working directory)
   
           modified:   start_git.md
   
   no changes added to commit (use "git add" and/or "git commit -a")
   
   ```

   CLI 에서는 현재 상태를 확인하기 위해서 지속적으로 확인해야 한다.

## 원격 저장소 활용하기(Github)

1. 저장소에 올리기

2. 저장소로부터 복제하기

   ```
   $git clone 
   https://github.com/odroidodroid/TIL.git
   ```

3. 원격 저장소에 올리기
4. 



3. 



