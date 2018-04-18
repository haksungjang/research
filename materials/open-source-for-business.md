**Open Source for Business**

출처 : [https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645](https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645)

The original work of Open Source For Business was written in English by Heather Meeker (www.heathermeeker.com). 

A Practical Guide to Open Source Software Licensing / Second Edition

©2015–2017 Heather Meeker. All Rights Reserved.

**Preface**

- “killer apps” of open source : “LAMP stack”
    - Linux kernel
    - Apache web server
    - MySQL database
    - PHP scripting

Background: UNIX, Linux, and Software Licensing

- 사실, open source licensing은 software licensing의 original model이다. 
    - proprietary licensing은새로운것(newcomer)이다. 
    - 이두 model이어떻게함께발전했는지이해하려면 computing 역사에대해이해해야한다. 

Once Upon a Time, There Was an Operating System Called UNIX

- “open source”는 license model이면서 software development model이다. 
    - license model과 development model의 risk는매우다르기때문에이차이는중요하다. 

- open source의 killer app은 Linux OS이다. 
    - Linux가개발된이유와방법을배우는것이 
        - 현재 “open source”로알려진 license model이어떻게개발되었고, 
        - open source model이 proprietary model과어떻게다른지이해하는가장좋은방법이다. 

- UNIX는 “free software” model이등장한이유이다. 
    - computing 초기에는 UNIX가지배적인 operating system였다. 
        - AT&T Bell lab에서개발
        - 당시 AT&T는독점금지법의결과로미국법무부의법원명령(consent decree)에따라 telephone service 분야이외의상업활동에종사하는것을금지당하였다. 
        - 이에따라 AT&T의가장뛰어나고유능한엔지니어들이 AT&T Bell Lab이라는비영리단체를통해 computer science 개발에참여했다.

- Ken Thompson과 Dennis Ritchie는 Bell Lab의과학자였으며, computer programming을공부한사람은이이름을알고있다. 
    - 그들은 UNIX의 creator이고, UNIX는최초의범용 operating system였다. 
    - UNIX를개발하면서, C언어를발명하였다. 
    - C는유연하고강력한 programming언어이고, “low-level”언어, 즉, software가 hardware와상호작용하는박식을 programmer에게 high level로제어할수있게한다. 
    - C는오늘날에도여전히 common하게사용되고있다.(C++, object C 등으로확장하기도함)

- 그러나, 법원명령은 AT&T가 UNIX를상업용제품으로사용하는것을금지시켰다. 
    - 이에따라 Bell Lab은 UNIX를수정과재배포를헝횽하는조항하에 source code form으로제공했다. 

- 이후법원명령이철회되었고, AT&T는 UNIX에 object code form으로만재배포를허용하는 licensing 조건의제한된 license를부여하기시작하였다. 
    - 이로인해 UNIX와호환되지않는많은 “forking” version이만들어졌다. 
    - 예를들어, IBM의 UNIX에맞게작성된 program이 Sun의 UNIX에서는실행되지않았다. 

- free software movement는 UNIX의 forking, 즉 proprietary licensing으로의전환에대한직접적인 reaction이었다. 
- 당시 “proprietary license”가오늘날처럼보편적이아니었다는점을이해하는것이중요하다. 
    - 1980년대에는 software를구매하면어떤 computer에서도실행할수있다는사실이생소했다. 

- 당시 software는둘중하나였다. 
    - 구매한 computer에이미 load되있는것이거나
    - system 통합업체에서개발한 custom software이었다.

- 그리고, 항상 source code form으로제공되었다. 
    - 왜냐하면, micro-computer (혹은 IBM PC) 이전에는 binary-only software distribution model을지원하거나필요로하는표준화가충분하지않았다. 

- 회사들은거의항상동일한 vendor로부터 hardware와 software를 bundle로구입했다.
    - 기술지원을담당하는사람들은 source code를사용해야했으며, 기술지원은 machine, OS, environment에만해당되었다. 

- 그렇다면, source code와 binary를분리한이유는무엇이었나? 
    - 당시에는합리적이지않았다. 
    - 그러나 computing 세계는곧변화하였다. 
    - 몇년후, microcomputer가표준이었고, binary software가표준이되었다. 

Linux: The “Killer App”

- Open source software (특히 copyleft software licensing)는 Linux가아니었다면법적호기심정도로남아있었을것이다. 
    - 많은 system에서 Linux를 operating system core로사용하고, 그위에 Android, Chrome 또는 Mac과같은 layer들이있다. 
    - open source licensing을이해하려면 Linux가왜그렇게인기있고중요한지이해해야한다. 

- 1980년대후반, UNIX의인기는사라졌다.
    - 1980년대이전에는대부분의 computer가정부, 교육기관, 은행및대기업과같은대형기관에서사용되었다.
    - 1세대 microcomputer (Apple II, TRS-80 / 물론, DOS PC)는몇년만에모든것을바꿔버렸다.
    - 이 machine들은더새롭고저렴한 processor에서실행되었다. 
    - UNIX는이런 platform을위해쉽게적응하지못했다.

- UNIX는표준규격을갖고있었다. - UNIX platform과의호환성을정의한일련의 system routine
    - 이표준은 POSIX라고한다. 
    - 여러사람들이 POSIX와호환되지만 AT&T가제시한 license 제한없이자유롭게사용할수있는 operating system를찾기시작했다. 

- 그중한명은 MINIX라는학술 project를작성한네덜란드의 computer science 교수였다.
    - 다른한명은헬싱키의 Linus Torvalds라는 10대였다.
    - Torvalds는 1991년에 Linux의첫번째버전을발표하고세상을바꾸었다. 

- 한편, MIT 인공지능연구소의 computer 과학자인 Richard Stallman은 GNU project를시작했다.
    - GNU는 “GNU’s not UNIX”의재귀적약어이다. 
    - GNU project는 UNIX의 free 대안이될 operating system를만들려고했다. 

- full 운영체제는많은 element가필요하며, 핵심은 kernel (computer 실행, memory 관리, program 실행, 주변장치및기타 hardware와통신)이다. 
    - full operating system에는또한 compiler, debugger, text editor, 관리도구및 user interface와같은개발도구가필요하다. 
    - Torvalds는자신의 software를자유롭게사용할수있도록동의하였으며, Torvalds가작성한 original version에서개선되어서채택된 Linux kernel은 GNU operating system의 core가되었다. 
    - 이 operating system을이제는보통 Linux라고부른다. 

- Stallman은이와더불어자신이개발하려고했던새로운 free operating system의사유화를막을수있는 licensing paradigm을만들어갔다. 
    - 그는이 paradigm을 “free software”라고불렀고, 이는 GNU General Public License (GPL)라는 license를통해구체화되었다. 
    - 이 license는 source code를비밀로유지할수없는조건으로 software를재배포할수있는자유로운권리를부여했다. 
    - 이는 copyleft의근거였다. 저작권법을사용하여저작권이있는 software 저작물의공유를강제하는것이다. 

- free software 정신에입각하여 Linux kernel은처음개발된이래로극적으로성장, 변경및개선되었다. 
    - 현재는수천명의 contributor, 이를관리하는한비영리조직, 수백만명의채택자, 수십억명의사용자를보유하고있다. 
    - 그리고, 여전히자유롭게변경, 재배포및개선할수있다. 
    - 결과적으로, open source licensing model을업계전체를협력하게하였고, 결과적으로수백명의 volunteer와함께 IT분야의가장큰기업들이관리하는강력하고확장성이뛰어난 system이되었다. 

- 하지만, 더중요한것은 Linux를사용하기위해업계는 Linux의 licensing 조항을사용해야했다.
    - 이에따라, Stallman이개척한 copyleft paradigm은천천히견인력을얻었다. 

**Part I: A Foundation**

**Chapter 1 The Philosophy of Free and Open Source Software**

- 대부분의사람들은 Linux kernel과 Apache web server와같은 software를 “open source” software라고한다. 
    - 하지만, open source 운동의선구자들은 open source라는용어를사용하지않으며, 그들이시작한것은 “free software” 운동이었다. 
    - 이러한용어의차이는이운동에참여한사람들의철학에서중요한차이점을나타낸다. 

- free software 운동의창시자인 Richard Stallman은그의철학을기술적이고경제적인 freedom을장려하는것으로묘사한다. 
    - 그는 “software 저작권체계를감안할때, software 개발은그 software의사용을통제하는 owner의존재와연계가있다. 이연계가존재하는한, 우리는 proprietary software를선택하거나선택하지않아야하는상황에직면하는경우가종종있다. 그러나이러한연계는내재적이거나필연적인것이아니다. 이것은특정사회적 / 법적정책결정(소유주를결정하는것)의결과이고, 이는우리가의문을제기하는것이다. “라고말했다. 

- Copyleft는저작권법(Stallman이도덕적으로반대하는)의힘을이용해다른사람들이저작권으로인한이익을포기하도록하는 system이다. 
    - free software license는저작권이있는저작물의공유및수정허락을요구하는조건으로모든사람에게광범위한저작권사용허가를부여한다. 
    - 이는 free software뿐만아니라 permissive term하에허가된 software를포함하는광범위한 open source 개념과는상당히다르다. 
