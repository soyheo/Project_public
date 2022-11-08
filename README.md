# Project No.1

## 프로젝트의 방향 설정

- Goal :  '다음 분기에 어떤 게임을 설계해야 할까'에 대한 의사결정
- Data analyst : 게임 회사의 기획팀 대리 
- Target : 투자사
- Content :
> 1. 지역에 따라서 선호하는 게임 장르가 다를까 
> 2. 연도별 게임의 트렌드가 있을까
> 3. 출고량이 높은 게임에 대한 분석 및 시각화

## 데이터 분석 내용

**1. Data EDA & Wrangling** 
- 결측값 제거 
- Sales의 K, M값 숫자로 변환 
- 데이터 타입 변환
- Year 이상치 보정
- Total_Sales 항목 추가
- 게임 플랫폼 그룹 항목 추가
- 중복값과 그 영향의 미비함을 확인하고 유지 결정

**2. 전체 데이터 분포 확인**
<center class="half">
  <image src="https://user-images.githubusercontent.com/114864819/200472742-81995d02-1bed-46df-b730-50269c739058.png" width="30%"/>
  <image src="https://user-images.githubusercontent.com/114864819/200472764-c5d7d1c7-133d-4eb2-b470-ce39af39bf31.png" width="30%"/>
center>

**-> 0.5보다 큰 데이터가 30%나 되고, 게임산업의 특성상 경쟁이 심하고 게임별 편차가 크기 때문에 이상치로 판단하지 않는다**

**3. 테마별 데이터 분석**
> 1. 지역별 선호하는 게임 장르
<image src="https://user-images.githubusercontent.com/114864819/200473096-535575d7-4035-4e57-b632-0a33d7c7e653.png" width="30%" height="30%"/>
<image src="https://user-images.githubusercontent.com/114864819/200473179-ba9dfa6e-e9b2-4765-9bd5-3f9b44bde889.png" width="30%" height="30%"/>

**->일본과 기타 지역은 장르별 선호 유사성이 약간 있어보이고, 네개 지역 모두에서 Action이 전체적으로 상위권에 분포한다는 점을 알 수 있다**



> 2. 연도별 게임 트랜드
- 연도별 장르의 변화
<image src="https://user-images.githubusercontent.com/114864819/200477072-b85e7497-4c15-4397-9316-5eb905e7c474.png" width="30%" height="30%"/>
<image src="https://user-images.githubusercontent.com/114864819/200477202-091766cf-6cf0-4942-8ad5-5a5d29eef125.png" width="30%" height="30%"/>

- 연도별 플랫폼 변화 확인
<image src="https://user-images.githubusercontent.com/114864819/200477339-6a8e9611-6ab2-4f60-8a04-08f6f1650813.png" width="30%" height="30%"/>

- 연도별 퍼블리셔 변화 확인
<image src="(https://user-images.githubusercontent.com/114864819/200477414-7ac5c77d-e425-42d7-81fa-624c455ce5f9.png" width="30%" height="30%"/>

**장르 : 연도별 장르의 변화가 매우 다양하지만 전반적으로 Action의 비중이 높아 보인다.**

**지역 : 전 기간을 통틀어 북미시장과 유럽시장이 선전하고 있다**

**플랫폼 : 콘솔 플랫폼이 가장 크고 Portable 게임시장은 점점 감소하는 추세이다**

**퍼블리셔 : 상위 10개사의 분포를 보면 연도별 뚜렷한 독점 추세가 없이 매년 바뀌므로 경쟁이 치열한 것으로 보인다**



> 3. 출고량이 높은 게임에 대한 분석 및 시각화
- 상위 50위 게임의 전체 데이터에서의 비중 확인
<image src="(https://user-images.githubusercontent.com/114864819/200477865-077a2866-aab4-4172-92ac-4f528a537e90.png" width="30%" height="30%"/>
**상위 50개의 게임이 전체 출고량의 대부분을 차지한다는 것을 알 수 있다**

- 장르별 특징
<image src="(https://user-images.githubusercontent.com/114864819/200478144-e43603ca-a8ef-48d6-aade-3a9210d4283d.png" width="30%" height="30%"/>




