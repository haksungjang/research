# Open Source for Business

  

> 출처 : [https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645](https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645)
>
> The original work of Open Source For Business was written in English by Heather Meeker (www.heathermeeker.com).
>
> A Practical Guide to Open Source Software Licensing / Second Edition
>
> ©2015–2017 Heather Meeker. All Rights Reserved.

# Preface 
  - “killer apps” of open source : “LAMP stack”
    - Linux kernel
    - Apache web server
    - MySQL database
    - PHP scripting
 
## Background: UNIX, Linux, and Software Licensing

사실, open source licensing은 software licensing의 original model이다.

  -  proprietary licensing은  새로운것(newcomer)이다.
  -  이  두 model이  어떻게  함께  발전했는지  이해하려면 computing 역사에  대해  이해해야  한다.

## Once Upon a Time, There Was an Operating System Called UNIX

   - “open source”는 license model이면서 software development model이다. license model과 development model의 risk는  매우  다르기  때문에  이  차이는  중요하다.

  - open source의 killer app은 Linux OS이다. Linux가  개발된  이유와  방법을  배우는  것이
    -   현재 “open source”로  알려진 license model이  어떻게  개발되었고,
    -   open source model이 proprietary model과  어떻게  다른지  이해하는  가장  좋은  방법이다.

-   UNIX는 “free software” model이  등장한  이유이다.
    -  computing 초기에는 UNIX가  지배적인 operating system였다.
    -  UNIX는  AT&T Bell lab에서  개발
-   당시 AT&T는  독점  금지법의  결과로  미국  법무부의  법원  명령(consent decree)에  따라 telephone service 분야  이외의  상업  활동에  종사하는  것을  금지당하였다. 이에  따라 AT&T의  가장  뛰어나고  유능한  엔지니어들이 AT&T Bell Lab이라는  비영리  단체를  통해 computer science 개발에  참여했다.
    -   Ken Thompson과 Dennis Ritchie는 Bell Lab의  과학자였으며, computer programming을  공부한  사람은  이  이름을  알고  있다.
    -   그들은 UNIX의 creator이고, UNIX는  최초의  범용 operating system였다.
    -   UNIX를  개발하면서, C언어를  발명하였다.
    -   C는  유연하고  강력한 programming언어이고, “low-level”언어, 즉, software가 hardware와  상호작용하는  박식을 programmer에게 high level로  제어할  수  있게  한다.
    -   C는  오늘날에도  여전히 common하게  사용되고  있다.(C++, object C 등으로  확장하기도  함)

-   그러나, 법원  명령은 AT&T가 UNIX를  상업용  제품으로  사용하는  것을  금지시켰다.
    -   이에  따라 Bell Lab은 UNIX를  수정과  재배포를  헝횽하는  조항  하에 source code form으로  제공했다.
-   이후  법원  명령이  철회되었고, AT&T는 UNIX에 object code form으로만  재배포를  허용하는 licensing 조건의  제한된 license를  부여하기  시작하였다.
    -   이로  인해 UNIX와  호환되지  않는  많은 “forking” version이  만들어졌다.
    -   예를  들어, IBM의 UNIX에  맞게  작성된 program이 Sun의 UNIX에서는  실행되지  않았다.
    -   free software movement는 UNIX의 forking, 즉 proprietary licensing으로의  전환에  대한  직접적인 reaction이었다.
-   당시 “proprietary license”가  오늘날  처럼  보편적이  아니었다는  점을  이해하는  것이  중요하다.
    -   1980년대에는 software를  구매하면  어떤 computer에서도  실행할  수  있다는  사실이  생소했다.
    -   당시 software는  둘중  하나였다. 구매한 computer에  이미 load되있는  것이거나
    -   system 통합업체에서  개발한 custom software이었다.
-   그리고, 항상 source code form으로  제공되었다.
    -   왜냐하면, micro-computer (혹은 IBM PC) 이전에는 binary-only software distribution model을  지원하거나  필요로하는  표준화가  충분하지  않았다.
    -   회사들은  거의  항상  동일한 vendor로부터 hardware와 software를 bundle로  구입했다.
    -   기술  지원을  담당하는  사람들은 source code를  사용해야했으며, 기술  지원은 machine, OS, environment에만  해당되었다.
-   그렇다면, source code와 binary를  분리한  이유는  무엇이었나?
    -   당시에는  합리적이지  않았다.
    -   그러나 computing 세계는  곧  변화하였다.
    -   몇년  후, microcomputer가  표준이었고, binary software가  표준이  되었다.
