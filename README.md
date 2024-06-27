# Final_Pjt

## 1. 팀원 정보 및 업무 분담 내역
  - 공통업무
    1. 프로젝트 기획 
    2. 프로젝트 레이아웃 초안 작성
    3. 홈페이지 디자인(css)

  - 나의 담당 주요 업무
    1. DB관리 
    2. ERD 설계
    3. 영화 추천 게임 구현 (장르별 이상형 월드컵)
    3. 좋아요, 팔로우, 유저 기능 구현
    4. 영화 장르 데이터처리

  -  주요 업무
    1. API 사용 처리 (youtube API, TMDB API)
    2. 동영상 편집 및 이미지 편집
    3. 영화 추천 알고리즘 구현 
    4. UI/UX 
    
---

## 2. 목표 서비스 구현 및 실제 구현 정도
  - 목표 서비스
    1. 홈페이지 기본 기능 구현(o)
    2. 검색을 통한 영화찾기 기능 구현(o)
    3. 장르에 따른 영화목록 구성(o)
    4. 자유게시판, 댓글 및 커뮤니티 기능(o)
    5. YOUTUBE API 요청을 통한 동영상 렌더링(o)
    6. 유저 프로필, 이미지 추가(o)
    7. 유저 간의 팔로우, 유저의 영화 좋아요 기능(o)
    8. 유저의 영화 별점 기능(x)
    9. 구글 로그인, 카카오 맵 기능(x)
    10. 대댓글 기능(x)

---

## 3. 데이터베이스 모델링(ERD)
<img src="./ERD.png">
---

## 4. 영화 추천 알고리즘에 대한 기술적 설명
  1. 영화 장르 선택 기능
  <br>
  - movie 와 genres 모델간의 many to many fields를 설정
  - genres의 key, value값 데이터를 처리하여 원하는 장르를 고를 수 있게함
  - genre에 맞는 리스트들을 저장하여 웹에서 버튼을 통해 화면에 보여주도록 설정

  2. 영화 월드컵게임
  <br>
  - 게임을 통해 영화의 포스터만으로 유저가 장르를 세분화 할 수 있도록 설정
  - 전체 movie 리스트에서 랜덤으로 뽑아내어 두 개씩 정보를 보여주면서 토너먼트 식으로 하나의 작품이 나올 수 있도록 구성
  - 마지막으로 하나의 영화의 장르의 데이터를 추출하여 해당 장르의 영화중 4개의 작품을 랜덤으로 뽑아 추천

---

## 5. 서비스 대표 기능에 대한 설명
  1. 검색 기능
  - 제목과 내용에서의 검색한 내용이 포함되면 해당하는 영화 리스트를 가시적으로 보여줌
  2. 유저간 팔로우 기능
  - 유저의 팔로우를 통해 유저간 팔로워, 팔로잉 숫자를 나타냄
  3. 영화 좋아요 기능
  - 각 유저의 영화 좋아요를 누름으로써 프로필에서 유저가 좋아요를 누른 영화의 리스트들을 평점 높은 순으로 추출
  4. 자유 게시판, 영화 디테일 에서의 댓글 기능
  - 커뮤니티 활성화를 통해 유저 간 소통가능
  5. YOUTUBE 동영상
  - 디테일에서 영화의 제목, 내용, 평점으로는 어떤 영화인지 판별이 불가하다고 생각해 예고편 동영상을 통해 영화에 대한 이해도를 높임
  6. 로그인, 회원가입, 회원탈퇴
  - 회원가입을 통한 유저의 로그인의 유무에 따라 커뮤니티 기능 사용 유무 판별
---
