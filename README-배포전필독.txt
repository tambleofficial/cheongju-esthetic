청주 에스테틱 SEO 사이트 - GitHub / Cloudflare Pages용
====================================================

임시 사이트 정보
- 업체명: 아르케 에스테틱 청주
- 전화번호: 0507-0000-0000
- 임시 배포 도메인: https://cheongju-esthetic.pages.dev

중요: 실제 업체 확정 후 배포 전에 반드시 아래를 교체하세요.
1) 모든 HTML의 "아르케 에스테틱 청주" -> 실제 업체명
2) "0507-0000-0000" 및 "05070000000" -> 실제 전화번호
3) "https://cheongju-esthetic.pages.dev" -> 실제 Cloudflare Pages 도메인 또는 연결 도메인
4) /location/ 의 상세 주소, 주차, 영업시간
5) 네이버 플레이스, 인스타그램, 예약 링크
6) index.html의 naver-site-verification 주석을 실제 토큰으로 교체 후 활성화

SEO 구조
- / : 청주에스테틱 메인
- /services/skin-care/ : 청주피부관리
- /services/contour-care/ : 청주윤곽관리
- /services/wedding-care/ : 청주웨딩관리·청주신부관리
- /services/body-care/ : 청주바디관리
- /location/ : 가경동·강서동·청주터미널 지역 검색
- /guide/ : 정보성 콘텐츠 허브
- /guide/... : 롱테일 정보성 글
- /sitemap.xml : 전체 수집 URL
- /rss : 네이버 서치어드바이저 제출용 RSS 피드 (권장)
- /rss.xml : 동일 RSS의 호환 주소
- /robots.txt : 전체 수집 허용 + sitemap 선언

Cloudflare Pages 배포
- 이 폴더 전체를 GitHub 저장소 루트에 업로드
- Cloudflare Pages > Git 연결
- Framework preset: None
- Build command: 비워두기
- Build output directory: /

네이버 서치어드바이저 배포 후
- 사이트 소유 확인
- robots.txt 확인
- sitemap.xml 제출
- RSS 제출란: https://cheongju-esthetic.pages.dev/rss
- (호환 주소 https://cheongju-esthetic.pages.dev/rss.xml 도 포함)
- 메인/서비스 페이지 수집 요청

주의
- 상세 주소를 모르는 상태에서 가짜 주소를 넣지 않았습니다. LocalBusiness 구조화데이터는 청주시까지만 지정했습니다.
- meta keywords는 보조 신호용으로만 두고, 실제 SEO 중심은 페이지별 고유 title/description/H1/본문/내부링크입니다.
- 같은 지역키워드로 얇은 페이지를 여러 개 복제하지 않았습니다. 지역 키워드는 /location/에서 하나의 실질적인 페이지로 묶었습니다.


2026-09-17 RSS 404 수정
- 네이버 서치어드바이저가 요청한 /rss 경로가 404가 나지 않도록 루트에 실제 rss 파일을 추가했습니다.
- /rss 와 /rss.xml 모두 같은 RSS 2.0 XML을 반환하도록 구성했습니다.
- Cloudflare Pages에서 /rss 응답 Content-Type을 application/rss+xml로 고정했습니다.
- 이번 버전 배포 후 네이버 RSS 주소에는 https://cheongju-esthetic.pages.dev/rss 를 입력하세요.
