<h1 align="center" style="position: relative;">
  <br>
    <img src="./assets/shoppy-x-ray.svg" alt="logo" width="200">
  <br>
  The Moved Mover - Shopify Theme
</h1>

<p align="center">
  독립 출판물의 가치를 전하는 온라인 서점 테마
</p>

<p align="center">
  <a href="./LICENSE.md"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License"></a>
</p>

## 📖 프로젝트 소개

**The Moved Mover**는 독립 출판물, 아티스트북, 그리고 창작자들의 목소리를 담은 책들을 판매하는 Shopify 테마입니다.

> "우리는 매 순간 흔들리고, 움직이며, 변합니다. 그리고 그 흔들림은 다시 누군가를 움직입니다. **The Moved Mover**는 그 파동을 기록으로 남깁니다."

이 테마는 Shopify의 최신 기능과 모범 사례를 활용하여 독립 출판사가 온라인에서 자신의 브랜드와 도서를 효과적으로 소개하고 판매할 수 있도록 설계되었습니다.

## ✨ 주요 기능

### 🏠 홈페이지
- **히어로 배너**: 브랜드 철학과 메시지를 전달하는 대형 배너
- **추천 도서**: 엄선된 독립 출판물 소개
- **협력 출판사**: 파트너 출판사 하이라이트
- **최신 뉴스**: 출간 소식 및 이벤트 정보
- **뉴스레터 구독**: 독자와의 지속적인 소통

### 📚 도서 카탈로그
- **카테고리별 필터링**: 에세이, 소설, 시, 예술, 철학 등
- **검색 기능**: 도서명, 저자명으로 빠른 검색
- **도서 상세 페이지**: 표지, 저자 소개, 책 소개문, 구매 링크
- **컬렉션 페이지**: 다양한 도서 컬렉션 탐색

### 📖 페이지
- **About (소개)**: 출판사 스토리, 가치, 팀 소개
- **Authors (작가)**: 소속 작가 및 출간 작가 소개
- **Contact (연락처)**: 문의 폼 및 연락처 정보
- **FAQ (자주 묻는 질문)**: 자주 묻는 질문과 답변
- **Submission (투고 안내)**: 원고 투고 절차 및 가이드라인

### 🛒 쇼핑 기능
- **장바구니**: Shopify 기본 장바구니 기능
- **상품 페이지**: 도서 상세 정보 및 구매 옵션
- **검색**: 전역 검색 기능

### 📝 블로그
- **블로그 목록**: 최신 글 목록
- **블로그 상세**: 개별 글 보기
- **작가 인터뷰**: 작가와의 대화 콘텐츠

## 🚀 시작하기

### 사전 요구사항

시작하기 전에 다음이 설치되어 있어야 합니다:

- [Shopify CLI](https://shopify.dev/docs/api/shopify-cli) – 테마 개발, 업로드, 미리보기를 위한 도구

VS Code를 사용하는 경우:

- [Shopify Liquid VS Code Extension](https://shopify.dev/docs/storefronts/themes/tools/shopify-liquid-vscode) – Liquid 템플릿을 위한 구문 강조, 린팅, 인라인 문서화, 자동 완성

### 설치

이 저장소를 Git 또는 Shopify CLI로 클론합니다:

```bash
git clone <repository-url>
cd learn-shopify-theme
```

### 개발

Shopify CLI를 사용하여 테마를 미리 볼 수 있습니다:

```bash
shopify theme dev
```

이 명령은 로컬 개발 서버를 시작하고 변경 사항을 실시간으로 미리 볼 수 있게 해줍니다.

### 배포

테마를 Shopify 스토어에 배포하려면:

```bash
shopify theme push
```

## 📁 테마 구조

```
.
├── assets/          # 정적 자산 (CSS, JS, 이미지, 폰트 등)
│   ├── critical.css # 필수 CSS (모든 페이지에 필요)
│   └── ...
├── blocks/          # 재사용 가능한, 중첩 가능한, 커스터마이징 가능한 UI 컴포넌트
│   ├── group.liquid
│   └── text.liquid
├── config/          # 전역 테마 설정 및 커스터마이징 옵션
│   ├── settings_data.json
│   └── settings_schema.json
├── layout/          # 페이지의 최상위 래퍼 (레이아웃 템플릿)
│   ├── theme.liquid
│   └── password.liquid
├── locales/         # 테마 국제화를 위한 번역 파일
│   ├── en.default.json
│   └── en.default.schema.json
├── sections/        # 모듈식 전체 너비 페이지 컴포넌트
│   ├── home-hero.liquid
│   ├── featured-books.liquid
│   ├── books-catalog.liquid
│   ├── about-hero.liquid
│   ├── submission-form.liquid
│   └── ...
├── snippets/        # 재사용 가능한 Liquid 코드 또는 HTML 조각
│   ├── css-variables.liquid
│   ├── image.liquid
│   └── meta-tags.liquid
└── templates/       # 섹션을 결합하여 페이지 구조를 정의하는 템플릿
    ├── index.json
    ├── collection.json
    ├── product.json
    ├── page.about.json
    ├── page.submission.json
    └── ...
```

자세한 내용은 [Shopify 테마 아키텍처 문서](https://shopify.dev/docs/storefronts/themes/architecture)를 참조하세요.

## 🎨 주요 섹션

### 홈페이지 섹션
- **home-hero**: 메인 히어로 배너 (비디오/이미지 배경 지원)
- **featured-books**: 추천 도서 그리드
- **publishers-spotlight**: 협력 출판사 소개
- **latest-news**: 최신 뉴스 및 이벤트
- **newsletter**: 뉴스레터 구독 폼

### 도서 관련 섹션
- **books-catalog**: 카테고리별 도서 카탈로그 (필터링 및 검색)
- **featured-books**: 추천 도서 섹션
- **product**: 도서 상세 페이지

### 페이지 섹션
- **about-hero**: About 페이지 히어로
- **about-story**: 출판사 스토리
- **about-values**: 핵심 가치
- **about-team**: 팀 소개
- **submission-hero**: 투고 안내 히어로
- **submission-process**: 투고 절차
- **submission-guidelines**: 투고 가이드라인
- **submission-form**: 원고 제출 폼
- **contact-hero**: 연락처 히어로
- **contact-form**: 문의 폼
- **contact-info**: 연락처 정보
- **faq-hero**: FAQ 히어로
- **faq**: 자주 묻는 질문 목록

### 공통 섹션
- **header**: 헤더 네비게이션
- **footer-custom**: 커스텀 푸터
- **newsletter**: 뉴스레터 구독

## 🛠️ 개발 가이드

### 스키마 설정

섹션과 블록은 `{% schema %}` 태그를 통해 커스터마이징 가능합니다. 설정에 대한 자세한 내용은 [섹션 스키마 문서](https://shopify.dev/docs/storefronts/themes/architecture/sections/section-schema)를 참조하세요.

#### 단일 속성 설정

단일 CSS 속성에 해당하는 설정의 경우 CSS 변수를 사용하는 것을 권장합니다:

```liquid
<div class="collection" style="--gap: {{ block.settings.gap }}px">
  ...
</div>

{% stylesheet %}
  .collection {
    gap: var(--gap);
  }
{% endstylesheet %}

{% schema %}
{
  "settings": [{
    "type": "range",
    "label": "gap",
    "id": "gap",
    "min": 0,
    "max": 100,
    "unit": "px",
    "default": 0
  }]
}
{% endschema %}
```

#### 다중 속성 설정

여러 CSS 속성을 제어하는 설정의 경우 CSS 클래스를 사용합니다:

```liquid
<div class="collection {{ block.settings.layout }}">
  ...
</div>

{% stylesheet %}
  .collection--full-width {
    /* multiple styles */
  }
  .collection--narrow {
    /* multiple styles */
  }
{% endstylesheet %}

{% schema %}
{
  "settings": [{
    "type": "select",
    "id": "layout",
    "label": "layout",
    "options": [
      { "value": "collection--full-width", "label": "전체 너비" },
      { "value": "collection--narrow", "label": "좁은 너비" }
    ]
  }]
}
{% endschema %}
```

### CSS & JavaScript

CSS와 JavaScript의 경우 [`{% stylesheet %}`](https://shopify.dev/docs/api/liquid/tags#stylesheet)와 [`{% javascript %}`](https://shopify.dev/docs/api/liquid/tags/javascript) 태그를 사용하는 것을 권장합니다. 이 태그들은 여러 번 포함될 수 있지만 코드는 한 번만 나타납니다.

### critical.css

이 테마는 모든 페이지에 필요한 필수 CSS를 별도의 `critical.css` 파일로 명시적으로 분리합니다. 이 파일은 페이지 로드 성능을 최적화하는 데 도움이 됩니다.

## 🎯 브랜드 철학

**The Moved Mover**는 다음과 같은 철학을 바탕으로 설계되었습니다:

- **흔들림과 움직임**: 우리는 매 순간 변화하고 성장합니다
- **기록의 가치**: 그 변화의 파동을 기록으로 남깁니다
- **독립의 정신**: 창작자들의 독립적인 목소리를 존중합니다
- **커뮤니티**: 독자, 작가, 출판사가 함께 만드는 공간입니다

## 📄 라이선스

이 프로젝트는 [MIT 라이선스](./LICENSE.md) 하에 오픈소스로 제공됩니다.

## 🤝 기여하기

이 프로젝트에 기여하고 싶으시다면 [CONTRIBUTING.md](./CONTRIBUTING.md)를 참조하세요.

## 📞 문의

프로젝트에 대한 문의사항이 있으시면 이슈를 생성해 주세요.

---

**The Moved Mover** - 흔들림과 움직임을 기록하는 곳
