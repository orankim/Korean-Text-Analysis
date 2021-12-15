뉴스 빅데이터를 활용한 코로나19 전후 게임관련 보도 분석
==============================================================================
토픽 모델링 중심으로
-------------------------------------------------------------------------------

### 분석 배경 및 분석 목적

- 코로나 19 팬데믹 상황에서 게임 산업은 큰 성장을 하였음
- 이는 게임이 대표 비대면 컨텐츠이기 때문으로 예상되며 각 게임 시장의 성장률을 보면 비대면으로 즐길 수 있는 게임 유형이 성장하였음을 알 수 있음 
- 이런 사실을 바탕으로 코로나19 팬데믹 사태 전인 2019년과 후인 2020년의 게임 키워드로 뉴스 기사를 토픽 모델링 방법을 활용하여 분석하여 게임 산업의 변화에 대해 분석하고자 함

### 관련 선행 연구
#### Erica Kleinman, Sara Chojnacki, and Magy Seif El-Nasr. 2021. The Gang’s All Here: How People Used Games to cope with COVID19 Quarantine. In CHI Conference on Human Factors in Computing Systems (CHI ’21), May 8–13, 2021, Yokohama, Japan. ACM, New York, NY, USA, 12 pages.
- 격리 기간에 사람들이 디지털 게임을 어떻게 이용하는지 조사
  - 연구 방법 : 트위터 포스트를 분석 -> 페이스북에서 설문조사 진행 -> 응답을 바탕으로 4개의 카테고리, 15개 테마로 분류함 
- 결과
  - People are using games to maintain mental well-being.
  - People are using games to connect with others.
  - People are using games to substitute reality.
  - People are using quarantine as an opportunity to create games.

#### Unity Technologies, Covid-19’s impact on the gaming industry : 19 takeaways, 2020
- How has the Covid-19 pandemic affected gaming habits?
  - More people are playing than ever, with a 46% DAU increase in HD gaming and 17% in mobile gaming
  - Microtransactions have grown, with IAP revenue for mobile games increasing by 24% since the pandemic was declared

- What has changed for mobile game user acquisition?
  - Mobile gamers are installing 84% more apps
  - CTR for mobile gaming ads went up 34% compared to 2019

- How has the Covid-19 pandemic affected different areas of the world?
  - Different countries showed similar performance spikes corresponding to the timing of stay-at-home restrictions

- Has the Covid-19 pandemic affected what players play?
  - Engagement on “Commuter” apps decreased 7% in volume, while mid and hardcore apps increased 39%

#### Nam, HyeonWoo. "Study on the Competitiveness Plan of the Game Industry in the Post Corona Era according to Changes of Game Platforms and Game Use Types." (2020): 137-147.
- 포스트 코로나 시대의 경쟁력 제고를 위한 게임산업의 변화 요인
  - 지속적인 모바일 게임의 발전
  - 차세대 게임 콘솔의 변화
  - 플레이하는 게임에서 보는 게임으로의 게임 이용 형태의 변화
  - 게임 마케팅의 다변화 – 게임 아이돌 마케팅

- 결론
  - 코로나19 팬데믹은 게임산업에서의 새로운 기회이며 포스트 코로나 시대에도 경쟁력을 발휘할 수 있을 것으로 예상됨
  - 클라우드 기술을 기반으로한 게임 스트리밍 서비스는 게임 개발사에게 좋은 기회이며 시장 확대에 투자가 필요함
  - 9세대 콘솔의 출시로 인해 콘솔 게임이 확대될 것으로 예상되므로 국내 게임 업계에서도 콘솔 게임 콘텐츠 확보에 주력할 필요가 있음
  - 코로나19 팬데믹으로 인해 신규 이용자들이 많이 유입되었고 이 기회를 활용해 게임 업계에서 플랫폼 다변화에 노력해야 함

### 실험 설계


#### 자료 수집
- 한국언론진흥재단에서 운영하는 빅카인즈(BIGKinds)를 활용
- 신문사 및 방송사 선정 기준 : 중앙지, 디지털 전문지, 지상파
- 검색어 : 게임
- 2019년 전체, 2020년 전체 뉴스 기사 수집
- ‘게임’은 여러 분야에서 통용되는 단어이므로 연예기사, 사건/사고 기사 등은 제외함

#### 분석 방법
- 뉴스 빅데이터 텍스트에 내재된 키워드와 토픽들을 추출하기 위해, 토픽 모델링 분석 방법 중 LDA(잠재 디리클레 할당) 기법 사용
- LDA기법은 문헌들을 구성하는 키워드들을 출현확률 및 분포에 따라 군집화하여 토픽을 추론하는 통계적 텍스트 처리 기법임
- 토픽의 수를 변경하면서 토픽 모델링을 실시한 결과, 10개의 토픽을 추출하였을 때 해석이 용이하여 토픽의 수를 10개로 설정하여 분석하였음

### 분석 결과
#### 2019년
- VR이 가장 큰 비중을 차지하며, 최근 트렌드인 클라우드 게임 역시 큰 비중을 차지함

#### 2020년
- 2019년과 동일하게 클라우드 게임의 비중이 있고, 코로나바이러스의 비중이 가장 높게 나타남
- 코로나19 팬데믹 사태로 게임 키워드 관련 뉴스 기사에서도 코로나19관련 토픽이 나타남

### 결론
#### 시사점
- 기술의 발전으로 집에서도 즐길 수 있는 VR게임이 출시되고 있으며, 이런 양상이 뉴스 기사에서 나타남
- 선행연구에서 언급했듯이, 최근 클라우드 기반으로 정기비용을 내면 즐길 수 있는 게임이 인기를 끌고있으며, 2019년 2020년 뉴스 기사에서도 관련 토픽들이 나타남
- 코로나19 팬데믹으로 인해 2019년에서는 나타나지 않은 ‘코로나＇관련 키워드가 2020년에는 높은 비중으로 나타남
- 이런 결과를 확인하였을 때 클라우드 게임과 코로나19는 게임 산업에서 무시할 수 없는 요소임

#### 분석의 한계
- ‘게임’이란 용어는 사회 전반에서 사용하기 때문에 단순히 ‘게임＇이라는 검색어로는 게임산업과 관련된 뉴스 기사만을 추출하는 데 한계가 있음
- 결과에서 스마트폰 관련 토픽이 높은 비중으로 나타나는데 이는 모바일 게임의 영향인 것으로 보이며, 해당 결과를 해석하는데 어려움이 있음
- 뉴스기사 뿐 아니라 각종 게임 커뮤니티 게시글이나 SNS를 활용하여도 관련 토픽을 파악할 수 있음
