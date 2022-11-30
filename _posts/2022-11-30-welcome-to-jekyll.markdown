---
layout: post
title:  "Welcome to Jekyll!"
date:   2022-11-27 01:11:11 +0900
categories: jekyll update
---

## Git
`Git은 버전관리의 알파이자 오메가`
Git은 분산 버전관리 시스템으로 로컬 저장소와 원격 저장소가 존재한다. 로컬 저장소는 개발자의 pc에 존재하는 공간으로 개발자가 직접 코드를 짜는 공간이다.
로컬 저장소에서 짜여진 코드는 `commit`과 `push`를 통해 원격자장소에 저장된다. 원격 저장소에 저장된 코드는 또 다른 개발자가 `pull`과 `update`를 통해 자신의 로컬
저장소에 불러와 개발을 이어간다.

#### 로컬 저장소 생성
`user $ git init`
현재 작업중인 디렉토리를 git 저장소로 지정한다.

#### Git에 변경사항 반영하기


`user $ git init`

현재 Git 상태를 확인한다.   

{% highlight ruby %}
user $ git add examlpe.py
{% endhighlight %}
example.py를 생성(혹은 수정)하고, 이를 Commit에 반영하고 싶은 경우.   

{% highlight ruby %}
user $ git commit -m "add example.py"
{% endhighlight %}
변경사항이 반영된 new commit 생성.   

{% highlight ruby %}
user $ git log
{% endhighlight %}
commit 기록 확인하기 (Author, Commitor, Date, ...)   

## Git의 Branch
코드의 흐름을 분산시켜 더욱 효율적인 개발을 가능케 한다.

#### Branch 생성
{% highlight ruby %}
user $ git branch <branch_name>
{% endhighlight %}
git branch <branch 이름> 을 통해 branch 생성한다.

#### Branch 전환
{% highlight ruby %}
user $ git checkout <branch_name>
{% endhighlight %}
현재 작업중인 branch를 전환한다.

#### Branch 병합
{% highlight ruby %}
user $ git merge <branch_name>
{% endhighlight %}
현재 작업중인 branch를 원하는 branch에 병합한다.

#### Branch 삭제
{% highlight ruby %}
user $ git branch -d <branch_name>
{% endhighlight %}
git branch -d <branch 이름> 을 통해 branch 삭제한다.

## Github
지금까지는 Git의 로컬 저장소에서 할 수 있는 일들을 다뤘다.
`Github`는 원격 저장소 중 가장 대표적인 원격 저장소다. 

## Markdown
#### Markdown이 무엇일까요?
Markdown은 일반 텍스트로 `서식이 있는 문서`를 작성하는 방법이다.
#### Markdown 문법
`Header`
{% highlight ruby %}
# Header 1
## Header 2
### Header 3
{% endhighlight %}
#, ##, ###, ... 으로 제목(header)을 작성한다.

`Italic`
{% highlight ruby %}
*Italic*
_Italic_
{% endhighlight %}
*이나 _로 감싸서 기울임체(italic)를 작성한다.

`Bold`
{% highlight ruby %}
**Bold**
__Bold__
{% endhighlight %}
**이나 __로 감싸서 강조체(bold)를 작성한다.

`Strikethrough`
{% highlight ruby %}
~Strikethrough~
{% endhighlight %}
~로 감싸서 취소선(strikethrough)을 작성한다.

`Unordered List`
{% highlight ruby %}
-Unordered List1
-Unordered List
{% endhighlight %}
-를 앞에 붙여서 순서없는 리스트(unordered list)를 작성한다.

`Ordered List`
{% highlight ruby %}
1.Ordered List1
2.Ordered List2
{% endhighlight %}
숫자를 앞에 붙여서 순서 리스트(ordered list)를 작성한다.

`Code`
{% highlight ruby %}
'code'
{% endhighlight %}
`로 감싸서 코드(code)를 작성

`Code Block`
{% highlight ruby %}
'''
code block
'''
{% endhighlight %}
'''...''' 으로 코드 블록(code block)을 적성한다.
