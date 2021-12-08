---
layout: post
title: git bash로 계정 바꾸기 
categories: resolution
tags: [github, git, error]
---

### 1. 계정 바꿀 때 git bash를 통해서 변경하는 방법

```git!
$ git config --global user.name 변경을 희망하는 계정

$ git config --global user.email 변경을 희망하는 이메일
```

### 2. Windows 자격증명 수정하기

제어판 > 사용자 계정 > 자격 증명 관리 > Windows 자격 증명 > github항목 삭제 후 수정(git 관련 전부 삭제)


### 3. 오류 해결
자격 증명 수정한 이후 git에 명령어를 쓰니 오류가 나서 해결법을 찾았다

```git!
remote: Repository not found.
```

### 4. 해결
먼저 터미널에 git repository를 식별해줘야한다
```git!
git remote set-url origin https://github.com/MyRepo/project.git
```

그리고 git에 이 명령어를 입력한다
```git!
git add .
git commit -m "initial commit"
git push origin master
```
그러면 깃허브 로그인 창이 뜨면서 계정 변경이 가능하다

### 5. 출처


[Git - remote: Repository not found](https://stackoverflow.com/questions/37813568/git-remote-repository-not-found)

[git bash 터미널 계정 변경 방법](https://somjang.tistory.com/entry/Git-Git-Bash-%ED%84%B0%EB%AF%B8%EB%84%90-%EA%B3%84%EC%A0%95-%EB%B3%80%EA%B2%BD-%EB%B0%A9%EB%B2%95)
