# 성심당 방문객 이동경로 및 소비 패턴 분석을 통한 지역 경제 활성화 방안 제안

## 중구, 맞춤형 관광 추천 시스템을 통한 새로운 관광 경험 제안

본 프로젝트는 대전의 대표적인 관광지인 **성심당**을 중심으로, 방문객들의 **이동 경로** 및 **소비 패턴**을 데이터 기반으로 분석하여, **중구 지역 경제 활성화**와 **관광 산업 발전**을 촉진할 수 있는 정책적 방안을 제시하는 것을 목표로 합니다. 성심당 방문객의 구체적인 소비 행태를 분석함으로써 중구 내 상권 활성화와 **소상공인과의 상생 효과**를 극대화하는 전략을 도출합니다.

## 프로젝트 개요

### 배경
성심당은 그 독특한 역사와 맛으로 인해 대전광역시를 대표하는 관광 명소로 자리 잡았으며, 많은 관광객이 방문하고 있습니다. 그러나 대다수의 방문객은 **성심당 방문 후 중구 지역을 떠나는 경향**을 보이고 있으며, 이로 인해 중구 관광 수요는 **최하위 수준**을 기록하고 있습니다.

이에 본 프로젝트는 데이터를 활용해 성심당 방문객들의 **이동 경로** 및 **소비 패턴**을 분석하고, 이를 바탕으로 **중구 지역 관광 활성화 및 상권 발전을 위한 맞춤형 정책**을 제안하는 데 목적이 있습니다.

### 목표
- **성심당 방문객의 이동 경로 및 소비 행태 분석**: 방문객의 유동 경로를 파악하여 주요 소비 지점 및 상권과의 연결성을 도출
- **지역 상권과의 상생 도모**: 관광객의 소비 패턴을 분석하여 소상공인과의 상생 효과를 극대화할 수 있는 전략 제안
- **맞춤형 관광 추천 시스템 구축**: 분석 결과를 바탕으로 중구 관광지와 상권에 대한 추천 시스템을 개발하여 방문객의 만족도를 제고하고, 중구 지역 경제 활성화에 기여

## 데이터 개요

### 사용 데이터
- **성/연령별 유동인구 데이터**: 셀별, 행정동별, 일별, 시간별 데이터를 바탕으로 성별 및 연령대별 유동 인구 파악
- **하나카드 가맹점 실적 정보**: Cell ID별 업종별 가맹점 실적 정보 분석을 통한 소비 패턴 파악
- **하나카드 지역별 업종 유입 고객 및 상권 특성 정보**
- **국토조사 500M 빈격자 데이터**
- **소상공인시장진흥공단 상가(상권) 정보**
- **국내 지역별 주요 관광 명소 데이터**

### 데이터 전처리 과정
1. **격자 생성**: 50m x 50m 격자 생성 후 행정동 기준으로 변환하여 결합
2. **격자 병합**: 격자 ID 기준 병합 후 대전 중구의 데이터 추출
3. **월별 데이터 병합 및 업종 소분류 매핑**: 소비 데이터를 월별로 병합하고 업종 소분류를 매핑
4. **결측치 처리**: 시군구 유입 결측치 제거 및 업종 중분류 'NaN' 값을 '기타'로 처리하여 분석에 활용

## 분석 방법론

### K-Means 클러스터링
- **K-Means 알고리즘**을 통해 방문객의 이동 패턴을 분석하여, 유동인구가 집중되는 주요 지역과 상권을 효과적으로 분류하였습니다. 이 분석을 통해 특정 시간대나 구역에서 인구 밀집도가 높은 지역을 파악하고, 중구 내 **핵심 상권**을 식별할 수 있었습니다.

### 주요 분석 결과
1. **유동 인구 집중 지역**: 서대전역 인근 문화동이 유동 인구 비율이 가장 높았으나, **성심당을 포함한 격자와 그 인근 지역**이 중구 상권의 중심부임을 확인
2. **방문객 소비 패턴**: 충남, 경기, 서울, 세종 지역에서 많은 방문객이 유입되었으며, 성심당을 중심으로 한 상권이 대전 중구의 주요 소비지로 작용
   - 타지인 방문객의 소비 활동은 주로 음식점업에 집중되었으며, 이들이 중구 지역 경제에 미치는 긍정적 영향이 크다는 것을 확인하였습니다.

## 추가 분석: 인기 격자 분석
- **관광지 중심 분석**: 관광지를 중심으로 한 소비 패턴을 분석하여 **소상공인 상권**과의 연계 가능성을 도출하였습니다. 이를 바탕으로 격자 기반 행정동 연계 소비 정보를 통해 방문객 특성에 맞는 **소비 유도 전략**을 제안할 수 있습니다.

## 최종 결과 및 기대 효과

### 결과 요약
본 분석을 통해 성심당 방문객들의 이동 경로 및 소비 패턴을 심층적으로 파악할 수 있었으며, 성심당과 그 인근 지역이 중구의 핵심 상권으로 자리매김하고 있음을 확인하였습니다. 방문객의 소비 활동이 지역 경제에 큰 영향을 미치는 것으로 분석되어, 이를 바탕으로 **지역 경제 활성화**와 **소상공인과의 상생**을 도모할 수 있는 맞춤형 정책을 제안합니다.

### 기대 효과
- **상권 활성화**: 성심당과 주변 상권의 유기적 연계를 통한 지역 경제 활성화 방안 도출
- **맞춤형 관광 추천 시스템 구축**: 방문객의 소비 패턴에 맞춰 관광지와 상권을 추천하는 **데이터 기반 맞춤형 관광 추천 시스템** 제안
- **정책 제안**: 성심당을 중심으로 한 **대전 중구 상권 활성화 정책**을 기반으로 관광객 유입을 확대하고, 중구 지역의 지속 가능한 발전을 도모할 수 있습니다.

---

본 프로젝트는 **성심당**을 중심으로 한 **지역 상권의 발전 모델**을 제시하며, 이를 통해 **대전광역시 중구의 관광 및 경제 활성화**에 실질적으로 기여할 수 있는 방안을 구체화하였습니다.
