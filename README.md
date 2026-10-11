# 발췌기

**바로 쓰기 → https://romantic-lamb.github.io/excerptourstory/**

AI 채팅(SillyTavern, 그 밖의 채팅 플랫폼)을 붙여 넣고 다듬어 **이미지 · PDF · HTML** 발췌본으로 만드는 도구입니다.
설치 없이 브라우저에서 바로 쓰고, 붙여 넣은 글은 브라우저 밖으로 나가지 않습니다.

## 쓰는 법

1. **쓰기** 탭에서 `+ 대사`, `+ 지문`으로 칸을 만들어 글을 쓰거나 붙여 넣습니다.
   - `한꺼번에 붙여넣기`: 채팅을 통째로 넣으면 대사와 지문을 칸으로 나눠 줍니다.
   - `채팅 파일에서 가져오기`: SillyTavern의 `.jsonl` 채팅 파일에서 메시지를 골라 가져옵니다.
   - `글 형식`: `"대사" 지문`(따옴표 안이 대사)과 `*지문* 대사`(별표 안이 지문) 중에 고릅니다.
2. **꾸미기** 탭에서 모양(책장 · 대본 · 커스텀 · 말풍선 · 창 테마), 글꼴, 크기, 자간, 장평, 색, 간격을 정합니다.
3. 오른쪽 미리보기 위에서 **이미지 / PDF / HTML**을 골라 저장합니다. 긴 글은 비율이나 장수를 정해 여러 장으로 나눌 수 있고, 나뉜 장은 미리보기에 저장될 모습 그대로 한 장씩 보입니다.

꾸미기 값과 쓰던 글은 그 브라우저에 자동으로 기억됩니다. `내 설정`에서 이름을 붙여 저장하거나 파일로 내려받을 수도 있습니다.

## 내 깃허브에서 열기 (GitHub Pages)

1. 이 폴더의 파일(`index.html`, `README.md`, `.nojekyll`)을 공개 저장소에 올립니다.
2. 저장소의 **Settings → Pages**에서 Source를 `Deploy from a branch`, Branch를 `main` / `/ (root)`로 고르고 저장합니다.
3. 1~2분 뒤 `https://<아이디>.github.io/<저장소 이름>/` 주소로 열립니다.

파일은 `index.html` 하나로 동작합니다. 빌드 과정이 없습니다.

## 개인정보

- 붙여 넣은 글, 불러온 채팅 파일, 프로필 그림, 배경 그림은 **브라우저 안에서만** 처리합니다. 서버로 보내지 않고, 이 도구에는 서버가 없습니다.
- 페이지가 바깥에서 받아 오는 것은 아래의 라이브러리와 글꼴 파일뿐입니다.

## 쓰인 것들

라이브러리 (cdnjs에서 불러옵니다)

| 이름 | 쓰임 | 라이선스 |
|---|---|---|
| [html2canvas](https://github.com/niklasvh/html2canvas) 1.4.1 | 이미지로 그리기 | MIT |
| [jsPDF](https://github.com/parallax/jsPDF) 2.5.1 | PDF 만들기 | MIT |
| [Showdown](https://github.com/showdownjs/showdown) 2.1.0 | 마크다운 | MIT |
| [DOMPurify](https://github.com/cure53/DOMPurify) 3.0.6 | 붙여 넣은 HTML 정리 | Apache-2.0 / MPL-2.0 |

글꼴 (저장소에 넣지 않고, 고를 때 각 배포처에서 불러옵니다)

| 글꼴 | 만든 곳 | 불러오는 곳 |
|---|---|---|
| [Pretendard](https://github.com/orioncactus/pretendard) | 길형진 | jsDelivr |
| [Wanted Sans](https://github.com/wanteddev/wanted-sans) | 원티드랩 | jsDelivr |
| [갈무리11](https://github.com/quiple/galmuri) | 이민서 | jsDelivr |
| [페이퍼로지](https://noonnu.cc/font_page/1456) | 이주임 × 김도균 | 눈누 CDN |
| [리디바탕](https://noonnu.cc/font_page/324) | 리디 | 눈누 CDN |
| [조선굴림체](https://noonnu.cc/font_page/415) | 조선일보 | 눈누 CDN |
| Orbit, Noto Sans KR, Noto Serif KR, IBM Plex Sans KR, 고운바탕, 고운돋움, 나눔명조, 함렛 | 각 제작자 | Google Fonts |

각 글꼴의 사용 범위는 배포처의 라이선스를 따릅니다.

## 알아 둘 점

- PDF는 글자가 그림으로 들어가 텍스트 선택과 검색이 되지 않습니다. 글자를 살려야 하면 HTML로 저장하세요.
- 메시지 속 외부 링크 이미지는 그려지지 않습니다.
- 모양 이름에 나오는 카카오톡, iMessage, Safari, Windows 98은 각 회사의 상표이며, 이 도구는 그 회사들과 관계가 없습니다. 해당 모양은 색과 틀의 분위기만 빌린 것입니다.
