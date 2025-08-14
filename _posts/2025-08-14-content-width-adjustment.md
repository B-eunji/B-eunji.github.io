---
title: "Minimal Mistakes 테마에서 본문 폭 조정하는 법 (classes 속성 활용)"
date: 2025-08-14
# categories: blog 발전
tags: [jekyll, minimal-mistakes, blog, css, front-matter, wide-class]
classes: wide
---

## 📌 문제 상황
Minimal Mistakes 테마를 사용하고 있는 현재 블로그에서 본문 폭이 좁아서 너무 답답해 보이는 상황이었습니다. 사이드바를 사용하지 않는데도 여백이 넓어, 실제 콘텐츠 영역이 작아 보였습니다.

---

## 🛠 해결 과정

1. **원인 파악**
   - `_sass` 폴더의 `page.scss`를 확인하니, 기본 레이아웃이 **사이드바 폭**을 고려하여 본문 폭을 제한하고 있었습니다.
   - 사이드바를 사용하지 않아도 이 폭 제한이 적용되고 있었습니다.

2. **해결 방법**
   - Front Matter에 `classes: wide`를 추가해 폭 제한을 해제.
   - `custom.scss`생성 후 `max-width`를 직접 조정.

3. **적용 전/후 비교 이미지**
![wide 적용 전 화면](/assets/images/2025-08-14-wide-class/before.png)
![wide 적용 후 화면](/assets/images/2025-08-14-wide-class/after.png)

