출처 : Report from the Geniatech vs. McHardy GPL violation court hearing - http://laforge.gnumonks.org/blog/20180307-mchardy-gpl/

# 2018-03 Geniatech vs. McHardy

(2018년 3월7일, 고등법원의 공개 구두 심리에 참석했던 Harald Welte가 본
case에 대해 작성한 report를 정리함)

# 1. History of the Case

-   원고 : Patrick McHardy

-   피고 : Geniatech
    ([*https://www.geniatech.com/contact-us/*](https://www.geniatech.com/contact-us/))

    -   본사 - 중국 심천

    -   유럽 지사 (독일 위치) - Geniatech Europe GmbH

    -   위성 TV 수신기

    -   Geniatech Europe CEO : "과거에 GPL incompliance가 있었음을
        공개적으로 인정하지만, preliminary injunction (예비 금지
        명령)에서의 주장은 지나치게 광범위한 것임"

경과
----

1.  2017년 7월

    -   Patrick McHardy는 Geniatech Europe product 구매하고, 이 제품이
        GPL-2.0 침해를 발견함

        -   명백하게 binary와 함께 source code (혹은 written offer)가
            제공되지 않았음

        -   이는 license 조항 위반임으로 저작권 침해임

    -   원고는 쾰른 지방 법원에 피고에 대한 preliminary injunction 요청

2.  2017년 9월 8일

    -   preliminary injunction 부여

    -   (참고: 독일의 legal procedure) 

        -   원고가 preliminary injunction을 신청하면, 간단한 검토 후
            즉시 부여됨 (구두 심리에서 피고인의 말을 듣는 과정 없이)

        -   피고가 preliminary injunction에 항소하기를 원하면, 항소를
            제기하여 구두 심리(court hearing)를 함

    -   피고가 preliminary injunction에 대해 항소

3.  2017년 10월 20일

    -   쾰른 지방 법원은 injuction (금지 명령)을 부분적으로 지지하는
        판결을 내림

    -   피고는 고등법원 (OLG Cologne)에 위의 판결을 철회할 것을 항소

4.  2018년 3월 7일

    -   구두 심리 (court hearing)

명백한 사실 : copyright infringement
------------------------------------

-   copyright infringement에 대해서는 이견이 없음

-   copyright holder는 infringing party의 추가적인 침해를 중지 (cease
    and desist) 시킬 수 있는 권리가 있음

논란 : 매우 광범위한 범위의 injunction
--------------------------------------

-   이 injunction은 매우 광범위한 범위를 가짐

1.  (license를 준수 하지 않는한) 피고는 모든 version의 Linux를 download,
    publising, selling, offering하는 것을 중지(cease and desist)

2.  (complete and corresponding source code를 제공하는 등의 GPL 의무를
    준수하지 않는한)

    1.  피고의 website에 있는 모든 version의 Linux에 대한 hyperlink 두는
        것을 중지(cease and desist)

    2.  피고는 사용자에게 모든 version의 Linux에 대해 download하라는
        요청을 중지(cease and desist)

# 2. The appeals case at OLG Cologne

-   피고는 고등법원 (OLG Cologne)에 지방법원에서의 광범위한 범위를 갖는
    injunction의 제거를 요청하는 항소 제기

-   구두 심리 당일, 재판관 (presiding judge)은 35분간 법원의 이해에 대한
    사전 설명 (OLG 법원이 본 case에 대해 연구한 깊이가 놀라웠음)

    1.  법원은 Linux가 1991년 Linux Torvalds에 의해 만들어지고,
        collaborative development 촉진을 위해 GPL하에 배포되었음을
        이해함

    2.  법원은 Linux kernel 전체에 co-authorship / joint authorship이
        없음을 인정함

        -   이는, program을 많은 사람들이 함께 plnanning +
            developing하는 것이 아니고,

        -   Linus Torvalds가 program을 release한 이래로, 15,000명 이상의
            개발자들이 어떠한 "grand joint plan" 없이 편집되고, 이것이
            연속적으로 반복되는 형태이기 때문.

    3.  법원은 "head of the netfilter core team" 혹은 "subsystem
        maintainer"에 이름을 올리는 것이 반드시 copyrightable work에
        contributing하는 사람인 것을 의미하지 않는다는 것을 인정

        -   수천개의 patch를 review하는 것이 이들의 copyright을 소유하는
            것이 아님

    4.  법원은 Patric McHardy's code가 포함되지 않는 수많은 Linux
        version (예: older version)이 있다는 것을 이해

-   심리 이전, 재판관은 그들의 내부적으로 고심(internal elaboration)한
    사항에 대해 요약 설명.

    1.  재판관은 피고의 주장에 merit가 있다고 믿고, 본 case에 대한
        법원의 이해에 비춰볼때 피고에게 유리한 판결을 할 것임을
        진술하며, 다음과 같은 사항을 주요 이유로 언급

    <!-- -->

    1.  Linux kernel development model은 Patrick McHardy가 Linux의
        co-author라는 주장을 support하지 않음

        -   지금까지 그는 단지 editing author이지 co-author인 것이 아님

        -   단, editing author라도 cease and desist을 요구할
            권리가 있음. 다만, 그가 authored/edited인 부분에 대해서만
            요청할 수 있지, 전체 Linux kernel에 대해 요청할 수는 없음.

    2.  원고는 그의 contribution이 정확히 무엇인지, 그리고 그것들이
        스스로 어떻게 copyrightable work을 형성하고 있는지에 대해 충분히
        보여주지 못함

    3.  원고는 netfilter/iptables 외 그가 작성한 copyrightable
        contributions이 무엇인지에 대해 입증하지 않음

        -   단지, general networking subsystem maintainer에 이름을 올린
            것만으로는 그의 copyrightable contributions이 무엇인지
            명확하지 않음

    4.  원고가 netfilter core team의 member이거나 core team의 head였다고
        하는 것으로는 여전히 co-author라는 주장을 support하지 않음

        -   netfilter는 1999년 이후 실질적으로 존재하였음. 이는
            Pactrick이 netfilter에 첫 contribution하기 3년전이고, core
            team에 join (2004년)하기 5년전임.

<!-- -->

-   전반적으로 법원도 판결이 너무 가혹 (far-fetching)하다고 생각

-   법원은 현재 적용되어 있는 preliminary procedure와는 달리 regular
    main proceeding을 갖는 것이 나을 것이라고 제안

    -   regular main proceeding에서는 전문가 증인을 요구할 수있고, 실제
        증거를 제공해야 함

-   이외 법원에서 언급된 다른 세부 사항:

    -   Patrick McHardy는  2017년 7월 26 일 피고인 측에 e-mail로 자신의
         저작물에 대한 license를 일방적으로 종료

        -   피고 (그리고 나(Welte)를 포함한 general legal opinion)에
            따르면, 이렇게 license를 일방적으로 종료하는 것은 결국
            GPL-2.0 위반임.

        -   GPL-2.0은 단지 원고의 work을 모든 third party(피고 포함)에게
            GPL-2.0으로 license해야하는 의무 하에 Linux의 modified
            version을 create / publish 할 수 있도록 허용함

        -   피고는 이렇게 license를 일방적으로 종료하는 것은 원고의
            권리를 남용하는 것으로 생각함  
            "According to the defendant (and general legal opinion,
            including my own position), this is in turn a violation of
            the GPLv2, as it only allowed plaintiff to create and
            publish modified versions of Linux under the obligation that
            he licenses his works under GPLv2 to any third party,
            including the defendant. The defendant believes this is
            abuse of his rights (German: Rechtsmissbraeuchlich)."

    -   senior kernel developer인 Greg Kroah-Hartman과 현재 netfilter
         maintainer인 Pablo Neira의 선서 진술서(sworn affidavits)가
         피고의 주장을 support하기 위해 제출됨 (내용은 비공개)

    -   피고는 Patrick McHardy가 license compliance가 아닌 금전적 이득을
         창출하는 방법으로 enforcement activity를 수행한다는 주장을
         입증함

        -   McHardy가 38건 이상의 case를 처리하였고, 이중 하나는 180만
            유로의 contractual penalty를 요구했음

        -   contractual penalty로 받은 총금액은 2백만 유로를 넘음

        -   이는 피고의 주장이며, 법원은 이에 대한 타당성을 평가하지는
            않았음

        -   하지만, 재판관은 개인적으로 알고 있는 변호사로부터 이 건에
            대해 전화를 받았으며, 다른 case에서 큰 contractual penalty가
            지급되고 있음을 들었다고 명시적으로 진술함.

    -   원고의 주장 중 하나는 그가 2017년까지
         general kernel networking maintainer에 등록되어 있는 것으로
         보임 (그의 latest patch는 2015년이고, 그것도 netfilter가
         유일함에도 불구하고)

# 3. Withdrawal by Patrick McHardy

-   법원 심리는 일시적으로 중단

    -   원고의 법적 대리인이 원고와 전화 통화할 수 있는 기회 제공

    -   preliminary injunction을 계속해서 요청할 것인지에 대해 결정

-   몇 분 후, 심리가 재개되었고, 원고는 injunction 요청을 철회함

-   결과적으로, injunction은 철회되었고, 원고는 모든 법적 비용 (법원
    수수료, 양쪽 변호사 비용)을 부담해야함

# 4. Personal Opinion

-   나는 copyright holders에 의한 license enforcement를 선호함

-   Linux kernel에 기여한 individual developer는 필요할 경우 license를
    시행할 권리가 있어야 함

    -   distributed copyright을 갖는것, 그리고 (industry friendly한)
        단지 하나의 entity만이 legal action을 취할 수 있는 상황을 피하는
        것이 중요

-   나는 "too soft" approach를 주장하는 것이 아님

    -   Linux에 대한 license violation에 대한 첫 court case로부터 15년이
        지난 지금도 여전히 문제가 존재함

    -   이는 industry가 simple problem을 해결하는데도 아직 멀었음을
        분명히 보여줌

-   반면, 이러한 활동은 항상 compliance에만 초점을 맞추어야함

    -   엄청난 contractual penalty를 모으는 것은 questionable

    -   만약, 많은 기업을 compliant하게 만들기 위한 동기로 막대한 자금을
        모으는 것이 필요하다면, 이는 공개적으로 해야하고,
        community와 협의해야함. 또한 contractual penalty는 free software
        관련 단체에 기부해야 함. 개인적인 재정적 이익이 동기가 아니라는
        것을 보여줘야함

-   Software Freedom Conservancy의 "principles of community oriented
    enforcement"나 최근의 kernel enforcement statement은 license
    violation을 어떻게 다뤄야하는지에 대해 가장 공정한 접근 방식을 제시

-   이번 결과에 행복하냐고 묻는다면, 완전히 그렇지는 않음

    -   over-reaching injunction이 제거된 것은 좋은 일임

    -   그러나, 많은 돈과 노력이 투입되었음에도 배심원단의 평결이나 법원
        판결이 없이 끝나서 아쉬움. 

    -   injunction의 범위가 크게 축소되는 법원의 판결이 나왔으면 좋았을
        것임 (예: 오직 netfilter에 대해서만 혹은 kernel의 특정
        version에서만, 혹은 특정 제품에 대해서만. hyperlink 두는 것에
        대해서는 제외 등)

    -   오늘 심리에서 나온 말들이 그냥 "증발"해버리는 것보다는, 법원의
        서면 판결로 다른 argument들도 종결이 되면 좋았을 것

# 5. Lessons learned for the developer community

-   computer programming에 detailed knowledge가 없는 법조계 사람들은
    "metadata"를 보는 경향이 있음. 이것이 그들이 이해할 수 있는
    것이기 때문.

-   누가, 어떤 title을, 언제 갖고 있는지가 중요함. 누군가가 active
    maintainer가 아니라면, list에서 그를 제외시켜야함. 

-   누군가 project의 maintainer나 developer가 더이상 아니라면, 즉시 그를
    각각의 list에서 제거해야함

-   Copyright statement가 중요. 

    -   실제로 유효한지 확인하지 않고고 copyright statement를 추가하는
        patch는 merge하지 말아야 함. 

# 6. Lessons learned for the IT industry

-   좋지 않은 동기로 GPL enforcement를 하는 사람이 있을 수 있음

-   법정에서 claim으로부터 자신을 방어하는 것은 가치가 있음. (법정
    밖에서 돈으로 합의하는 것 말고)

    -   현재의 Geniatech 사례나 2016년 Telefonica 사례에서 보듯이. 

    -   Legal system은 기회를 주면 효과가 있음

-   그럼에도 불구하고, license를 위반하고, copyright holder중 한명이
    적절하게 claim을 입증하면, 당신은 여전히 injuction을 받게 될 것임

    -   이때는 이 Patrick case처럼 되지는 않을 것임

# 7. Dear Patrick

For years, your former netfilter colleagues and friends wanted to have a
conversation with you. You have not returned our invitation so far.
Please do reach out to us. We won't bite, but we want to share our views
with you, and show you what implications your actions have not only on
Linux, but also particularly on the personal and professional lives of
the very developers that you worked hand-in-hand with for a decade. It's
your decision what you do with that information afterwards, but please
do give us a chance to talk. We would greatly appreciate if you'd take
up that invitation for such a conversation. Thanks.
