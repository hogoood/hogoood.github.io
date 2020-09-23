---
layout: post
comments: true
title : 깃허브에 disqus 연동하기
categories: [Github]
---

## 깃허브에 disqus 댓글기능 추가하기

깃허브에서 제공해주지 않는 댓글기능을
disqus를 통해서 추가할 수 있다.

1. [disqus](https://disqus.com/) 가입하기

2. 가입완료후 "I want to install Disqus on my site"를 클릭, 사이트를 생성한다.

3. 생성이 완료되면 같이 생성된 shortname으로 댓글기능을 추가할 수 있다.

4. 오른쪽 우측 프로필 탭 > Install on site > 나타난 페이지 하단의 "install manually with Universal code"

5. 4번까지 완료후 나오는 페이지의 1번박스에 들어있는 코드를 복사한다.

6. 깃헙 페이지 레파지토리의 include 용 disqus.html을 생성한다.

7. 해당 레파지토리의 config.yml에 disqus shortname을 추가한다.

8. posting할때 comments: true로 댓글을 활성화 시켜준다.
