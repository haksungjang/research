# Open Source for Business

출처 : [https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645](https://www.amazon.com/Open-Source-Business-Practical-Licensing/dp/1544737645)

The original work of Open Source For Business was written in English by Heather Meeker (www.heathermeeker.com).

A Practical Guide to Open Source Software Licensing / Second Edition

©2015–2017 Heather Meeker. All Rights Reserved.

# Preface

- &quot;killer apps&quot; of open source : &quot;LAMP stack&quot;
  - Linux kernel
  - Apache web server
  - MySQL database
  - PHP scripting

## Background: UNIX, Linux, and Software Licensing

- 사실, open source licensing은software licensing의original model이다.
  - proprietary licensing은새로운것(newcomer)이다.
  - 이두model이어떻게함께발전했는지이해하려면computing 역사에대해이해해야한다.

## Once Upon a Time, There Was an Operating System Called UNIX

- &quot;open source&quot;는license model이면서software development model이다.
  - license model과development model의risk는매우다르기때문에이차이는중요하다.
- open source의killerapp은Linux OS이다.
  - Linux가개발된이유와방법을배우는것이
    - 현재&quot;open source&quot;로알려진license model이어떻게개발되었고,
    - open source model이proprietary model과어떻게다른지이해하는가장좋은방법이다.
- UNIX는&quot;free software&quot; model이등장한이유이다.
  - computing 초기에는UNIX가지배적인operating system였다.
    - AT&amp;T Bell lab에서개발
    - 당시AT&amp;T는독점금지법의결과로미국법무부의법원명령(consent decree)에따라telephone service분야이외의상업활동에종사하는것을금지당하였다.
    - 이에따라AT&amp;T의가장뛰어나고유능한엔지니어들이AT&amp;T Bell Lab이라는비영리단체를통해computer science 개발에참여했다.
- Ken Thompson과Dennis Ritchie는Bell Lab의과학자였으며, computer programming을공부한사람은이이름을알고있다.
  - 그들은UNIX의creator이고, UNIX는최초의범용operating system였다.
  - UNIX를개발하면서, C언어를발명하였다.
  - C는유연하고강력한programming언어이고, &quot;low-level&quot;언어, 즉, software가hardware와상호작용하는박식을programmer에게high level로제어할수있게한다.
  - C는오늘날에도여전히common하게사용되고있다.(C++, object C등으로확장하기도함)
- 그러나, 법원명령은AT&amp;T가UNIX를상업용제품으로사용하는것을금지시켰다.
  - 이에따라Bell Lab은UNIX를수정과재배포를헝횽하는조항하에source code form으로제공했다.
- 이후법원명령이철회되었고, AT&amp;T는 UNIX에object code form으로만재배포를허용하는licensing 조건의제한된license를부여하기시작하였다.
  - 이로인해UNIX와호환되지않는많은&quot;forking&quot; version이만들어졌다.
  - 예를들어, IBM의UNIX에맞게작성된program이Sun의UNIX에서는실행되지않았다.
- free software movement는UNIX의forking, 즉proprietary licensing으로의전환에대한직접적인reaction이었다.
- 당시&quot;proprietary license&quot;가오늘날처럼보편적이아니었다는점을이해하는것이중요하다.
  - 1980년대에는software를구매하면어떤computer에서도실행할수있다는사실이생소했다.
- 당시software는둘중하나였다.
  - 구매한computer에이미load되있는것이거나
  - system 통합업체에서개발한customsoftware이었다.
- 그리고, 항상source code form으로제공되었다.
  - 왜냐하면, micro-computer (혹은IBM PC)이전에는binary-only software distribution model을지원하거나필요로하는표준화가충분하지않았다.
- 회사들은거의항상동일한vendor로부터hardware와software를bundle로구입했다.
  - 기술지원을담당하는사람들은source code를사용해야했으며, 기술지원은machine, OS, environment에만해당되었다.
- 그렇다면, source code와binary를분리한이유는무엇이었나?
  - 당시에는합리적이지않았다.
  - 그러나computing 세계는곧변화하였다.
  - 몇년후, microcomputer가표준이었고, binary software가표준이되었다.

## Linux: The &quot;Killer App&quot;

- Open source software (특히copyleft software licensing)는Linux가아니었다면법적호기심정도로남아있었을것이다.
  - 많은system에서Linux를operating systemcore로사용하고, 그위에Android, Chrome 또는Mac과같은layer들이있다.
  - open source licensing을이해하려면Linux가왜그렇게인기있고중요한지이해해야한다.
- 1980년대후반, UNIX의인기는사라졌다.
  - 1980년대이전에는대부분의computer가정부, 교육기관, 은행및대기업과같은대형기관에서사용되었다.
  - 1세대microcomputer (Apple II, TRS-80 / 물론, DOS PC)는몇년만에모든것을바꿔버렸다.
  - 이machine들은더새롭고저렴한processor에서실행되었다.
  - UNIX는이런platform을위해쉽게적응하지못했다.
- UNIX는표준규격을갖고있었다. - UNIX platform과의호환성을정의한일련의system routine
  - 이표준은POSIX라고한다.
  - 여러사람들이POSIX와호환되지만AT&amp;T가제시한license 제한없이자유롭게사용할수있는operating system를찾기시작했다.
- 그중한명은MINIX라는학술project를작성한네덜란드의computer science 교수였다.
  - 다른한명은헬싱키의Linus Torvalds라는 10대였다.
  - Torvalds는 1991년에Linux의첫번째버전을발표하고세상을바꾸었다.
- 한편, MIT 인공지능연구소의computer 과학자인Richard Stallman은GNU project를시작했다.
  - GNU는&quot;GNU&#39;s not UNIX&quot;의재귀적약어이다.
  - GNU project는UNIX의free 대안이될operating system를만들려고했다.
- full 운영체제는많은element가필요하며, 핵심은kernel (computer실행, memory 관리, program 실행, 주변장치및기타hardware와통신)이다.
  - full operating system에는또한compiler, debugger, text editor, 관리도구및user interface와같은개발도구가필요하다.
  - Torvalds는자신의software를자유롭게사용할수있도록동의하였으며, Torvalds가작성한original version에서개선되어서채택된Linux kernel은GNU operating system의core가되었다.
  - 이operating system을이제는보통Linux라고부른다.
- Stallman은이와더불어자신이개발하려고했던새로운free operating system의사유화를막을수있는licensing paradigm을만들어갔다.
  - 그는이paradigm을 &quot;free software&quot;라고불렀고, 이는GNU General Public License (GPL)라는license를통해구체화되었다.
  - 이license는source code를비밀로유지할수없는조건으로software를재배포할수있는자유로운권리를부여했다.
  - 이는copyleft의근거였다. 저작권법을사용하여저작권이있는software저작물의공유를강제하는것이다.
- free software 정신에입각하여Linux kernel은처음개발된이래로극적으로성장, 변경및개선되었다.
  - 현재는수천명의contributor, 이를관리하는한비영리조직, 수백만명의채택자, 수십억명의사용자를보유하고있다.
  - 그리고, 여전히자유롭게변경, 재배포및개선할수있다.
  - 결과적으로, open source licensing model을업계전체를협력하게하였고, 결과적으로수백명의volunteer와함께IT분야의가장큰기업들이관리하는강력하고확장성이뛰어난system이되었다.
- 하지만, 더중요한것은Linux를사용하기위해업계는Linux의licensing 조항을사용해야했다.
  - 이에따라, Stallman이개척한copyleft paradigm은천천히견인력을얻었다.

## Part I: A Foundation

# Chapter 1 The Philosophy of Free and Open Source Software

- 대부분의사람들은Linux kernel과Apache web server와같은software를&quot;open source&quot; software라고한다.
  - 하지만, open source 운동의선구자들은open source라는용어를사용하지않으며, 그들이시작한것은&quot;free software&quot; 운동이었다.
  - 이러한용어의차이는이운동에참여한사람들의철학에서중요한차이점을나타낸다.
- free software 운동의창시자인Richard Stallman은그의철학을기술적이고경제적인freedom을장려하는것으로묘사한다.
  - 그는 &quot;software 저작권체계를감안할때, software 개발은그software의사용을통제하는owner의존재와연계가있다. 이연계가존재하는한, 우리는proprietary software를선택하거나선택하지않아야하는상황에직면하는경우가종종있다. 그러나이러한연계는내재적이거나필연적인것이아니다. 이것은특정사회적 / 법적정책결정(소유주를결정하는것)의결과이고, 이는우리가의문을제기하는것이다. &quot;라고말했다.
- Copyleft는저작권법(Stallman이도덕적으로반대하는)의힘을이용해다른사람들이저작권으로인한이익을포기하도록하는system이다.
  - free software license는저작권이있는저작물의공유및수정허락을요구하는조건으로모든사람에게광범위한저작권사용허가를부여한다.
  - 이는free software뿐만아니라permissive term하에허가된software를포함하는광범위한open source개념과는상당히다르다.
