---
layout: post
title: jekyll 오류 해결
categories: resolution
tags: [github, jekyll, ruby, error]
---

### 깃허브 블로그 오류 해결
깃허브 블로그 만들다가 오류가 너무나서 오류 해결한 것들 정리하는 글

### Jekyll 4.2.1 Please append --trace to the serve command
``` ruby!
      Jekyll 4.2.1   Please append `--trace` to the `serve` command
                     for any additional information or backtrace.
```

해결 방법
```ruby!
bundle exec jekyll serve --trace
```

### cannot load such file -- webrick
```ruby!
servlet.rb:3:in `require': cannot load such file -- webrick (LoadError)
```

해결방법
```ruby!
bundle add webrick
```

참고 사이트
[Load error: cannot load such file - webrick](https://talk.jekyllrb.com/t/load-error-cannot-load-such-file-webrick/5417)


[jekyll 오류 해결 (부제: github 블로그 만들기)](https://velog.io/@minji-o-j/jekyll-%EC%98%A4%EB%A5%98-%ED%95%B4%EA%B2%B0)
