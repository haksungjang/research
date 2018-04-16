# Oracle v Google -- new decision (2018-03-28)

- 2010년
  - Oracle이 Google을 상대로 저작권 침해 소송 제기 (이유 : Google이 Android를 만들면서 Java API 37개를 무단 도용)
- 2012년 5월,
  - 1심 (캘리포니아 북부 지역 법원) : Google 승리. Java API를 쓴 것은 저작권 침해가 아니라는 판결
  - 곧바로 Oracle 항소
- 2014년 5월
  - 2심 (연방 항소 법원) : Oracle 승리. Java API도 저작권 보호 대상이라고 판결
    - 한가지 유예 조건 추가 : Google의 저작권 침해 행위가 저작권법상의 공정 이용 (Fair Use)에 해당되는지 논의해보라면서 사건을 1심 법원으로 되돌려 보냄.
  - Google이 대법원에 상고
- 2015년 6월
  - 연방 대법원 : Google의 상고 신청을 받아들이지 않음.
- 2016년 5월
  - 캘리포니아 북부 지역 법원 : Google의 Java API 이용은 저작권법상의 공정 이용에 해당된다는 취지의 판결
  - Oracle 항소 (2016년 10월)
- 2018년 3월
  - 연방 항소 법원 : Google의 Java API 이용은 공정 이용으로 인정할 수 없다는 판결
- (추후)
  - 샌프란시스코 지역법원으로 무대를 옮겨 Google이 Oracle에 지불할 배상금 액수를 산정하는 또 다른 재판을 하게 됨 (Oracle은 그 동안 저작권을 침해한 Google에 90억 달러를 배상해달라고 요구해옴)

- References :  [http://www.zdnet.co.kr/news/news\_view.asp?artice\_id=20180328141031](http://www.zdnet.co.kr/news/news_view.asp?artice_id=20180328141031)

# Google vs. Oracle, 제2라운드

출처 : [http://www.helloiplaw.com/598](http://www.helloiplaw.com/598)

(아래내용은위출처의글을개인학습을위해단순히정리한내용입니다. 내용에대한저작권은위출처글의작성자에게있음을알립니다.)

## 1.배경

- Java2 SE (Standard Edition)

-
  - --Sun Microsystems가개발
  - --Oracle이매입

- API (Application Programming Interface)

-
  - --공통적이고반복적인컴퓨터기능들을구현

- Java Programming 언어자체는누구든지허락을받을필요없이무료로사용가능
- Oracle은경쟁Platform이나Embedded 기기에Java API를사용하는데에는License 비용을부과하고있음

- Google
  - 2005년Android 인수하여Mobile 기기를위한새로운Software Platform 개발착수
  - Java Platform사용에관한License 계약체결을위해Sun Microsystems와협상돌입 -&gt; 결론없이무산
  - 자체적으로API개발시도 -&gt; 그성과가여의치않았음
  - License를체결하지않은채 Java 채택
  - 37개의Java API package에서 11,500줄에달하는declaring code를그대로차용
  - Java API package의SSO (Structure, Sequence, Organization)을그대로베껴서Android 운영체제개발및공개

## 2. 법적논쟁

- 2010년
  - Oracle은Java에관한특허와저작권법을근거로캘리포티아주북부연방지방법원에Google을대상으로침해의소를제기
  - Google은저작권침해에관하여는fair use의방어법리를들며Java API사용이정당함을주장
  - 특허에관한부분은비침해로결론
  - 저작권에관해서도API package는저작권의대상이아니라는법적결론
    - 저작권자체가성립을하지않는다고결론이내려짐에따라fair use인지에관한판단도미뤄짐

- 2013년
  - Oracle 항소
  - 연방순회항소법원에서Oracle 첫승리
  - 항소법원은Program code와SSO 역시저작권의보호를받을수있다고판결 (하위심의판결을뒤집음)

- Google은연방대법원에저작권문제에관하여항소신청 (petition for certiorari) -&gt; 대법원은이신청을거절

- 결국이사건은 1심으로다시환송이되어다음issue인fair use에관한사항이쟁점이됨

- 두번째사실심
  - Google승리
  - Java API 사용이정당한것으로인정을받음
  - Oracle 두번째항소 (첫번째항소와는다른사안)
    - Computer code와SSO가저작권의보호대상이냐의문제에관한것이기때문에fair use에관한별개의문제로재차항소하는것이가능했음

- 결론 : 연방순회항소법원은두번째항소심에서도하위심의판결을번복하며Oracle의손을들어줌
  - 즉, Google의사용이fair use에관한방어법리로정당화될수없다는것이그요지

## 3. Fair Use

## 4. 맺음말

- 당연한수순
  - Google이연방순회항소법원에서전원합의체(en banc)판결을신청하거나
  - 대법원에항소신청(petition for certiorari)
- 그러나, 이러한신청이받아들여질가능성은미미해보임
- fair use가모든저작권침해방어에사용할수있는만병통치약이아님을확인
- fair use의법리만믿고악의의침해사용을하는것은매우위험
- fair use에관한결론은재판관의재량과각사건의사실관계에따라예측하기가어려움
  - 소송지역에따라적용되는법리가미묘하게달라서결과역시조금씩달라질수있음
- 본사건의판례로인해computer code에fair use의방어법리를사용할수없다는뜻은아님.
  - 연방순회항소법원역시본판례는&quot;computer code를도용하는경우에fair use defense가절대로성립할수없다는것은아니다.&quot; 라고분명히못을박고있음
