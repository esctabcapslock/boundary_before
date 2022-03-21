# 한반도 과거 / 북한 행정구역 경계 SHP 파일 (2021.11~2021.12 작성)

- SHP 파일을 찾지 못해서, 한번 만들어봄
- 대충
    1. [조선시대 수륙교통로](http://waks.aks.ac.kr/rsh/?rshID=aks-2014-kfr-1230005)에서 pdf 파일 다운
    2. SHP 변환
    3. 엑셀을 이용해 다른 출처(인구 등)의 목록과 교차검증
    4. QGIS에서 일일히 수정

    하여 만듦
- 북한의 행정구역은 오픈스트리트맵을 활용

## 각 값의 뜻
- **l1**: 도명
- **l2**: 이름
- **level**: 행정구역의 등급
- **level_org**: 값이 있다면, 1454년 기준 지역이며, 아니면 1432년 기준임
- **POP**:  인구

## 1432_1454_SGG

- **세종실록지리지** 기준 행정구역 (부, 군, 현)
- 4군6진 지역은 1454년 기준 행정구역, 인구, 위계    
- 기타 지역은 1432년 기준
- 속현은 반영하지 않으며, 일부 존재하는 데이터는 주현 기준임


### 출처 (적혀진 순서대로 우선하여 반영 / 추론함)

- [조선왕조실록 세종실록지리지](http://sillok.history.go.kr/id/kda_400)
- [조선시대 수륙교통로 / 행정구역 역추적 / 성신여대 양보경(현 국토연구원) (~17)](http://waks.aks.ac.kr/rsh/?rshID=aks-2014-kfr-1230005)
- [조선시대 전자문화지도 시스템, 고려대 2007](http://www.atlaskorea.org/historymap.web)
- [경기도 600년 기념 1414~2014 : 육백년 경기도, 37p](https://memory.library.kr/items/show/28541)
- [대동여지도](https://mirror.puzzlet.org/ddy/)
- [동여도](https://kostma.aks.ac.kr/e-map/mapSearch_AN.aspx?lang=ko&mType=anciNm&sType=anSearch&sWord=DYD_15_04_0280)
- [신증동국여지승람](https://db.itkc.or.kr/dir/item?itemId=BT#dir/node?grpId=&itemId=BT&gubun=book&depth=2&cate1=G&cate2=&dataGubun=%EC%84%9C%EC%A7%80&dataId=ITKC_BT_B001A)
- [한국민족문화대백과사전](http://encykorea.aks.ac.kr)
- [한국어 위키백과 지역정보](https://ko.wikipedia.org)
- [정요근.(2014).\[한국사\] GIS 기법의 활용을 통한 조선후기 越境地의 복원.역사학보,224(),109-162.](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE06071914)

### 참고사항

- 일부 경계는 1789_EMD 파일을 기준으로 경계를 추론하였음
- 그 장소는  다음과 같음
    1. 전라도 장성-진원 경계
    1. 평안도 의주-인산-정령 경계
    1. 평안도 정주-수천 경계
    1. 황해도 우봉-강음
    1. 각종 속현 지역

## 1789_EMD
- **호구총수(1789)** 시기의 행정구역 (읍, 면 단위)
- PDF 파일을 SHP 파일로 변환한 것

### 출처
- [조선시대 수륙교통로 / 행정구역 역추적 / 성신여대 양보경(현 국토연구원) (~17)](http://waks.aks.ac.kr/rsh/?rshID=aks-2014-kfr-1230005)
## 1789_SGG

- **호구총수(1789)** 시기의 행정구역 (부, 군, 현 단위)

### 참고문헌
- **1432_1454_SGG**과 같음

## 1912_EMD

- PDF 파일을 SHP 파일로 변환한 것
### 출처
- [조선시대 수륙교통로 / 행정구역 역추적 / 성신여대 양보경(현 국토연구원) (~17)](http://waks.aks.ac.kr/rsh/?rshID=aks-2014-kfr-1230005)

## 1912_SGG

- 부군면 통폐합 직전의 행정구역도
- 행정구역 경계만 나와 있어 구체적인 이름을 타이핑한 것임

### 출처
- [정요근.(2014).\[한국사\] GIS 기법의 활용을 통한 조선후기 越境地의 복원.역사학보,224(),109-162.](https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE06071914)
- [조선시대 수륙교통로 / 행정구역 역추적 / 성신여대 양보경(현 국토연구원) (~17)](http://waks.aks.ac.kr/rsh/?rshID=aks-2014-kfr-1230005)
- [조선시대 전자문화지도 시스템, 고려대 2007](http://www.atlaskorea.org/historymap.web)
- [한국민족문화대백과사전](http://encykorea.aks.ac.kr)
- [한국어 위키백과 지역정보](https://ko.wikipedia.org)

## 2008_SGG

- 통계정보서비스의 파일을, 휴전선에 맞추어 다듬은 파일임
- 휴전선은 오픈스트리트 맵을 활용
- [여기서](https://github.com/vuski/admdongkor)도 그냥 공개한 것을 보아, 본인도 그냥 공개함
- 법정동 코드 변환표 첨부됨

### 출처
- [통계지리정보서비스 2008년 센서스용행정구역경계 ](https://sgis.kostat.go.kr/contents/shortcut/shortcut_05.jsp)
- [오픈스트리트맵 휴전선](https://openstreetmap.org/)
- [오픈스트리트맵](https://openstreetmap.org/)
- [경계 다운로드](polygons.openstreetmap.fr)
- [해안선 다운로드](https://osmdata.openstreetmap.de/data/land-polygons.html)

## 사용 유의사항
- (2022.03 보완) 일제강점기 이후 경기, 강원, 충청, 황해도의 공신력있는 행정구역 자료: [국사편찬위원회 역사정보지리DB 사업](http://db.history.go.kr/hgis/pro_g1/intro/intro01.do)
- 파일이 사실관계와 많이 다를 수 있으며, 이에 따른 책임은 본인에게 있음
- 본인이 임의로 업데이트 할 수 있음
- **사실관계가 다른 경우**, 본 깃헙의 [이슈](https://github.com/esctabcapslock/boundary_before/issues)나 [pull requests](https://github.com/esctabcapslock/boundary_before/pulls)기능 등을 이용해 많은 사람들이 혜택을 볼 수 있으면 좋겠음
- 위와 같은 이유로, 사용시 출처를 남기길 권장함

