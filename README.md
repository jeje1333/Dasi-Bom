# Project: 다시, 봄
## 화면 보기
<details>
<summary><strong>📸 전체 화면 미리보기</strong> (클릭하여 보기)</summary>

| 구분 | 화면 | 미리보기 |
|------|------|----------|
| 공통 | 로그인 | <img height="300" alt="image" src="https://github.com/user-attachments/assets/eb962efa-8770-4d1f-9f20-31300461ef0e" /> |
| 관리자 | 관리자 메인 | <img height="300" alt="관리자페이지" src="https://github.com/user-attachments/assets/e9390e21-fc57-40cf-93fc-450fa8b5bc49" /> |
| 관리자 | 가게 관리 | <img height="300" alt="가게관리" src="https://github.com/user-attachments/assets/7d6bd95a-baca-4028-9777-993e424b440c" /> |
| 관리자 | 메뉴 관리 | <img height="300" alt="image" src="https://github.com/user-attachments/assets/398c9fd3-d574-416d-a59c-24f3791d90af" /> |
| 관리자 | 예약 확인 | <img height="300" alt="예약확인" src="https://github.com/user-attachments/assets/060e4a7d-a70d-4855-9f5f-7a599f55feb9" /> |
| 사용자 | 유저 메인 | <img height="300" alt="image" src="https://github.com/user-attachments/assets/0c799022-c865-41a0-8a1c-3cfa72eaf60e" /> |
| 사용자 | 예약 | <img height="300" alt="image" src="https://github.com/user-attachments/assets/aa43a009-59de-40aa-adb5-64e45514bc6d" /> |
| 사용자 | 예약 확인 | <img height="300" alt="image" src="https://github.com/user-attachments/assets/69089844-d290-463c-a331-296d40e89f01" /> |
</details>

## 기획 의도
숏폼, 영상에 익숙해진 사람들이 다시 책에 관심을 가질 수 있도록 ‘다시 봄’은 
도서 구매 쇼핑몰을 기반으로 커뮤니티, 중고거래, 이벤트, 굿즈샵 등을 결합하여 
독서의 다양한 즐거움을 제공하는 것을 목표로 했습니다.  

## 개발 개요
﻿2025.06.10 ~ 2025.06.30 (총 21일)  
팀원 수: 6명

## 개발 소요
- 도서 검색 및 추천 (네이버 API 활용)  
- 굿즈샵 기능 (장바구니/결제 플로우 포함)  
- 도서·굿즈 장바구니 관리  
- 커뮤니티 게시글 및 댓글 기능  
- 중고거래 페이지 개발  
- 출석체크 이벤트 팝업  
- 이벤트 페이지 운영 

## 맡은 역할
- **팀장**: 프로젝트 일정 관리 및 협업 조율  
- **문서 정리**: 개발 계획서, ERD, 기능 명세서 등 작성 및 관리  
- **서비스 설계**: 유스케이스, 다이어그램, ERD 설계  
- **기능 구현**: 네이버 API 기반 도서 검색 기능 개발  

## 사용 기술 스택
| 구분        | 기술 |
|-------------|------|
| 언어        | Java |
| 프레임워크  | Spring Legacy |
| DB          | Oracle 18c, MyBatis |
| 프론트엔드  | JSP, JSTL |
| 백엔드      | Spring MVC, REST API |
| 설계 도구   | Figma, Pencil(UI), dbdiagram.io(ERD) |

## 프로젝트 자문자답
#### Q1. 프로젝트를 진행하면서 가장 힘들었던 일은?
첫 조장을 맡은 프로젝트였던 만큼 일정 관리와 팀원 간 조율이 가장 어려웠던 것 같습니다.
팀원으로 참여했을 때는 맡은 일만 성실히 하면 되었지만 팀장이 되니 업무를 분배하고 진행 상황을 관리하는 책임이 생겼습니다. 
특히 팀원의 역량과 상황을 고려해 적절히 일을 나누는 것이 쉽지 않았습니다. 하지만 이 과정을 통해 의사소통 능력과 협업 조율 능력을 키울 수 있었습니다.

#### Q2. 본인이 개발한 도서 목록 페이지에 대한 상세한 설명
도서 목록 페이지는 네이버 도서 검색 API에서 가져온 데이터를 JSTL을 활용해 JSP에 출력하는 방식으로 구현했습니다.
검색 결과가 많아질 경우를 대비해 한 페이지에 10개씩 출력되도록 페이징 처리를 적용했으며, 
검색어 입력 → API 호출 → JSON 데이터 파싱 → JSP 출력까지의 흐름을 명확히 설계했습니다.

#### Q3. 프로젝트에서 가장 기억에 남는 문제 해결 경험은 무엇인가요?
협업 과정에서 팀원들이 AI 기반 코드 작성 툴을 많이 활용했는데, 그 과정에서 예상치 못한 문제가 발생했습니다.
코드를 작성하던 중 설정 파일에 UpperToCamelCase 옵션을 True로 지정하게 되었는데 
코드를 병합하는 과정에서 이 설정이 프로젝트 환경과 충돌을 일으켰습니다. 
정상적인 코드가 실행되지 않고, 오히려 잘못 작성된 코드가 작동하는 역전 현상이 발생한 것입니다.
문제가 코드 로직이 아니라 설정 파일에 숨어 있었기 때문에 원인을 찾는 데 시간이 오래 걸렸었습니다. 
원인을 발견한 후에는 회의를 열어 상황을 공유했고, Mapper의 올바른 사용법(주로 CRUD에 관해)을 직접 정리해 교육을 진행했습니다.

#### Q4. 프로젝트를 진행하면서 가장 아쉬웠던 일은?
버전 관리가 가장 아쉬웠습니다. 원래는 하루에 한 번씩 팀 전체 버전을 업데이트하며 동기화를 맞췄어야 했는데, 
일정에 쫓기다 보니 이를 제대로 지키지 못했습니다. 그 결과, 팀원들이 서로 다른 기준 버전에서 개발을 이어가게 되었고, 
잘못된 방향을 제때 수정할 기회를 놓치게 되었습니다.
특히 프로젝트 후반부 병합 과정에서 충돌이 대량으로 발생해 조율과 수정에 많은 시간이 소요되었습니다. 
이 경험을 통해 단순히 코드를 작성하는 것 이상으로, 지속적인 버전 관리와 팀 단위의 코드 동기화가 프로젝트 성공에 핵심적이라는 점을 크게 깨달았습니다.

#### Q5. 프로젝트를 진행하면서 가장 인상깊었던 일은?
6명이서 21일동안 프로젝트를 진행했는데 만든 페이지가 정말 많습니다.
그건 바로 팀원들이 야근을 열심히 해 주었기 떄문에
하지만 그 과정이 즐거웠습니다




## 프로젝트 관련 자료
[발표 PPT](https://docs.google.com/presentation/d/1p_OsoSNuF4TKWMCrN96TpJ6Qjzo4gyFD)  
[시연 동영상](https://drive.google.com/drive/folders/1Bnl7pMzE9mVtjxdJEZ7Ls_EgKEgRhBSn)  
[프로젝트 ERD](https://drive.google.com/drive/folders/1Bnl7pMzE9mVtjxdJEZ7Ls_EgKEgRhBSn)  
[화면 설계 및 기능 명세서](https://drive.google.com/drive/folders/1Bnl7pMzE9mVtjxdJEZ7Ls_EgKEgRhBSn)  
[프로젝트 개발 계획서](https://docs.google.com/document/d/1-Eby-sEILRy170nCE783xbKEqkqOgwbw)  
 
