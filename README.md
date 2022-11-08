# Project No.1

## 프로젝트의 방향 설정

- Goal :  '다음 분기에 어떤 게임을 설계해야 할까'에 대한 의사결정
- Data analyst : 게임 회사의 기획팀 대리 
- Target : 투자사
- Content :
> 1. 지역에 따라서 선호하는 게임 장르가 다를까 
> 2. 연도별 게임의 트렌드가 있을까
> 3. 출고량이 높은 게임에 대한 분석 및 시각화
> 4. 데이터 

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

<image src="https://user-images.githubusercontent.com/114864819/200472742-81995d02-1bed-46df-b730-50269c739058.png" width="30%" align="left">
<image src="https://user-images.githubusercontent.com/114864819/200472764-c5d7d1c7-133d-4eb2-b470-ce39af39bf31.png" width="30%">

**-> 0.5보다 큰 데이터가 30%나 되고, 게임산업의 특성상 경쟁이 심하고 게임별 편차가 크기 때문에 이상치로 판단하지 않는다**

**3. 테마별 데이터 분석**
> **1. 지역별 선호하는 게임 장르**      
                                                                                                                                       
<image src="https://user-images.githubusercontent.com/114864819/200473096-535575d7-4035-4e57-b632-0a33d7c7e653.png" width="30%" height="30%" align="left">
<image src="https://user-images.githubusercontent.com/114864819/200473179-ba9dfa6e-e9b2-4765-9bd5-3f9b44bde889.png" width="30%" height="30%">

**->일본과 기타 지역은 장르별 선호 유사성이 약간 있어보이고, 네개 지역 모두에서 Action이 전체적으로 상위권에 분포한다는 점을 알 수 있다**



> **2. 연도별 게임 트랜드**

- 연도별 장르의 변화          
                                                                                                                                            
<image src="https://user-images.githubusercontent.com/114864819/200477072-b85e7497-4c15-4397-9316-5eb905e7c474.png" width="30%" height="30%" align="left">
<image src="https://user-images.githubusercontent.com/114864819/200477202-091766cf-6cf0-4942-8ad5-5a5d29eef125.png" width="30%" height="80%">

- 연도별 플랫폼 변화 확인

<image src="https://user-images.githubusercontent.com/114864819/200477339-6a8e9611-6ab2-4f60-8a04-08f6f1650813.png" width="30%" height="30%"/>

- 연도별 퍼블리셔 변화 확인
                                                                                                                                            
<image src="https://user-images.githubusercontent.com/114864819/200477414-7ac5c77d-e425-42d7-81fa-624c455ce5f9.png" width="30%" height="30%"/>

**->장르 : 연도별 장르의 변화가 매우 다양하지만 전반적으로 Action의 비중이 높아 보인다. <br> 지역 : 전 기간을 통틀어 북미시장과 유럽시장이 선전하고 있다 <br> 플랫폼 : 콘솔 플랫폼이 가장 크고 Portable 게임시장은 점점 감소하는 추세이다 <br> 퍼블리셔 : 상위 10개사의 분포를 보면 연도별 뚜렷한 독점 추세가 없이 매년 바뀌므로 경쟁이 치열한 것으로 보인다**


> **3. 출고량이 높은 게임에 대한 분석 및 시각화**
- 상위 50위 게임의 전체 데이터에서의 비중 확인
                                                                                                                                            
<image src="https://user-images.githubusercontent.com/114864819/200477865-077a2866-aab4-4172-92ac-4f528a537e90.png" width="30%" height="30%"/>

**->상위 50개의 게임이 전체 출고량의 대부분을 차지한다는 것을 알 수 있다 -> 소수의 게임들만이 독식한다**

- 장르별 특징
                                                                                                                                            
<image src="https://user-images.githubusercontent.com/114864819/200478144-e43603ca-a8ef-48d6-aade-3a9210d4283d.png" width="30%" height="30%"/>

- 플랫폼별 특징
                                                                                                                                            
<image src="https://user-images.githubusercontent.com/114864819/200478431-9f829a98-0e19-4f7f-b9ce-676749038bf6.png" width="30%" height="30%" align="left">
<image src="https://user-images.githubusercontent.com/114864819/200478393-74ea2c3a-0df9-4ca3-a6ec-7a1a90937993.png" width="30%" height="100%">

- 퍼블리셔별 특징

<image src="https://user-images.githubusercontent.com/114864819/200478665-565acc71-39e2-4410-b005-98b8dad7649e.png" width="40%" height="100%" align="left">
<image src="https://user-images.githubusercontent.com/114864819/200478712-fd253e6f-faea-4b76-8288-305aa4255aae.png" width="30%" height="20%">

**->출고량이 높은 상위 50개 게임 분석 요약 : 가장 많이 사용된 플랫폼이 이고 콘솔이고, 2007년과 2013년도에 게임 출고량이 다소 많다는 걸 알 수 있다. 퍼블리셔는 Electronic Arts가 가장 출고량이 많으며 Activision이 뒤따르는데 두 퍼블리셔별 개발 장르는 다양하다. 전체 상위 50개 게임의 장르는 Action이 가장 큰 부분을 차지한다. Action장르의 다른 장르와의 상관관계는 전혀 없어 보인다.**


**4. 결론 : 다음 분기에 어떤 게임을 출시할까?**
  
-Action/Shooter 장르 </br> -콘솔 플랫폼, 그러나 2015년 이후 데이터가 없어 분석할 수 없었지만 현재 게임시장에서 큰 파이를 차지하는 모바일 플랫폼 활용도 고려 </br> -Electronic Arts사/Ubisoft의 액션/슈팅 게임을 참고하여 개발하도록 함

**5. 한계**
  
  - 모바일 게임 데이터 취합이 안되어 현재 시장 흐름 반영의 어려움
  - 데이터 분석을 통해 지역별, 플랫폼별로 굉장히 **fregmented**된 게임시장의 특성을 확인할 수 있는데 </br> 모든 지역을 타깃으로 한 장르의 게임을 선택하여 개발하는 것은 매우 어렵고 지역에 따라 맞춤 개발이 적합해 보이나 다품종 개발이 현실상의 어려움
  - 멀티플랫폼으로 운용되는 게임의 경우 주력으로 하는 플랫폼에 집중된 판매량을 보이는데, 그에 대한 데이터분석과 전략의 부재
  

