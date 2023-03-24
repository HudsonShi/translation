
**Part I**

**第一部分**

**Detailed Analysis of the GNU GPL and Related Licenses**

**GNU GPL 及相关许可证的详细分析**

This part of the tutorial gives a comprehensive explanation of the most popular Free Software copyright license, the GNU General Public License ("GNU GPL", or sometimes just "GPL") -- both version 2 ("GPLv2") and version 3 ("GPLv3") -- and teaches lawyers, software developers, managers and business people how to use the GPL (and GPL'd software) successfully both as a community-building "Constitution" for a software project, and to incorporate copylefted software into a new Free Software business and in existing, successful enterprises.

本教程的这一部分对最流行的自由软件版权许可证，即GNU通用公共许可证（“GNU GPL”，有时简称为“GPL”）——版本 2（“GPLv2”）和版本 GPLv3（“GPLv3”）——进行了全面的解释，引导律师、软件开发人员、管理人员和业务人员如何成功地使用GPL（以及GPL的软件），将其作为软件项目的社区建设“章程”，并将版权不标准(copylefted)的软件合并到新的自由软件业务和现有的成功企业中。

To benefit from this part of the tutorial, readers should have a general familiarity with software development processes. A basic understanding of how copyright law applies to software is also helpful. The tutorial is of most interest to lawyers, software developers and managers who run or advise software businesses that modify and/or redistribute software under the terms of the GNU GPL (or who wish to do so in the future), and those who wish to make use of existing GPL'd software in their enterprise.

为了从教程的这一部分中受益，读者应该对软件开发过程有一个大致的了解。对版权法如何适用于软件的基本理解也很有帮助。本教程最感兴趣的是律师、软件开发人员和管理人员，他们经营软件业务，建议根据GNU GPL条款修改和/或重新分发软件（或希望在将来这样做），还有那些希望在他们的企业中使用已有的GPL软件的人。

Upon completion of this part of the tutorial, readers can expect to have learned the following:

看完本教程的这一部分后，读者可以期望学到以下内容：

- The freedom-defending purpose of various terms in the GNU GPLv2 and GPLv3.
- GNU GPLv2和GPLv3中各种术语，目的是捍卫自由；

- The differences between GPLv2 and GPLv3.
- GPLv2和GPLv3的区别；

- The redistribution options under the GPLv2 and GPLv3.
- 基于GPLv2和GPLv3的再分发选项；

- The obligations when modifying GPLv2'd or GPLv3'd software.
- 修改GPLv2或GPLv3软件时应遵循的义务；

- How to build a plan for proper and successful compliance with the GPL.
- 如何制定计划以正确且成功地遵守GPL协议；

- The business advantages that the GPL provides.
- GPL提供的业务优势；

- The most common business models used in conjunction with the GPL.
- 与GPL结合使用的最常见的商业模式；

- How existing GPL'd software can be used in existing enterprises.
- 企业如何使用已有的GPL软件；

- The basics of LGPLv2.1 and LGPLv3, and how they differ from the GPLv2 and GPLv3, respectively.
- LGPLv2.1和LGPLv3的基础知识，以及它们分别与GPLv2和GPLv3的区别；

- The basics to begin understanding the complexities regarding derivative and combined works of software.
- 开始了解有关软件的衍生和组合作品的复杂性的基础知识。

## CHAPTER 1 WHAT IS SOFTWARE FREEDOM?

## 第一章 什么是软件自由？

Study of the GNU General Public License (herein, abbreviated as *GNU GPL* or just *GPL*) must begin by first considering the broader world of software freedom. The GPL was not created in a vacuum. Rather, it was created to embody and defend a set of principles that were set forth at the founding of the GNU Project and the Free Software Foundation (FSF) -- the preeminent organization that upholds, defends and promotes the philosophy of software freedom. A prerequisite for understanding both of the popular versions of the GPL (GPLv2 and GPLv3) and their terms and conditions is a basic understanding of the principles behind them. The GPL family of licenses are unlike nearly all other software licenses in that they are designed to defend and uphold these principles.

研究GNU通用公共许可证（此处缩写为*GNU GPL*或简称*GPL*）必须首先考虑更广泛的软件自由世界。 GPL不是凭空产生的，它是为了体现和捍卫在GNU项目和自由软件基金会 (FSF) 成立时提出的一系列原则而创建的，FSF是一个维护、捍卫和促进软件自由哲学的卓越组织。 理解GPL的两个流行版本（GPLv2 和 GPLv3）及其条款和条件的先决条件是对它们背后的原则有基本的理解。GPL系列许可证与几乎所有其他的软件许可证不同，因为它们旨在捍卫和维护这些原则。

### The Free Software Definition

### 自由软件的定义

The Free Software Definition is set forth in full on FSF's website at <http://fsf.org/philosophy/free-sw.html>. This section presents an abbreviated version that will focus on the parts that are most pertinent to the GPL.

自由软件定义在FSF的网站 <http://fsf.org/philosophy/free-sw.html> 上有完整的阐述。 本节提供一个缩略版，将重点放在与GPL最相关的部分。

A particular user has software freedom with respect to a particular program if that user has the following freedoms:

如果某个特定用户具有以下自由，则这个用户就具有与特定程序相关的软件自由：

- The freedom to run the program, for any purpose.
- 出于任何目的执行程序的自由；

- The freedom to study how the program works, and modify it
- 了解程序的运行机制，可以随意修改的自由；

- The freedom to redistribute copies.
- 随意分发软件副本的自由；

- The freedom to distribute copies of modified versions to others.
- 将修改后的软件副本分发给他人的自由。

The focus on "a particular user" is particularly pertinent here. It is not uncommon for a subset of a specific program's user base to have these freedoms, while other users of the same version the program have none or only some of these freedoms. Section [12.2](#business-models) talks in detail about how this can unfortunately happen even if a program is released under the GPL.

对“特定用户”的关注在这里尤为重要。某个特定程序的用户群的一部分人拥有这些自由的情况并不少见，而同一版本程序的其他用户则没有或只有其中的一部分自由。第 [12.2](#商业模式) 章节详细讨论了这种情况，即使程序是基于GPL发布的。

Many people refer to software with these freedoms as "Open Source." Besides having a different political focus from those who call such software by the name "Free Software",[^1^](#_bookmark4), those who call the software "Open Source" are often focused on a side issue. Specifically, user access to the source code of a program is a prerequisite to make use of the freedom to modify. However, the important issue is what freedoms are granted in the license that applies to that source code.

许多人将具有这些自由的软件称为“开源”。除了与那些将此类软件称为“自由软件” <sup>1</sup> 的人有着不同的政治关注点之外，将软件称为“开源”的人通常关注的是一个次要问题。具体来说，用户访问程序的源代码是实现修改自由的先决条件。然而，重要的问题是在适用于该源代码的许可证中授予了哪些自由。

<sup>1</sup>The political differences between the Free Software Movement and the Open Source Movement are documented on FSF's Web site at
<http://www.fsf.org/licensing/essays/free-software-for-freedom.html>.

<sup>1</sup>自由软件运动和开源运动之间的政治分歧记录在FSF的网站上，网址为 <http://www.fsf.org/licensing/essays/free-software-for-freedom.html>.

Software freedom is only complete when no restrictions are imposed on how these freedoms are exercised. Specifically, users and programmers can exercise these freedoms noncommercially or commercially. Licenses that grant these freedoms for noncommercial activities but prohibit them for commercial activities are considered non-free. The Open Source Initiative (*OSI* ) (the arbiter of what is considered "Open Source") also regards such licenses as inconsistent with its "Open Source Definition".

只有当如何行驶这些自由没有任何限制时，软件自由才是完整的。具体而言，用户和程序员可以非商业或商业的方式行使这些自由。那些仅限于非商业活动的一些自由，但禁止商业活动自由的许可，被认为是非自由的。开源促进会(*OSI*)（被认为是“开源”的仲裁者）也认为此类许可证与其“开源定义”不一致。

In general, software for which any of these freedoms are restricted in any way is called "nonfree" software. Some use the term "proprietary software" more or less interchangeably with "nonfree software". The FSF published a useful [explanation of various types of software and how they relate to one another.](http://www.gnu.org/philosophy/categories.html)

一般来说，以任何方式限制自由的软件被称为“非自由”软件。有些人或多或少地将“专有软件”一词与“非自由软件”互换使用。 FSF发布了一份有用的[对各种类型的软件以及它们之间的相互关系的解释](http://www.gnu.org/philosophy/categories.html)

Keep in mind that none of the terms "software freedom", "open source" and "free software" are known to be trademarked or otherwise legally restricted by any organization in any jurisdiction. As such, it's quite common that these terms are abused and misused by parties who wish to bank on the popularity of software freedom. When one considers using, modifying or redistributing a software package that purports to be Open Source or Free Software, one **must** verify that the license grants software freedom.

请记住，“软件自由”、“开源”和“免费软件”等术语均未被任何司法管辖区的任何组织注册商标，或以其他方式限制使用。这些术语被某些机构滥用和误用是很常见的现象，因为他们希望扩大软件自由的普及度。当考虑使用、修改或重新分发声称是开源或自由软件的软件包时，**必须**验证许可证是否授予软件自由。

Furthermore, throughout this text, we generally prefer the term "software freedom", as this is the least ambiguous term available to describe software that meets the Free Software Definition. For example, it is well known and often discussed that the adjective "free" has two unrelated meanings in English: "free as in freedom" and
"free as in price". Meanwhile, the term "open source" is even more confusing, because it appears to refer only to the "freedom to study", which is merely a subset of one of the four freedoms.

此外，在本文中，我们通常更喜欢“软件自由”一词，因为在那些描述符合自由软件定义的软件的一堆术语中，它的歧义最小。例如，大家经常讨论的英文中的形容词“自由”，它有两个不相关的含义：“使用的自由”和“价格的自由(免费)”。同时，“开源”一词更令人困惑，因为它似乎仅指“学习的自由”，这仅仅是四个自由中的一个。

The remainder of this section considers each of each component of software freedom in detail.

本节的其余部分将详细考虑软件自由的每个组成部分。

#### The Freedom to Run

#### 执行程序的自由

The first tenet of software freedom is the user's fully unfettered right to run the program. The software's license must permit any conceivable use of the software. Perhaps, for example, the user has discovered an innovative use for a particular program, one that the programmer never could have predicted. Such a use must not be
restricted.

软件自由的首要原则是用户拥有完全不受限制地执行该程序的权利。该软件的许可证必须允许用户以任意方式使用软件。例如，也许用户发现了针对一个特定场景的创新用途，这个场景可能是程序员从未预料到的。不得限制此类用途。

It was once rare that this freedom was restricted by even proprietary software; but such is quite common today. Most End User License Agreements (EULAs) that cover most proprietary software typically restrict some types of uses. Such restrictions of any kind are an unacceptable restriction on software freedom.

曾经很少有使用软件的自由受到限制的情况，在专有软件中也很少见；但现在却很普遍。大多数基于最终用户许可协议（EULAs）的专有软件，通常限制某些类型的用途。任何这些形式的限制对软件自由来说，都是不可接受的。

#### The Freedom to Change and Modify

#### 更改和修改程序的自由

Perhaps the most useful right of software freedom is the users' right to change, modify and adapt the software to suit their needs. Access to the source code and related build and installation scripts are an essential part of this freedom. Without the source code, and the ability to build and install the binary applications from that source, users cannot effectively exercise this freedom.

软件自由的最有用的权利也许是用户拥有根据自己的需求更改、修改和调整软件的权利。对源代码以及相关的构建和安装脚本的访问权限，是该自由的重要组成部分。如果没有源代码，以及基于该源码构建和安装二进制应用程序的脚本，用户就无法有效地行使这种自由。

Programmers directly benefit from this freedom. However, this freedom remains important to users who are not programmers. While it may seem counterintuitive at first, non-programmer users often exercise this freedom indirectly in both commercial and noncommercial settings. For example, users often seek noncommercial help with the software on email lists and in user groups. To make use of such help they must either have the freedom to recruit programmers who might altruistically assist them to modify their software, or to at least follow rote instructions to make basic modifications themselves.

程序员是这种自由的直接受益者。但是，这种自由对于非程序员的用户来说也很重要。虽然看起来似乎有点违反直觉，但非程序员用户通常在商业和非商业环境中，间接行使这种自由。例如，用户经常在电子邮件列表和用户群组中需求软件上的非商业性帮助。为了能够使用这种便利，必须允许他们自由地招募可能会免费帮助他们修改软件的程序员，或者允许他们按照使用说明可以自己进行基本的修改。

More commonly, users also exercise this freedom commercially. Each user, or group of users, may hire anyone they wish in a competitive free market to modify and change the software. This means that companies have a right to hire anyone they wish to modify their Free Software. Additionally, such companies may contract with other
companies to commission software modifications.

更常见的是，用户还可以在商业上行使这种自由。每个用户或一组用户都可以在竞争激烈的自由市场中，雇用他们希望的任何人来修改和更改软件。这意味着公司有权雇用任何愿意修改其免费软件的人。此外，公司可以与其他公司签订合同，委托进行软件修改。

#### The Freedom to Copy and Share

#### 复制和分享软件的自由

Users share Free Software in a variety of ways. Software freedom advocates work to eliminate a fundamental ethical dilemma of the software age: choosing between obeying a software license and friendship (by giving away a copy of a program to your friend who likes the software you are using). Licenses that respect software
freedom, therefore, permit altruistic sharing of software among friends.

用户以多种方式分享自由软件。软件自由倡导者致力于消除软件时代的一个基本道德困境：在遵守软件许可和友谊之间做出选择（当你的朋友喜欢你正在使用的软件时，赠送一份程序副本给他）。 因此，尊重软件自由的许可证允许在朋友之间无私地分享软件。

The commercial environment also benefits from this freedom. Commercial sharing includes selling copies of Free Software: that is, Free Software can be distributed for any monetary price to anyone. Those who redistribute Free Software commercially also have the freedom to selectively distribute (i.e., you can pick your customers) and to set prices at any level that redistributor sees fit.

商业环境也得益于这种自由。商业共享包括出售自由软件的副本：也就是说，可以用任何货币价格将自由软件分发给其他人。那些以商业方式重新分发自由软件的人，也可以有选择地自由分发（如可以选择你自己的客户），并可以自行设置合适的价格水平。

Of course, most people get copies of Free Software very cheaply (and sometimes without charge). The competitive free market of Free Software tends to keep prices low and reasonable. However, if someone is willing to pay billions of dollars for one copy of the GNU Compiler Collection, such a sale is completely permitted.

当然，大多数人都可以非常便宜地获得自由软件的副本（有时甚至是免费的）。竞争激烈的自由软件市场倾向于保持低价和合理的价格。但是如果真有人愿意花费数十亿美元购买一份GNU编译集，这也是完全允许的。

Another common instance of commercial sharing is service-oriented distribution. For example, some distribution vendors provide immediate security and upgrade distribution via a special network service. Such distribution is not necessarily contradictory with software freedom.

商业共享的另一个常见方式是面向服务的分发。例如，一些分发供应商通过特殊的网络服务提供即时安全和升级服务。这种分发方式不一定与软件自由相矛盾。

(Section [12.2](#business-models) of this tutorial talks in detail about some common Free Software business models that take advantage of the freedom to share commercially.)

（本教程的[第12.2章](#商业模式)部分详细讨论了一些常见的利用商业实现自由软件的自由共享的业务模式。）

#### The Freedom to Share Improvements

#### 分享改进的自由

The freedom to modify and improve is somewhat empty without the freedom to share those improvements. The software freedom community is built on the pillar of altruistic sharing of improved Free Software. Historically it was typical for a Free Software project to sprout a mailing list where improvements would be shared freely among members of the development community.<sup>2</sup> Such noncommercial sharing is the primary reason that Free Software thrives.

如果没有分享改进的自由，修改和改进的自由多少有点空洞。软件自由社区建立在无私共享改进的自由软件的基础上。从历史上看，自由软件项目的典型做法是建立一个邮件列表，开发社区的成员可以在其中免费分享改进的内容。<sup>2</sup> 这种非商业性质的共享方式是自由软件蓬勃发展的主要原因。

<sup>2</sup> This is still commonly the case, though today there are additional ways of sharing Free Software.

<sup>2</sup> 现在这仍然是常见的情况，尽管现在已经有其他共享自由软件的方法。

Commercial sharing of modified Free Software is equally important. For commercial support to exist in a competitive free market, all developers -- from single-person contractors to large software companies -- must have the freedom to market their services as augmenters of Free Software. All forms of such service marketing must
be equally available to all.

修改后的自由软件的商业共享同样重要。为了在竞争激烈的自由市场中提供商业支持，所有的开发人员——从个人承包商到大型软件公司——都应该可以自由地将他们的服务作为自由软件的补充进行销售。这种形式的服务营销必须对所有人一视同仁。

For example, selling support services for Free Software is fully permitted. Companies and individuals can offer themselves as "the place to call" when software fails or does not function properly. For such a service to be meaningful, the entity offering that service needs the right to modify and improve the software for the customer to correct any problems that are beyond mere user error.

例如，销售免费软件的支持服务是完全允许的。当软件出现故障或无法正常运行时，公司和个人可以将自己作为“呼叫客服”。为了使此类服务有意义，提供该服务的实体需要有权为客户修改和改进软件，以纠正任何超出用户错误的问题。

Software freedom licenses also permit any entity to distribute modified versions of Free Software. Most Free Software programs have a "standard version" that is made available from the primary developers of the software. However, all who have the software have the "freedom to fork" -- that is, make available nontrivial modified versions of the software on a permanent or semi-permanent basis. Such freedom is central to vibrant developer and user interaction.

软件自由许可证还允许任何实体分发自由软件的修改版本。大多数自由软件程序都有一个“标准版本”，可以从软件的主要开发人员那里获得。然而，所有拥有该软件的人都有“分叉自由”——也就是说，可以永久或半永久地提供软件的重要修订版本。这种自由是充满活力的开发人员和用户交互的核心。

Companies and individuals have the right to make true value-added versions of Free Software. They may use freedom to share improvements to distribute distinct versions of Free Software with different functionality and features. Furthermore, this freedom can be exercised to serve a disenfranchised subset of the user community. If the
developers of the standard version refuse to serve the needs of some of the software's users, other entities have the right to create a long- or short-lived fork to serve that sub-community.

公司和个人有权制作的自由软件的增值版本。他们可以自由地改进，并分享具有不同功能和特性的自由软件版本。此外，这种自由可以用来服务于被剥夺权力的用户群体。如果标准版本的开发人员拒绝满足某些软件用户的需求，则其他实体有权创建一个长期或短期的分支，提供服务满足于这些软件用户。

### How Does Software Become Free?

### 软件是如何变得自由的？

The previous section set forth key freedoms and rights that are referred to as "software freedom". This section discusses the licensing mechanisms used to enable software freedom. These licensing mechanisms were ultimately created as a community-oriented "answer" to the existing proprietary software licensing mechanisms. Thus, first, consider carefully why proprietary software exists in the first place.

上一节阐述了被称为“软件自由”的一些关键自由和权利。本节讨论用于实现软件自由的许可机制。这些许可机制被看作是将现有专有软件许可机制转变为面向社区机制的“答案”所在。 因此，首先要仔细考虑为什么会有专有软件存在。

The primary legal regime that applies to software is copyright law. Proprietary software exists at all only because copyright law governs software.<sup>3</sup> Copyright law, with respect to software, typically governs copying, modifying, and redistributing that software (For details of this in the USA, see [§106](http://www.copyright.gov/title17/92chap1.html#106) and [§117](http://www.copyright.gov/title17/92chap1.html#117) of [Title17](http://www.law.cornell.edu/uscode/text/17) of the *United States Code*).<sup>4</sup> By law (in the USA and in most other jurisdictions), the copyright holder (most typically,the author) of the work controls how others may copy, modify and/or distribute the work. For proprietary software, these controls are used
to prohibit these activities. In addition, proprietary software distributors further impede modification in a practical sense by distributing only binary code and keeping the source code of the software secret.

适用于软件的主要法律制度是版权法。专有软件的存在完全是因为版权法对软件的管理规定。<sup>3</sup> 关于软件的版权法，主要是对软件的复制、修改和再发行的管理规定（有关美国的详细信息，请参阅《美国法典》[第17篇](http://www.law.cornell.edu/uscode/text/17)的[§106](http://www.copyright.gov/title17/92chap1.html#106)和[§117](http://www.copyright.gov/title17/92chap1.html#117)）。<sup>4</sup> 根据法律（在美国和大多数其他司法管辖区），作品的版权持有者（通常是作者本人） 可以控制其他人如何复制、修改和/或分发作品。专有软件的这些控制行为禁止了软件的相关操作。此外，专有软件分销商只发行二进制可执行代码，严格保密源代码，这也进一步阻碍了实际意义上的代码修改。

<sup>3</sup> This statement is admittedly an oversimplification. Patents and trade secrets can cover software and make it effectively non-Free, and one can contract away their rights and freedoms regarding software, or source code can be practically obscured in binary-only distribution without reliance on any legal system. However, the primary control mechanism for software is copyright, and therefore this section focuses on how copyright restrictions make software proprietary.

<sup>3</sup> 诚然，这种说法过于简单化了。专利和商业秘密可以要求软件保密，使其成为非自由软件，并且可以通过合同剥夺他们在软件方面的权利和自由，或者源代码实际上可以在不依赖于任何法律制度的情况下，以二进制形式分发。但是，软件的主要控制机制是版权，因此本节重点讨论版权限制如何使软件成为专有软件。

<sup>4</sup> Copyright law in general also governs "public performance" of copyrighted works. There is no generally agreed definition for public performance of software and both GPLv2 and GPLv3 do not restrict public performance.

<sup>4</sup> 版权法一般也适用于版权作品的“公开性能”。对于软件的公开性能没有普遍认可的定义，GPLv2和GPLv3都不限制公开性能。

Copyright is not a natural state, it is a legal construction. In the USA, the Constitution permits, but does not require, the creation of copyright law as federal legislation. Software, since it is an "original work of authorship fixed in any tangible medium of expression ... from which they can be perceived, reproduced, or
otherwise communicated, either directly or with the aid of a machine or device" (as stated in [17 USC](http://www.law.cornell.edu/uscode/text/17/102) [§ 102)](http://www.law.cornell.edu/uscode/text/17/102), is thus covered by the statute, and is copyrighted by default.

版权不是一种自然状态，它是一种法律结构。在美国，宪法允许但不要求将版权法作为联邦立法。软件，因为它是“固定在任何有形表达媒介中的原创作品……可以直接或借助机器/设备从中感知、复制或以其他方式传播”（如 [《美国法典》第17篇](http://www.law.cornell.edu/uscode/text/17/102) [第§102章节](http://www.law.cornell.edu/uscode/text/17/102)所述)，因此受法规保护，默认情况下受版权保护。

However, software, in its natural state without copyright, is Free Software. In an imaginary world with no copyright, the rules would be different. In this world, when you received a copy of a program's source code, there would be no default legal system to restrict you from sharing it with others, making modifications, or redistributing those modified versions.<sup>5</sup>

但是，在没有版权的自然状态下，软件是自由软件。在没有版权的虚拟世界中，规则会有所不同。在虚拟世界上，当你收到一个程序的源代码副本时，不会有默认的法律制度来限制你与他人共享、进行修改或重新分发这些修改后的版本。<sup>5</sup>

<sup>5</sup> Note that this is again an oversimplification; the complexities with this argument are discussed in Section [1.2.3.](#software-and-non-copyright-legal-regimes)

<sup>5</sup> 注意，这里又将情况给简化处理了；关于这一争论的复杂情况的讨论详见[1.2.3 章节](#software-and-non-copyright-legal-regimes)

Software in the real world is copyrighted by default and is automatically covered by that legal system. However, it is possible to move software out of the domain of the copyright system. A copyright holder can often *disclaim* their copyright. (For example, under USA copyright law it is possible for a copyright holder to engage in
conduct resulting in abandonment of copyright.) If copyright is disclaimed, the software is effectively no longer restricted by copyright law. Software not restricted by copyright is in the "public domain."

现实世界中的软件默认受版权保护，并自动受该法律体系保护。但是，可以将软件移出版权系统的范围。版权所有者通常可以*放弃*他们的版权。（例如，根据美国版权法，版权所有者可以实施某些操作，放弃版权。）如果放弃版权，则该软件实际上不再受版权法的限制。不受版权限制的软件属于“公共领域软件”。

#### Public Domain Software

#### 公共领域软件

In the USA and other countries that are parties to the Berne Convention on Copyright, software is copyrighted automatically by the author when she fixes the software in a tangible medium. In the software world, this usually means typing the source code of the software into a file.

在美国和其他加入《伯尔尼版权公约》的国家，当作者将软件固定在有形介质中时，软件自动受到版权保护。在软件世界中，这通常意味着将软件的源代码输入到文件中。

Imagine if authors could truly disclaim those default controls of copyright law. If so, the software is in the public domain --- no longer covered by copyright. Since copyright law is the construction allowing for most restrictions on software (i.e., prohibition of copying, modification, and redistribution), removing the software from the copyright system usually yields software freedom for its users.

想象一下，如果作者真的放弃了版权法的默认控制。如果是这样，该软件就属于公共领域 --- 不再受版权保护。由于版权法是允许对软件进行操作限制（如禁止复制、修改和重新分发）的结构定义，因此从版权系统中删除软件通常会为其用户带来软件自由。

Carefully note that software truly in the public domain is *not* licensed in any way. It is confusing to say software is "licensed for the public domain," or any phrase that implies the copyright holder gave express permission to take actions governed by copyright law.

请注意，真正属于公共领域的软件*未*以任何方式获得许可。关于软件“已获得公共领域许可”，或任何关于版权所有者明确允许采取受版权法管辖的行为的暗示说法，都是令人困惑的。

Copyright holders who state that they are releasing their code into the public domain are effectively renouncing copyright controls on the work. The law gave the copyright holders exclusive controls over the work, and they chose to waive those controls. Software that is, in this sense, in the public domain is conceptualized by the developer as having no copyright and thus no license. The software freedoms discussed in Section [1.1](#the-free-software-definition) are all
granted because there is no legal system in play to take them away.

如果版权所有者声明将其代码发布到公共领域，实际上他就放弃了对作品的版权控制。法律赋予版权所有者对作品的独占控制权，他们可以选择放弃这些控制权。从这个意义上说，处于公共领域的软件被开发人员认定为没有版权，因此也就没有许可证。第[1.1] 节（#the-free-software-definition）中讨论的软件自由都是被授予的，因为没有法律制度可以剥夺这些自由。

Admittedly, a discussion of public domain software is an oversimplified example. Because copyright controls are usually automatically granted and because, in some jurisdictions, some copyright controls cannot be waived (see Section [1.2.4](#non-usa-copyright-regimes) for further discussion), many copyright holders sometimes incorrectly believe a work has been placed in the public domain. Second, due to aggressive lobbying by the entertainment industry, the "exclusive Right" of copyright, that was supposed to only exist for "Limited Times" according to the USA Constitution, appears to be infinite: simply purchased on the installment plan rather than in whole. Thus, we must assume no works of software will fall into the public domain merely due to the passage of time.

诚然，对公共领域软件的讨论是一个过于简单化的例子。因为版权控制通常是自动授予的，并且在某些司法管辖区，某些版权控制不能被放弃（请参考第 [1.2.4] 节（#non-usa-copyright-regimes）以了解进一步的讨论），许多版权所有者有时会错误地认为作品已经发布到了公共领域。其次，由于娱乐业的积极游说，根据美国宪法规定，版权的“专有权”本应仅存在于“有限时间”，但看起来似乎是无限的：只是分期付款购买，而不是全部购买。因此，我们必须假设没有任何软件作品会因为时间的流逝而落入公共领域。

Nevertheless, under USA law it is likely that the typical disclaimers of copyright or public domain dedications we see in the Free Software world would be interpreted by courts as copyright abandonment, leading to a situation in which the user effectively receives a maximum grant of copyright freedoms, similar to a maximally-permissive Free Software license.

然而，根据美国法律，我们在自由软件世界中看到的典型的版权免责声明，或公共领域专有申明，可能会被法院解释为放弃版权，从而授予了用户实际上最大程度的版权自由，类似于最大程度的自由软件许可证。

The best example of software known to truly be in the public domain is software that is published by the USA government. Under [17 USC 101 105,](http://www.law.cornell.edu/uscode/text/17/105) all works published by the USA Government are not copyrightable in the USA.

目前所知的真正属于公共领域的软件最好的例子，是由美国政府发布的软件。根据《美国法典》[第17章101-105](http://www.law.cornell.edu/uscode/text/17/105)，在美国，美国政府出版的所有作品均不受版权保护。

#### Why Copyright Free Software?

#### 为什么需要版权自由的软件？

If simply disclaiming copyright on software yields Free Software, then it stands to reason that putting software into the public domain is the easiest and most straightforward way to produce Free Software. Indeed, some major Free Software projects have chosen this method for making their software Free. However, most of the Free Software in existence *is* copyrighted. In most cases (particularly in those of FSF and the GNU Project), this was done due to very careful planning.

假如只是放弃了对软件的版权就产生了自由软件，那么将软件发布到公共领域是产生自由软件最简单和最直接的方式，这看起来是理所当然的。事实上，一些主要的自由软件项目已经选择了这种方法来使他们的软件成为自由软件。然而，现存的大多数自由软件*是*受版权保护的。在大多数情况下（特别是在FSF和GNU项目中），这些项目的规划都非常仔细。

Software released into the public domain does grant freedom to those users who receive the standard versions on which the original author disclaimed copyright. However, since the work is not copyrighted, any nontrivial modification made to the work is fully copyrightable.

当原作者将作品发布到公共领域以否认版权时，就将软件自由授予了那些已经收到标准版本的用户。虽然原作品不受版权保护，但对原作品所做的任何重要修改都是受版权保护的。

Free Software released into the public domain initially is Free, and perhaps some who modify the software choose to place their work into the public domain as well. However, over time, some entities will choose to proprietarize their modified versions. The public domain body of software feeds the proprietary software. The public commons disappears, because fewer and fewer entities have an incentive to contribute back to the commons. They know that any of their competitors can proprietarize their enhancements. Over time, almost no interesting work is left in the public domain, because nearly all new work is done by proprietarization.

起初，发布到公共领域的自由软件是自由的，一些修改软件的人也会选择将他们的作品发布到公共领域。然而，随着时间的推移，一些实体选择将其修改后的版本专有化。公共领域的软件主体为专有软件提供了支持。随着越来越少的实体有动力回馈公共领域，公共资源就消失了。他们知道，任何竞争对手都可以将自己的增强功能专有化。随着时间的推移，公共领域几乎不会留下任何有趣的项目，因为几乎所有的新项目都是由专有化的实体完成的。

A legal mechanism is needed to redress this problem. FSF was in fact originally created primarily as a legal entity to defend software freedom, and that work of defending software freedom is a substantial part of its work today. Specifically because of this "embrace, proprietarize and extend" cycle, FSF made a conscious choice to copyright its Free Software, and then license it under "copyleft" terms. Many, including the developers of the kernel named Linux, have chosen to follow this paradigm.

因此，需要一个法律机制来解决这个问题。事实上，FSF最初主要是作为一个捍卫软件自由的法律实体而创建的，而捍卫软件自由是其现在工作的重要组成部分。特别是由于这种“拥抱、专有化和扩展”的循环，FSF有意识地选择对其自由软件进行版权保护，然后根据“copyleft”条款对其进行许可。许多人，包括Linux内核的开发人员，都选择遵循这种模式。

Copyleft is a strategy of utilizing copyright law to pursue the policy goal of fostering and encouraging the equal and inalienable right to copy, share, modify and improve creative works of authorship. Copyleft (as a general term) describes any method that utilizes the copyright system to achieve the aforementioned goal. Copyleft as a concept is usually implemented in the details of a specific copyright license, such as the [GNU General Public License (GPL)](#_bookmark259) and the Creative Commons Attribution Share Alike License (the latter of which is the license of this work itself). Copyright holders of creative work can unilaterally implement these licenses for their own works to build communities that collaboratively share and improve those copylefted creative works.

Copyleft是一种利用版权法来实现政策目标的策略，意在促进和鼓励平等和不可剥夺的复制、共享、修改和改进原创作品的权利。Copyleft（作为一个通用术语）描述了利用版权系统实现上述目标的一些方法。Copyleft作为一个概念，通常在特定版权许可证的细节中体现，例如[GNU 通用公共许可 (GPL)](#_bookmark259) 和（Creative Commons Attribution Share Alike License）知识共享署名共享类似许可（后者是这个项目本身的许可证）。创意作品的版权持有者可以单方面为自己的作品实施这些许可，建立社区，共同分享和改进这些copyleft的创意作品。

Copyleft uses functional parts of the copyright system to achieve an unusual result (legal protection for free sharing). Copyleft modifies, or "hacks" copyright law, which is usually employed to strengthen the rights of authors or publishers, to strengthen instead the rights of users. Thus, Copyleft is a legal strategy and mechanism to defend, uphold and propagate software freedom. The basic technique of copyleft is as follows: copyright the software, license it under terms that give all the software freedoms, but use the copyright law controls to ensure that all who receive a copy of the software have equal rights and freedom. In essence, copyleft grants freedom, but forbids others to forbid that freedom to anyone else along the distribution and modification chains.

Copyleft使用版权系统的功能部分来实现一个不同寻常的结果（免费共享的法律保护）。Copyleft修改或“破解”版权法以加强用户的权利，而版权法通常用于加强作者或出版商的权利。因此，Copyleft是一种捍卫、支持和传播软件自由的法律策略和机制。Copyleft的基本原则为：对软件进行版权保护，在赋予所有软件自由的条款下颁发软件许可证，但使用版权法控制，以确保所有获得软件副本的人都享有平等的权利和自由。本质上，copyleft赋予用户自由，也禁止某些用户的垄断行为，即通过控制软件的分发和修改的后续链条限制其他人的软件自由。

Copyleft's "reciprocity" or "share and share alike" rule protects both developers, who avoid facing a "prioritized" competitor of their project, and users, who can be sure that they will have all four software freedoms --- not only in the present version of the program they use, but in all its future improved versions. Copyleft is a
general concept. Much like ideas for what a computer might do must be *implemented* by a program that actually does the job, so too must copyleft be implemented in some concrete legal structure. "Share and share alike" is a phrase that is used often enough to explain the concept behind copyleft, but to actually make it work in the real world, a true implementation in legal text must exist, written as a "copyright license". The GPL implements the concept of copyleft for software-oriented and other functional works of a technical nature. The "CC BY SA" license implements copyleft for works of textual, musical and visual authorship, such as this tutorial.

Copyleft的“互惠”或“共享和类似共享”的原则同时保护了开发者和用户，开发者可以避免面对他们项目的“优先”竞争对手，用户可以确保他们将拥有所有的四种软件自由——不仅限于当前他们使用的程序版本，也包括未来的所有改进版本中。Copyleft是一个笼统的概念。就像计算机可以做什么的想法必须由一个实际执行该任务的程序*实现*一样，copyleft也必须在某些具体的法律结构中实现。“共享和类似共享”这个短语经常被用来解释copyleft背后的概念，但要真正让它在现实世界中发挥作用，必须有一个真正的法律文本实现，即“版权许可”。GPL为面向软件和其他技术性质的功能性作品实现了copyleft的概念。 “CC BY SA”许可证为文本、音乐和视觉作者的作品提供了copyleft版权保护，例如本教程。

Copyleft advocates often distinguish between the concept of a "strong copyleft" or a "weak copyleft". However, "strong vs. weak" copyleft is not a dichotomy, it's a spectrum. The strongest copylefts strive to the exclusive rights that copyright grants to authors as extensively as possible to maximize software freedom.

Copyleft倡导者经常区分“强copyleft”或“弱copyleft”的概念。然而，“强与弱”copyleft并不是二分法原则，而是一个范围。最强的copyleft版权力图授予作者尽可能广泛的专有权，以最大限度地提高软件自由度。

As a copyleft gets "weaker", the copyleft license typically makes "trade offs" that might impede software freedom, but reach other tactic goals for the community of users and developers of the work.

随着copyleft变得“微弱”，copyleft许可证可能会做一些"权衡"，可能会阻碍软件自由，但会实现用户和项目开发者社区的其他策略目标。

In other words, strong copyleft licenses place the more requirements on how "the work" is licensed. The unit of copyright law is "the work". In that sense, the "work" referenced by the licenses is anything that can be copyrighted or will be subject to the terms of copyright law. Strong copyleft licenses exercise their scope fully.
Anything which is "a work" or a "work based on a work" licensed under a strong copyleft is subject to its requirements, including the requirement of complete, corresponding source code <sup>6</sup>. Thus, copyleft licenses, particularly strong ones, seek to ensure the same license covers every version of "work based on the work", as recognized by local copyright law, and thereby achieve the specific strategic policy aim of ensuring software freedom for all users, developers, authors, and readers who encounter the copylefted work.

换句话说，较强的copyleft许可对“作品”的许可方式提出了更高的要求。是以“作品”为单位进行版权法认定的。从这个意义上说，许可证所指的“作品”是任何可以受版权保护或受版权法条款约束的东西。较强的copyleft许可证充分发挥了其作用。任何基于较强的copyleft许可的“作品”或“基于作品的作品”都必须遵守其要求，包括所有相应的源代码 <sup>6</sup>。因此，copyleft许可证，特别是较强的许可证，旨在确保相同的许可证涵盖当地版权法认可的“基于作品的作品”的所有版本，从而确保实现与当前copyleft版权作品相关的所有用户、开发者、作者和读者的软件自由的特定战略目标。

<sup>6</sup> Copyleft communities' use of the term "strong copyleft" is undoubtedly imprecise. For example, most will call the GNU GPL a "strong copyleft" license, even though the GPL itself has various exceptions, such as the [GPLv3's system library exception](#the-system-library-exception) written into the text of the license itself. Furthermore, the copyleft community continues to debate where the a license cross the line from "strong copyleft" to "license that fails to respect software freedom", although ultimately these debates are actually regarding whether the license fits [Free Software definition](#the-free-software-definition) at all.

<sup>6</sup> Copyleft社区使用术语“强copyleft”无疑是不准确的。例如，大多数人会认为GNU GPL是“强copyleft”许可证，但其实GPL本身有多种例外情况，比如许可证文本中的[GPLv3的系统库例外情况](#the-system-library-exception)。此外，copyleft社区一直在争论许可证从“强copyleft”到“不尊重软件自由的许可证”之间的界限，尽管最终这些争论实际上是关于许可证是否符合 [自由软件的定义](#the-free-software-definition)

#### Software and Non-Copyright Legal Regimes

#### 软件和非版权法律制度

The use, modification and distribution of software, like many endeavors, simultaneously interacts with multiple different legal regimes. As was noted early via footnotes, copyright is merely the *most common way* to restrict users' rights to copy, share, modify and/or redistribute software. However, proprietary software licenses typically use every mechanism available to subjugate users. For example:

与许多努力一样，软件的使用、修改和分发同时与多种不同的法律制度相互制约。正如早期通过脚注指出的那样，版权只是限制用户复制、共享、修改和/或重新分发软件的*最常见的方式*。但是专有软件许可证通常会使用所有各种机制来控制用户。例如：

- Unfortunately, despite much effort by many in the software freedom community to end patents that read on software (i.e., patents on computational ideas), they still exist. As such, a software program might otherwise seem to be unrestricted, but a patent might read on the software and ruin everything for its users.<sup>7</sup>

- 软件自由社区中的人做了很多努力，希望能终止通过读取软件内容生成专利的行为（即跟软件思想相关的专利），但还是未能成功。因此，一个软件程序可能看起来不受限制，但有些人可能会读取该软件并生成专利，进而毁掉其他用户的一切。<sup>7</sup>

<sup>7</sup>See [6,](#_bookmark68) [7.5,](#gplv2-7-give-software-liberty-or-give-it-death) [9.14](#gplv3-11-explicit-patent-licensing) for more discussion on how
the patent system interacts with copyleft, and read Richard M. Stallman's essay, [*Let's Limit the Effect of Software Patents, Since
We Can't Eliminate Them*](http://www.wired.com/opinion/2012/11/richard-stallman-software-patents/) for more information on the problems these patents present to society.

<sup>7</sup>有关专利制度如何与copyleft交互的更多讨论，请参见[第6章](#_bookmark68)、[第7.5节](#gplv2-7-give-software-liberty-or-give-it-death)和[第9.14节](#gplv3-11-explicit-patent-licensing)，也请阅读Richard M. Stallman的文章 [*如果无法消除软件专利的影响就限制它吧*](http://www.wired.com/opinion/2012/11/richard-stallman-software-patents)，了解有关这些专利给社会带来的问题的更多信息。

Digital Restrictions Management (usually called *DRM* ) is often used to impose technological restrictions on users' ability to exercise software freedom that they might otherwise be granted.<sup>8</sup> The simplest (and perhaps oldest) form of DRM, of course, is separating software source code (read by humans),
from their compiled binaries (read only by computers). Furthermore, [17 USC 1201](http://www.law.cornell.edu/uscode/text/17/1201) often prohibits users legally from circumventing some of these DRM systems.

虽然授予了软件自由，但数字限制管理（也被称为*DRM*）通常对用户行使软件自由的能力施加技术限制。<sup>8</sup>最简单的（也是最古老的）DRM的形式，是将软件源代码（人类可阅读的）与编译的二进制文件（仅由计算机读取）分开。此外，[《美国法典》第17篇 第§102章节](http://www.law.cornell.edu/uscode/text/17/1201) 通常从法律层面禁止用户规避DRM系统中的一些。

<sup>8</sup> See [9.5](#gplv3s-views-on-drm-and-device-lock-down) for more information on how GPL deals with this issue.

<sup>8</sup> 想要了解GPL如何处理这类问题，可以查看[第9.5节](#gplv3s-views-on-drm-and-device-lock-down)

Most EULAs also include a contractual agreement that bind users further by forcing them to agree to a contractual, prohibitive software license before ever even using the software.

大多数EULA协议还包括一份用户合同，强制用户在使用软件之前同意合同性的、禁止性的软件许可来进一步约束用户。

Thus, most proprietary software restricts users via multiple interlocking legal and technological means. Any license that truly respect the software freedom of all users must not only grant appropriate copyright permissions, but also *prevent* restrictions from other legal and technological means like those listed above.

所以，大多数专有软件会通过多种相互关联的法律和技术手段来限制用户。任何真正尊重用户软件自由的许可证，不仅必须授予适当的版权许可，还必须*防止*上述其他法律和技术手段的限制。

#### Non-USA Copyright Regimes

#### 美国之外的版权制度

Generally speaking, copyright law operates similarly enough in countries that have signed the Berne Convention on Copyright, and software freedom licenses have generally taken advantage of this international standardization of copyright law. However, copyright law does differ from country to country, and commonly, software freedom licenses like the GPL must be considered under the copyright law in the jurisdiction where any licensing dispute occurs.

一般来说，在签署了《伯尔尼版权公约》的国家中，版权法的运作非常相似，软件自由许可通常采用了国际标准化的版权法。然而，不同国家的版权法确实有所不同，通常像GPL这样的软件自由许可，必须在发生许可纠纷的司法管辖区，根据版权法予以考虑。

Those who are most familiar with the USA's system of copyright often are surprised to learn that there are certain copyright controls that cannot be waived nor disclaimed. Specifically, many copyright regimes outside the USA recognize a concept of moral rights of authors. Typically, moral rights are fully compatible with respecting software freedom, as they are usually centered around controls that software freedom licenses generally respect, such as the right of an authors to
require proper attribution for their work.

那些最熟悉美国版权制度的人通常会惊讶地发现，有些版权控制既不能放弃也不能否认。具体来说，美国以外的许多版权制度都承认作者的道德权利概念。通常，道德权利与尊重软件自由完全兼容，因为道德权利通常是以软件自由许可所允许的控制为中心，例如作者要求对其作品进行适当归属的权利。

### A Community of Equality

### 平等的社区

The previous section described the principles of software freedom, a brief introduction to mechanisms that typically block these freedoms, and the simplest ways that copyright holders might grant those freedoms to their users for their copyrighted works of software. The previous section also introduced the idea of *copyleft* : a licensing mechanism to use copyright to not only grant software freedom to users, but also to uphold those rights against those who might seek to curtail them.

上一节描述了软件自由的原则，简要介绍了阻止这些自由的一些机制，以及版权所有者授予用户软件自由的最简单的方式，允许用户使用受版权保护的软件作品。同时还介绍了*copyleft* 的概念：一种使用版权的许可机制，不仅可以授予用户软件自由，还可以维护这些权利，防止试图限制这些权利的人。

Copyleft, as defined in [1.2.2,](#why-copyright-free-software) is a general term for this mechanism. The remainder of this text will discuss details of various real-world implementations of copyleft --most notably, the GPL.

如[第1.2.2节](#why-copyright-free-software)的Copyleft定义，它是该机制的一个通用术语。本书的其他章节将会讨论现实世界中copyleft的一些实现方式 -- 最值得注意的就是GPL。

This discussion begins first with some general explanation of what the GPL is able to do in software development communities. After that brief discussion in this section, deeper discussion of how GPL accomplishes this in practice follows in the next chapter.

讨论首先会解释GPL在软件开发社区中的作用。本节只进行简短讨论，下一章将深入讨论GPL如何在实践中实现这一点。

Simply put, though, the GPL ultimately creates a community of equality for both business and noncommercial users.

不过，简单来说，最终GPL为商业用户及非商业用户创建了一个平等的社区。

#### The Noncommercial Community

#### 非商业社区

A GPL'd code base becomes a center of a vibrant development and user community. Traditionally, volunteers, operating noncommercially out of keen interest or "scratch an itch" motivations, produce initial versions of a GPL'd system. Because of the efficient distribution channels of the Internet, any useful GPL'd system is adopted quickly by noncommercial users.

GPL的代码库已经成为充满活力的开发者和用户社区的中心。一般来说，出于浓厚的兴趣爱好或“试一把”的动机，志愿者会以非商业的方式制作一个GPL系统的初始版本。由于互联网的高效分发渠道，任何有用的GPL系统都会很快被非商业用户所采用。

Fundamentally, the early release and quick distribution of the software gives birth to a thriving noncommercial community. Users and developers begin sharing bug reports and bug fixes across a shared intellectual commons. Users can trust the developers, because they know that if the developers fail to address their needs or abandon the project, the GPL ensures that someone else has the right to pick up development. Developers know that the users cannot redistribute their software without passing along the rights granted by the GPL, so they are assured that every one of their users is treated equally.

从根本上来说，软件的早期发布和快速分发催生了一个繁荣的非商业社区。用户和开发人员都在知识共享的社区中分享错误报告和修复补丁。用户非常信任开发人员，因为他们知道如果开发人员不能满足他们的需求或放弃项目，GPL协议能确保其他人有权接手并持续开发。开发人员知道，如果将GPL的权利授予用户，用户就没法二次分发他们的软件，因此他们需要确信每一位用户受到平等对待。

Because of the symmetry and fairness inherent in GPL'd distribution, nearly every GPL'd package in existence has a vibrant noncommercial user and developer base.

就是因为GPL分发协议的对称性和公平性，几乎每个GPL项目都拥有一个活跃的非商业用户和开发者群体。

#### The Commercial Community

#### 商业群体

By the same token, nearly all established GPL'd software systems have a vibrant commercial community. Nearly every GPL'd system that has gained wide adoption from noncommercial users and developers eventually begins to fuel a commercial system around that software.

同样，几乎所有已建立的GPL软件系统都有一个充满活力的商业社区。每个获得非商业用户和开发人员拥护的GPL系统，最终几乎都开始围绕该软件为商业系统提供动力。

For example, consider the Samba file server system that allows Unix-like systems (including GNU/Linux) to serve files to Microsoft Windows systems. Two graduate students originally developed Samba in their spare time and it was deployed noncommercially in academic environments.<sup>9</sup> However, very soon for-profit
companies discovered that the software could work for them as well, and their system administrators began to use it in place of Microsoft Windows NT file-servers. This served to lower the cost of running such servers by orders of magnitude. There was suddenly room in Windows file-server budgets to hire contractors to improve Samba. Some of the first people hired to do such work were those same two graduate students who originally developed the software.

例如，以Samba文件服务器系统为例，它允许类Unix系统（如GNU/Linux）向微软的Windows系统提供文件服务。Samb最初是由两名研究生在业余时间开发的，并在学术环境中部署，并未商业化。<sup>9</sup> 之后很快商业公司就发现了该软件也适用于他们，公司的系统管理员开始使用它取代了微软的Windows NT文件服务器。这有助于将此类服务器的运行成本降低几个数量级。Windows文件服务器就有了多的预算空间，可以雇用承包商来改进Samba。最早受雇从事这项工作的正是最初开发该软件的两名研究生。

<sup>9</sup>See [Andrew Tridgell's "A bit of history and a bit of fun"](http://turtle.ee.ncku.edu.tw/docs/samba/history)

<sup>9</sup> 详情请看[Andrew Tridgell的《一点历史，一份趣味》](http://turtle.ee.ncku.edu.tw/docs/samba/history)

The noncommercial users, however, were not concerned when these two fellows began collecting paychecks off of their GPL'd work. They knew that because of the nature of the GPL that improvements that were distributed in the commercial environment could easily be folded back into the standard version. Companies are not permitted to
proprietarize Samba, so the noncommercial users, and even other commercial users are safe in the knowledge that the software freedom ensured by the GPL will remain protected.

当那两位学生开始从他们的GPL工作中获取报酬时，非商业用户也并不担心。他们知道，由于GPL的性质，在商业环境中实现的改进会很快地融入到标准版本。不允许任何公司将Samba私有化，非商业用户、其他商业用户都知道，GPL协议会确保软件自由将继续受到保护。

Commercial developers also work in concert with noncommercial developers. Those two now-long-since graduated students continue to contribute to Samba altruistically, but also get paid work doing it. Priorities change when a client is in the mix, but all the code is contributed back to the standard version. Meanwhile, many other
individuals have gotten involved noncommercially as developers, because they want to "cut their teeth on Free Software," or because the problems interest them. When
they get good at it, perhaps they will move on to another project, or perhaps they will become commercial developers of the software themselves.

商业开发商也会与非商业开发商合作。那两位已经毕业了的学生继续无私地为Samba做出贡献，但同时也获得了报酬。当有客户参与其中时，优先级会发生变化，但所有的代码都会回馈给标准版本。与此同时，许多其他人也作为开发者参与了非商业活动，因为他们想“在自由软件上小试牛刀”，或者是他们对这些问题感兴趣。当他们擅长编程时，也许会转向另一个项目，或者他们自己可能会成为软件的商业开发人员。

No party is a threat to another in the GPL software scenario because everyone is on equal ground. The GPL protects rights of the commercial and noncommercial contributors and users equally. The GPL creates trust, because it is a level playing field for all.

在GPL软件场景中，任何一方都不会对另外一方构成威胁，因为每个人都是平等的。GPL协议平等地保护了商业和非商业贡献者和用户的权利。GPL协议创造信任，因为它位所有人提供了公平的竞争环境。

#### Law Analogy

#### 法律类比

In his introduction to Stallman's *Free Software, Free Society*, Lawrence Lessig draws an interesting analogy between the law and Free Software. He argues that the laws of a free society must be protected much like the GPL protects software. So that I might do true justice to Lessig's argument, I quote it verbatim:

在介绍Stellman的《自由软件、自由社会》时，Lawrence Lessig在法律和自由软件之间做了一个有趣的类比。他认为自由社会的法律也需要受到保护，就像GPL协议保护软件一样。为了能真正公正地对待Lessig的论点，我逐字引用了它：

A "free society" is regulated by law. But there are limits that any free society places on this regulation through law: No society that kept its laws secret could ever be called free. No government that hid its regulations from the regulated could ever stand in our tradition. Law controls. But it does so justly only when visibly. And law is visible only when its terms are knowable and controllable by those it regulates, or by the agents of those it regulates (lawyers, legislatures).

“自由社会”是受法律规范的。但是任何自由社会都通过法律对这种规定施加了限制：任何对法律保密的社会都不能被称为自由。任何向受监管者隐藏其法规的政府都无法立足于我们的传统。法律控制。但只有在显而易见的情况下，它才会这样做。法律只有在其条款可被监管者或监管者的代理人（律师、立法机关）知晓和控制时才是可见的。

This condition on law extends beyond the work of a legislature. Think about the practice of law in American courts. Lawyers are hired by their clients to advance their clients' interests. Sometimes that interest is advanced through litigation. In the course of this litigation, lawyers write briefs. These briefs in turn affect opinions written by judges. These opinions decide who wins a particular case, or whether a certain law can stand consistently with a constitution.

这种法律条件超出了立法机关的工作范围。想想美国法院的法律实践。律师受雇于他们的客户，目的是促进他们客户的利益。有时，这种利益是通过法律诉讼来推进的。在此诉讼过程中，律师撰写简报。这些简报反过来会影响法官撰写的意见。这些意见决定了在某一案件中谁会获胜，或者某项法律是否能够与宪法保持一致。

All the material in this process is free in the sense that Stallman means. Legal briefs are open and free for others to use. The arguments are transparent (which is different from saying they are good), and the reasoning can be taken without the permission of the original lawyers. The opinions they produce can be quoted in later briefs. They can be copied and integrated into another brief or opinion. The "source code" for American law is by design, and by principle, open and free for anyone to take. And take lawyers do---for it is a measure of a great brief that it achieves its creativity through the reuse of what happened before. The source is free; creativity and an economy is built upon it.

正如Stallman所说，这个过程中的所有材料都是免费的。法律简报是公开的，可供他人免费使用。论据透明（这不同于说它们是好的），无需原律师许可即可取证。他们提出的意见可以在以后的简报中引用。可以将它们复制并整合到另一份简报或意见中。美国法律的“源代码”在设计上和原则上都是开放的，任何人都可以免费使用。以律师的做法为例——因为这是一个伟大的简报的衡量标准，
它通过重用以前的案例来实现其创造力。来源是免费的；创造力和经济是建立在它之上的。

This economy of free code (and here I mean free legal code) doesn't starve lawyers. Law firms have enough incentive to produce great briefs even though the stuff they build can be taken and copied by anyone else. The lawyer is a craftsman; his or her product is public. Yet the crafting is not charity. Lawyers get paid; the public doesn't demand such work without price. Instead this economy flourishes, with later work added to the earlier.

这种免费代码经济（这里我指的是免费法律代码）不会让律师挨饿。律师事务所有足够的动力来制作出色的简报，即使他们制作的东西可以被其他任何人拿走和复制。律师是工匠；他或她的简报是公开的。然而，手工艺品不是慈善。律师得到报酬；公众不会要求律师无偿工作。取而代之的是，这种经济会蓬勃发展，后期的工作会逐渐添加到早期的工作中。

We could imagine a legal practice that was different --- briefs and arguments that were kept secret; rulings that announced a result but not the reasoning. Laws that were kept by the police but published to no one else. Regulation that operated without explaining its rule.

我们可以想象一种不同的法律实践——保持简报和论据的保密性；宣布结果但不宣布推理的裁决。警察遵守的法律，但不向其他人公开。没有解释规则的相关规定。

We could imagine this society, but we could not imagine calling it "free." Whether or not the incentives in such a society would be better or more efficiently allocated, such a society could not be known as free. The ideals of freedom, of life within a free society, demand more than efficient application. Instead, openness and transparency are the constraints within which a legal system gets built, not options to be added if convenient to the leaders. Life governed by software code should be no less.

我们可以想象这样的社会，但我们无法假装称它为“自由”。无论这个社会中的激励是否会得到更好或更有效的分配，这样的社会都不能被称为自由。自由的理想，自由社会中的生活，需要的不仅仅是有效的应用。相反，公开和透明是建立法律体系的约束条件，而不是领导者需要时可以随意添加的选项。由软件代码支配的生活应该不会少。

Code writing is not litigation. It is better, richer, more productive. But the law is an obvious instance of how creativity and incentives do not depend upon perfect control over the products created. Like jazz, or novels, or architecture, the law gets built upon the work that went before. This adding and changing is what creativity always is. And a free society is one that assures that its most important resources remain free in just this sense.[^10^](#_bookmark26)

代码编写不是法律诉讼。它更好、更丰富、更有生产力。但创造力和激励是不依赖于对所创造产品的完美与否的，法律就是一个明显的例子。就像爵士乐、小说或建筑一样，法律是建立在之前的作品之上的。这种添加和改变就是创造力的本质所在。一个自由的社会就是确保其最重要的资源在某种意义上保持免费。<sup>10</sup>

<sup>10</sup>This quotation is Copyright c 2002, Lawrence Lessig. It is licensed under the terms of [the "Attribution License" version 1.0](http://creativecommons.org/licenses/by/1.0/) or any later version as published by Creative Commons.

<sup>10</sup>此引文版权所有c 2002, Lawrence Lessig. 它根据[“署名许可”版本1.0](http://creativecommons.org/licenses/by/1.0/)或Createive Comments 发布的任何更新条款获得许可。

In essence, lawyers are paid to service the shared commons of legal infrastructure. Few citizens defend themselves in court or write their own briefs (even though they are legally permitted to do so) because everyone would prefer to have an expert do that job.

从本质上讲，律师是为法律基础设施的公共服务而工作的。很少有公民在法庭上为自己辩护或撰写自己的案情简报（即使法律允许他们这样做），每个人都更愿意让专家来做这项工作。

The Free Software economy is a market ripe for experts. It functions similarly to other well established professional fields like the law. The GPL, in turn, serves as the legal scaffolding that permits the creation of this vibrant commercial and noncommercial Free Software economy.

对于专家来说，自由软件经济是一个成熟的市场。它的功能类似于法律等其他成熟的专业领域。反过来，GPL协议又是一个法律脚手架，允许创建这个充满活力的商业和非商业的自由软件经济。
