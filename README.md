# VELUNE 컬러 메이크업 쇼핑몰 스킨

20–30대 여성을 위한 미니멀 스트릿 럭셔리 색조 브랜드 시안입니다. 구매·결제·회원 기능은 포함하지 않고 카페24가 연결할 화면 형태만 구현했습니다.

## 페이지

- `index.html` — 메인(히어로/카테고리/추천/신상품/베스트/프로모션)
- `products.html` — 16개 상품 목록
- `product-detail.html` — 상품 상세, 리뷰, 문의
- `cart.html` — 장바구니
- `login.html`, `signup.html` — 로그인/회원가입
- `notice.html`, `review.html`, `qna.html` — 게시판

## 디자인 토큰

각 HTML의 `<head><style>` 최상단 `:root`에서 아래 값을 수정할 수 있습니다.

- `--color-main`, `--color-sub`, `--point`, `--color-bg`
- `--container`, `--section-gap`, 여백 토큰 `--space-*`
- 글자 크기 `--fs-*`, 두께 `--weight-*`
- `--radius`

포인트 컬러는 `--point:#FF3D72` 하나로 연결되어 있습니다.

## 이미지 규격

- 히어로 3장: 2000×900
- 띠배너 2장: 1500×420
- 팝업 2장: 400×300
- 상품 16장: 600×600
- 상품 상세 롱이미지: 800×3000

모든 이미지는 `assets/images` 안의 로컬 JPG 실사 에셋이며 임시 이미지 URL이나 SVG 플레이스홀더를 사용하지 않습니다.

## 참고

메인 슬라이드는 Swiper 11의 JavaScript CDN을 사용하며 스타일은 HTML 안에 직접 작성되어 있습니다. `build-site.mjs`는 동일한 헤더·푸터와 인라인 스타일로 전체 페이지를 다시 생성하는 관리용 소스입니다.
