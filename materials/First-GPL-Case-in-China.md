# First GPL Case in China
## 출처
1. https://heathermeeker.com/2018/04/30/first-gpl-case-in-china-or-is-it/
2. http://www.bjcourt.gov.cn/cpws/paperView.htm?id=100734294859&n=1

## 경과
### plaintiff
"Digital Heaven Internet Technology CO., LTD"
1. HBuilder를 개발하여 shareware로 공개
	- HBuilder내 module
		- Aptana : [https://github.com/aptana/studio3](https://github.com/aptana/studio3) - GPL-3.0
		- CIM plugin, ACR plugin, HTML code drawing in real time plugin : licensing term 명시 없음
2. defendant가 APICloud라는 project를 개발하며 사전 서면 허가 없이  HBuilder의 source code 일부분을 가져갔음을 발견
3. defendant를 copyright infringement로 고소
### defendant
"Pomelo Technology CO., LTD"
1. "HBuilder"내 module중 하나(Aptana)가 GPL이기 때문에 total solution은 GPL로 제공되야 함
2. 따라서, HBuilder의 일부 code를 GPL하에서 개발하는 APICloud에 사용하는 것은 문제되지 않음을 주장
## 법원 의견
1.  GPL은 중국에서 enforceable함. 단, Copyleft가 어떻게 해석될 수 있는지는 case-by-case로 결정되어야함
2.  defendant가 허락없이 사용한 plaintiff의 개발 module(CIM plugin, ACR plugin, HTML code drawing in real time plugin)은 직접적으로 "Aptana"를 기반으로 개발된 것이 아님
    -   오히려, 이 3개의 module은 "HBuilder"내에서 Eclipse framework를 기반으로 하는 "Aptana" plugin과 같은 독립 module로 구현됨
3.  GPL-3.0에서 "aggregation"과 "derivative"는 구분이 됨
    -   plaintiff에 의해 개발된 module과 GPL licensed "Aptana"의 관계는 "aggregation"임
## 법원 판단
1.  plaintiff가 개발한 3개의 module은 plaintiff의 선택에 따라 release될 수 있음 (GPL로 license될 필요 없음)
2.  plaintiff는 이들을 GPL-3.0으로 제공한 적이 없음
    -   "HBuilder"내 이 세 module의 sub-folder에는 어디에도 copyright notice 혹은 license text가 없음
3.  copyright infringement로 인해 plaintiff에게 보상이 되어야함 : 1,250,000 RMB (약 165,000 EURO), 변호사 및 절차 비용 별도
