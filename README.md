# 강재훈 branch

dart.report('회사이름', '임원', '날짜') 호출 시 반환되는 피처 설명

* rcept_no : 접수번호
* corp_cls : 법인구분 Y(유가), K(코스닥), N(코넥스), E(기타)
* corp_code : 고유번호
* corp_name: 법인명
* nm: 이름
* sexdstn: 성별
* birth_ym: 생년월일
* ofcps: 직책
* rgist_exctv_at: 등기임원 여부
* fte_at: 상근 or 비상근
* chrg_job: 담당업무
* main_career: 학력, 주요경력
* mxmm_shrholdr_relate: 최대주주와의 관계
* hffc_pd: 재직기간
* tenure_end_on: 임기만료일
----
dart.report('회사이름', '최대주주', '날짜') 호출 시 반환되는 피처 설명

* rcept_no : 접수번호
* corp_cls : 법인구분 Y(유가), K(코스닥), N(코넥스), E(기타)
* corp_code : 고유번호
* corp_name: 법인명
* stock_knd: 주식의 종류
* nm: 성함
* relate: 관계
* bsis_posesn_stock_co: 분기 초 주식 수
* bsis_posesn_stock_qota_rt: 분기 초 지분율
* trmend_posesn_stock_co: 분기 말 주식 수
* trmend_posesn_stock_qota_rt: 분기 말 지분율

---
인물 네트워크 형성 기법

최대주주와의 관계를 기반으로 네트워크를 형성할 수 있습니다. 최대주주와의 관계 변수를 사용하여, 최대주주를 루트 노드로 하여 인물간의 연결관계를 파악할 수 있습니다.

회사 내부 조직 구조를 기반으로 네트워크를 형성할 수 있습니다. 직책 변수를 사용하여 회사 내부 조직 구조를 파악하고, 해당 직책에 속한 인물 간의 연결관계를 파악할 수 있습니다.

학력이나 주요 경력을 기반으로 네트워크를 형성할 수 있습니다. 학교나 회사, 기관 등을 루트 노드로 하여 해당 학교나 회사, 기관 출신 인물들 간의 연결관계를 파악할 수 있습니다.

재직 기간이나 임기 만료일을 기반으로 네트워크를 형성할 수 있습니다. 해당 변수를 사용하여, 같은 기간 동안 회사에 재직한 인물들 간의 연결관계를 파악할 수 있습니다.