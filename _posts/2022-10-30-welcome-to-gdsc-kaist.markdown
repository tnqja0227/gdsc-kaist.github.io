---
layout: single
title:  Welcome to GDSC KAIST
date:   2022-10-30 18:30:26 +0900
author: Bongjun Jang
---

# Register yourself as an author of this blog

## GDSC KAIST Github Organization 초대

다음 링크에 접속해 초대받을 Github 계정을 남겨주세요.

https://github.com/gdsc-kaist/gdsc-kaist.github.io/issues/1

## Create a pull request against `main` branch

Fork this repository, and

1. modify _data/authors.yml to include your information
2. upload your image at `assets/images`.

For example, modify the `_data/authors.yml` file first.

``` yml
/* authors information so far */

Gildong Hong:
  name        : "Gildong Hong"
  bio         : "I will save the world"
  avatar      : "/assets/images/gildong.hong.jpg"
  links:
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      url: "gildong.hong@kaist.ac.kr"
    - label: "Website"
      icon: "fas fa-fw fa-link"
      url: "https://gildong-hong.github.io"
```

And, upload your profile image `assets/images/gildong.hong.jpg`.
Please make sure that the filepath `avatar` and your image's filename match!

And then, create a pull request. And that's it!

You can now create a post, or creating a pull request containg a new post in `_posts` directory, with your information on the front matter.
Your profile will display on the sidebar in the post you created.

```
// _posts/2022-11-01-awesome-title.md

---
title: Awesome Title
author: Gildong Hong
---

Hello, world!
```
