---
layout: single
title:  2022년 하반기 Research Project
date:   2022-11-03 15:20:00 +0900
author: Bongjun Jang

header:
  og_image: /assets/images/logo.jpg
---

2022년 하반기(11월 ~ 12월)동안 진행할 프로젝트입니다.

## 크롬 V8 자바스크립트 엔진의 동작 과정

{% assign lgh = site.data.authors["Gahyeon Lee"] %}
* Project Leader: {{ lgh.name }}

자바스크립트 개발자라면 V8 엔진에 대해 한 번쯤은 들어봤을 거라 생각한다. V8 엔진은 C++로 작성된 고성능의 오픈소스 자바스크립트 엔진으로, 현재 Google Chrome과 Node.js에서 사용되고 있다. 이러한 V8 엔진의 동작 과정 분석을 통해 자바스크립트 코드가 어떻게 실행되는지 알아보고자 한다.

## 브라우저에 따른 사진/영상의 랜더링 차이

{% assign jyh = site.data.authors["Younho Jeon"] %}
* Project Leader: {{ jyh.name }}

아마 웹 브라우저에 대해 다들 잘 알고 있을 것입니다. 크롬, 네이버 웨일, 사파리 등이 대표적인 예입니다. 웹 브라우저가 웹 서퍼에, 필요한 웹 페이지를 요청하면 서버는 응답하고, 웹 브라우저는 이를 해석하여 사용자에게 보여줍니다. 우리는 이 해석하는 과정에, 특히 이미지와 영상이 해석되는 방식에 집중해 볼 예정입니다.

## RustPython Contribution

{% assign jbj = site.data.authors["Bongjun Jang"] %}
* Project Leader: {{ jbj.name }}

2022년 현재 Python은 세계에서 가장 많이 사용되는 언어 중 하나이며, Rust는 가장 빠르게 성장하고 있는 언어다. Python의 대표적인 인터프리터는 CPython으로, C로 작성되어 있다. RustPython은 이를 Rust로 구현한 인터프리터로 대체하고자 하는 프로젝트로, Lexer, VM, stdlib 등 여러가지 서브프로젝트가 진행되고 있다. RustPython을 분석하고, 기여하면서 Python과 Rust에 대해 더 깊이 이해해보고자 한다.

## Hello JIT!

{% assign lsh = site.data.authors["Seohyun Lee"] %}
* Project Leader: {{ lsh.name }}

파이썬은 정말 느린 언어다. 인터프리터 언어 중에서도 매우 느린 축에 속한다. 만일 당신이 알고리즘 문제 해결을 해 본 적이 있다면, 파이썬으로 제출했을 시 올바른 알고리즘을 작성했음에도 "Time Limit Exceed"를 본 적이 있을 것이다. 그리고 아마 당신은 한 번쯤 이런 대답을 들었을지도 모른다. "PYPY3으로 제출해보세요."

PYPY는 파이썬으로 만든 파이썬 구현체이다. 놀랍게도, 이것의 속도는 많은 경우에서 파이썬보다 몇 배는 빠르다. 느린 파이썬에서 파이썬을 돌리는 건데, 어떻게 이것이 가능한걸까? 비결은 바로 JIT에 있다. 이 문서에서는 JIT가 무엇인지, 그리고 최근 딥마인드에서 발표한 "s6"라는 라이브러리를 통해 이것을 CPython에도 적용시킬 수 있을 지 탐구해 보고자 한다.