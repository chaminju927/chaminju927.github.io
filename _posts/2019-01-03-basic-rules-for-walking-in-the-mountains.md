---
layout: Studying records
title: "Linux 명령어 매뉴얼"
description: 
date: 2022-11-23
---

## 1. 파일 시스템 탐색 기본 명령어
### pwd
: 현재 작업 디렉토리를 표시하는 명령어
$ pwd
 /home/vagrant

### cd
: 특정 디렉토리로 이동. cd 디렉토리명
[vagrant@host1 ~]$ cd git
[vagrant@host1 git]$

### ls 
: 현재 위치의 디렉토리 내용 리스트 출력.
[vagrant@host1 git]$ ls
bitcamp-ncp  bitcamp-ncp2  bitcamp-study  bitcamp-test

### file
: 리눅스 명령어로 파일 종류 확인할때 사용. file [파일명]
$ file c.txt
 c. txt: ASCll text

### less
: 파일 내용을 한 화면에 보여주는 명령어, 파일 내용을 보여주는 화면에서 나갈때는 q 사용
$ less c.txt
 9999
 8888
 7777
 c.txt (END)

## 2. 파일과 디렉토리 조작 명령어
### cp
: 기존 파일을 복사해 새 파일을 생성한다. cp 기존파일명 새파일명
$ cp file1 file2
$ ls
  file1 file2

### mv
: 파일 위치를 이동하는 명령어. 같은 폴더에서 파일, 디렉토리 이동을 하는 경우 이름 변경도 가능.
: 파일명 변경하는 경우 mv 기존파일명 새파일명
$ mv file1 file2   
$ls
 file2             

: 파일 위치를 이동하는 경우 mv 이동할파일명 이동할 디렉토리나 파일명
$ ls
 dir1/ file1 file2
$ mv file1 file2 dir1/      
$ ls
  dir1/
 ~ dirl1] $ ls
           file1 file2 


### mkdir
: 디렉토리를 만들때 사용하는 명령어. 
  ~ git]$ ls
bitcamp-ncp  bitcamp-ncp2  bitcamp-study
 ~ git]$ mkdir file3
  ~ git]$ ls 
file3 bitcamp-ncp  bitcamp-ncp2  bitcamp-study 



### rm
: remove의 약자로 디렉토리를 삭제할때 사용하는 명령어.
 ~  git]$ rm -rf 11
 ~  git]$ ls
bitcamp-ncp  bitcamp-ncp2  bitcamp-study  bitcamp-test



### ln
: link의 약자로 링크파일을 만들때 사용한다. 링크는 원본이 삭제되어도 사용가능한 하드링크와, 원본이삭제되 사용할 수 없는 심볼릭링크가 있다.
하드링크는 아래 명령어로 만들수 있다.
$ ln [원본링크] [링크이름] 
심볼릭링크는 아래 명령ㅇ로 만들수 있다.
$ ln -s [원본링크] [링크이름]
