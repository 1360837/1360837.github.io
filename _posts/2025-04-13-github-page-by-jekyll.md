---
layout: post
title: "Jekyll을 이용한 GitHub Pages 생성하기"
date: 2025-04-13 03:00:00 +0900
author: Jiwoo Nam
tags: [Jekyll, GitHub Pages]
categories: GitHub Pages
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

## Jekyll

[Jekyll 홈페이지](https://jekyllrb-ko.github.io/)

**Jekyll**을 사용하지만 Jekyll에 대해서는 아직 잘 모릅니다

## Jekyll 테마

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

repository 이름은 `GitHub 닉네임.github.io`로 설정해야 합니다.

> 이름을 잘못 설정했다면, 나중에 다시 `GitHub 닉네임.github.io`로 변경할 수 있습니다.

그럼 `GitHub 닉네임.github.io` 주소로 접속하면, Demo에서 본 GitHub Pages가 생성됩니다.

*지금 이 블로그처럼 말이죠* 😄

> 이 과정은 조금 시간이 걸릴 수 있습니다.

이제 repository 속 코드를 조금씩 수정하여 블로그를 커스터마이징할 예정입니다.

이미 일부 커스터마이징을 완료한 상태에서 블로그를 작성하고 있기 때문에, 모든 과정을 다 기록할 수는 없겠지만, 생각나는 대로 기록해보겠습니다.
