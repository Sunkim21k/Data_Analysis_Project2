# Data_Analysis_Project2
채용플랫폼 이용패턴 분석 팀프로젝트

# JobPlatform-Filter-A/B-Test-project

## 프로젝트 개요


- 이 프로젝트는 채용 플랫폼에서 구직자의 이탈을 탐지하고, 검색 필터 UI를 개선하여 전환율을 높이기 위한 A/B 테스트 설계를 제공하는 것을 목표로 함
- 검색 필터 사용 빈도와 전환율에 대한 분석을 통해 개선이 필요한 퍼널 단계를 파악하고, 구직자가 플랫폼 내에서 채용 공고를 검색하고 지원하는 여정을 최적화하기 위한 전략적 A/B 테스트 설계를 제안함
- 활용 기술 : Python, Tableau, Notion, Figma

### 목표

	1.	사용자 여정 분석: 플랫폼 방문부터 지원 완료까지의 사용자 여정을 분석하여 주요 이탈 지점을 파악함
	2.	필터 사용 분석: 다양한 검색 필터가 구직자의 전환에 미치는 영향을 평가함
	3.	A/B 테스트 제안: 검색 필터 UI 개선을 통해 전환율이 상승할 것이라는 가설을 검증하기 위한 A/B 테스트 설계를 제공함


### 정의된 퍼널 단계

사용자 여정은 세 가지 주요 단계로 구성됨:
	•	방문: 플랫폼에 방문한 사용자
	•	채용 공고 조회: 채용 공고를 조회한 사용자
	•	지원서 제출: 채용 공고를 조회 후 실제로 지원서를 제출한 사용자


### 데이터셋

본 프로젝트에서는 로그 데이터만을 사용하여 분석을 진행함. 로그 데이터에는 사용자 활동 기록이 포함되어 있으며, 페이지 방문, 필터 사용, 이벤트 타임 등의 정보가 담겨 있음


### 주요 분석 내용

1. 사용자 여정 분석

퍼널 분석을 통해 각 단계의 전환율을 측정하였으며, 채용 공고 조회 단계에서 지원서 제출 단계로 이어지는 구간에서 큰 이탈이 발생하는 것을 발견함. 이는 구직자가 원하는 공고를 쉽게 찾지 못하거나, 필터 사용에서 어려움을 겪고 있음을 시사함

2. 필터 사용 효과 분석

분석 결과, 직무 분야와 지역 필터는 사용 빈도가 높았지만 상대적으로 낮은 전환율을 보임. 반면, 언어 필터는 높은 전환율을 보였지만 사용 빈도가 낮아, 필터 기능 개선의 여지가 있음을 확인함

3. 클릭-to-전환 시간 분석

사용자가 채용 공고 조회에서 지원서 제출로 이어지는 시간도 분석함. 필터 사용이 클릭-to-전환 시간을 증가시키는 경향을 보이며, 이는 필터 선택 과정에서 사용자의 마찰을 의미할 수 있음


## A/B 테스트 제안

### 목표

검색 필터 UI를 개선하여 채용 공고 조회에서 지원서 제출로 이어지는 전환율을 높이는 것

### 가설

드롭다운 방식의 기존 필터 UI를 전면 배치 방식의 필터 UI로 변경하면, 사용자의 마찰이 줄어들어 지원 전환율이 증가할 것임

### 테스트 설계

	•	비교군: 기존 드롭다운 필터 UI를 사용하는 사용자
	•	대조군: 개선된 전면 배치 필터 UI를 사용하는 사용자로, 가시성과 접근성을 강화한 필터

### 성공 지표

	•	주요 지표: 채용 공고 조회에서 지원서 제출로의 전환율
	•	부가 지표: 채용 공고 조회한 사용자 중 필터 사용률
 	•	가드레일 지표: 한 달 간의 유저 평균 지원서 제출수
 
