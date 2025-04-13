---
layout: post
title: "Jekyll을 이용한 GitHub Pages 생성하기"
date: 2025-04-13 03:00:00 +0900
author: Jiwoo Nam
tags: [jekyll, github.io]
categories: blog-setup
toc : true
published: true
---

>**블로그 시작하기**

> 2023년부터 생각만 해오던 블로그를 드디어 시작하게 되었습니다.
>
> 여러 플랫폼을 고민한 끝에, ChatGPT의 추천으로 **GitHub Pages**와 **Jekyll**을 선택했습니다.  
>
> 복잡한 웹 기술 없이 **Markdown**만으로도 쉽게 글을 쓸 수 있다는 점이 매력적이었습니다.
>
> 준비물 : GitHub 계정

# Jekyll 과 GitHub Pages

[Jekyll 홈페이지](https://jekyllrb-ko.github.io/)

**Jekyll**이라는 단어를 이번에 처음 들었습니다. 루비 기반 정적 사이트 생성기라는 설명을 봤지만, 솔직히 아직도 Jekyll이 정확히 뭘 하는 도구인지 완전히 이해하지 못했습니다.

루비도 설치하지 않았고, 터미널에서 `jekyll` 명령어를 쳐본 적도 없습니다.  
그런데도 GitHub에서 테마 저장소를 포크하고, 저장소 이름을 `username.github.io`로 바꿨을 뿐인데 블로그가 바로 생성되었습니다.

아무것도 모른 채 시작했지만, 이처럼 쉽게 블로그를 만들 수 있다는 점이 Jekyll과 GitHub Pages의 가장 큰 장점인 것 같습니다.

## Jekyll 테마 선택

Jekyll은 다양한 테마를 무료로 제공하기 때문에, 취향에 맞는 블로그 스타일을 어느 정도 선택할 수 있습니다.

우선 테마를 고르기 위해 [여기](http://jekyllthemes.org/)로 들어가줍니다.

![](/assets/image/2025-04-13-github-page-by-jekyll/1.png)

깔끔한 디자인과 심플한 구성이 좋아서 `Not Pure Poole`라는 테마로 선택했습니다.

Not Pure Poole을 클릭하면 아래처럼 나타납니다.

![](/assets/image/2025-04-13-github-page-by-jekyll/2.png)

여기서 **Homepage**를 누르면 됩니다

> *Demo를 누르면 미리보기가 가능하니 테마 고를때 참고하세요*

## Repository 생성, 빌드

![](/assets/image/2025-04-13-github-page-by-jekyll/3.png)

GitHub repository가 뜨면, 그곳에서 **fork**를 눌러 새로운 repository를 만들면 됩니다.

repository 이름은 `username.github.io`로 설정해야 합니다.

> 이름을 잘못 설정했다면, 나중에 다시 `username.github.io`로 변경할 수 있습니다.

## GitHub Pages 설정 확인

포크한 저장소에서 `Settings > Pages`에 들어가면 GitHub Pages 설정을 확인할 수 있습니다.  
보통 `main` 브랜치를 선택하고, 디렉토리는 `/ (root)`로 설정하면 자동으로 블로그가 배포됩니다.

저는 GitHub Pages 설정을 마친 후, 블로그 주소인 `https://1360837.github.io`로 접속해보았습니다.  
몇 분 지나지 않아 페이지가 정상적으로 열리는 것을 확인할 수 있었습니다.  

> 처음엔 "왜 안 뜨지?" 하고 당황했지만, 보통 1~5분 정도 시간이 걸리니 조금만 기다려보시면 됩니다.

![](/screenshot.png)

> ※ 참고: 제 블로그는 이미 기본 설정을 일부 변경한 상태라, 처음 블로그가 생성됐을 때의 스크린샷은 따로 남기지 못했습니다.  
대신 테마에서 기본으로 제공하는 `screenshot.png` 이미지를 활용했습니다.

## 기본 설정 변경하기

블로그를 내 스타일로 바꾸기 위해 가장 먼저 수정한 파일은 `_config.yml`입니다.  
사이트 이름, 이메일, 소개글, SNS 링크 등 여러 정보를 이 파일에서 바꿀 수 있습니다.

예를 들어 저는 아래처럼 변경했어요:

```yml
# Setup
title: "#define Jiwoo"
description: From Pixels to Programs
url: https://1360837.github.io
avatar: /avatar.jpeg
paginate: 5
permalink: pretty
cover_image: /bg.jpeg

...

# Specify the author for blog posts
author:
  name: Jiwoo Nam
  url: https://github.com/1360837/
  email: woowoo4599@naver.com
```

<del> 블로그 title과 description은 ChatGpt가 추천해주었습니다.</del>

여기서 `avatar.jpeg`와 `bg.jpeg` 파일 설정이 있어서, 원하는 사진을 해당 이름으로 저장해 프로젝트 폴더에 넣어두었더니
아바타, 커버 이미지, 블로그 타이틀과 소개글까지 함께 적용된 걸 확인할 수 있었습니다.

![](/assets/image/2025-04-13-github-page-by-jekyll/4.png)

<del>트위터는 사용하지 않아서 트위터 항목을 코드에서 제거했더니, 블로그 상의 트위터 아이콘도 함께 사라졌습니다.</del>

## 마무리하며

아직 블로그에 대해 모든 걸 이해한 것은 아니지만, 이렇게 하나씩 시도해보고 글로 남기면서 조금씩 배워가고 있습니다.

처음 도전하시는 분들도 “GitHub Pages? 뭔가 어려울 것 같아…” 하는 마음은 잠시 내려두시고, 가볍게 시작해보시길 추천드립니다.

앞으로도 블로그를 개설하고 꾸며가는 과정을 이곳에 차근차근 정리해볼 예정입니다.
