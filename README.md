# News-Recommend-System
The 5th Future Finance A.I.Challenge 뉴스 추천시스템 공모전 참가

## 내용 요약
**사용자가 검색한 뉴스 기반으로 유사한 뉴스 추천 시스템**
    
    🔍 목적 :
    
    - 바쁜 직장인 들을 위한 목적
    
    - 상품 투자 전 빠르게 앱을 통해 (전날, 주식 개장 전) 뉴스를 확인하여 빠르게 경제 흐름 확인
    
    - 일일히 뉴스를 안 찾아봐도 빠르게 유사한 뉴스를 볼 수 있다는 장점 
    
    🔍 제공하는 이유:
    
    - 맞춤형 콘텐츠 제공
    
    - 더 높은 이용률과 유지율: 관심 있는 뉴스를 제공함으로써 사용자가 앱을 자주 이용하게 될 가능성이 높아짐. 금융 앱의 이용률과 유지율을 높일 수 있다.
    
    - 투자 결정에 도움
    
    - 경쟁 우위 제공 : 뉴스 기사 추천 시스템을 적용하는 것은 다른 금융 앱과의 경쟁에서 우위를 가질 수 있는 요소가 될 수 있다.
    
    🔍 흐름
    
    - 전날 / 주식 개장 전 ? 뉴스 가져오기 : 뉴스 기사, 링크, 본문
        - 사진에 있는 추가 설명은 제외하고 크롤링
    - 어떤 하나의 뉴스 기사 검색
    - 추천 유사도 방법론, 이런 것들 리서치 ⇒ 협업 필터링 / Bert 적용
    - 가능하다면 뉴스 본문 요약
    
    - 뉴스 기사 + 본문 내용 검색
    - 상위 10개의 기사 제목, 링크, 본문 내용 (키워드) 제공, 날짜
    - 가져올 뉴스 :
    - 네이버 증권에서 시황.전망 / 기업.종목 분석 / 해외 증시 / 채권.선물 / 환율 

    - 전처리 기준
    - 기자 이름 제거
    - 특정 불필요한 단어 제거
    - 특수 기호 제거
    - 하루 전 뉴스 / 주식 개장 전 뉴스 (예: 화욜에 추천 기사를 보고 싶으면 , 하루전 추천 뉴스 5개, 당일 추천 뉴스 5개 이런식으로)
    - 단, 월요일은 금요일 부터 월요일 개장 전 뉴스 검색
