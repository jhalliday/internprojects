# Red Hat Newcastle Student Projects

For 2021 this page replaces [https://developer.jboss.org/docs/DOC-17343](https://developer.jboss.org/docs/DOC-17343)
as the definitive source of information specifically on internship placements at Red Hat Newcastle for Newcastle MSc students.

### Not quite what you're looking for?
- For global information try [Red Hat Research](https://research.redhat.com)
- Legacy information for JBoss research projects is also available at
[https://developer.jboss.org/docs/DOC-12331](https://developer.jboss.org/docs/DOC-12331)
- [Google Summer of Code](https://summerofcode.withgoogle.com/) projects are at
  [https://docs.jboss.org/display/GSOC/Google+Summer+of+Code+2021+Ideas](https://docs.jboss.org/display/GSOC/Google+Summer+of+Code+2021+Ideas)

## Project Proposals

The following projects are offered to students for summer 2021.

### io_uring for JMS

The recently added io_uring interface to the linux kernel provides for scalable, high performance, asynchronous I/O operations.
The performance of Java based messaging systems can potentially benefit from this new API. 

In this project you will evaluate the use of io_uring from Java (via JNI) to provide
enhanced persistent messaging performance in
[Apache ActiveMQ Artemis](https://activemq.apache.org/components/artemis/).

Skills: Some experience of messaging systems or JNI may be beneficial.

Reading: 
[What is io_uring?](https://unixism.net/loti/what_is_io_uring.html) ;
[Efficient IO with io_uring](https://kernel.dk/io_uring.pdf) ;
Netty transport
[blog](https://netty.io/news/2020/11/16/io_uring-0-0-1-Final.html) and
[src](https://github.com/netty/netty-incubator-transport-io_uring)

### SIMD Vector operations for Java

The new jdk.incubator.vector module provides Java with a portable API for accessing a hardware platform's vector (SIMD) instructions.
This brings the potential for accelerating many operations, including image and signal processing.
For middleware applications, however, the most interesting application may be JSON Parsing.

In this project you will evaluate the use of the new Java Vector instruction API for accelerating processing tasks applicable to Red Hat's middleware portfolio.

Skills: Some experience of vector processing, parsing or benchmarking may be beneficial.

Reading:
[JEP-338](https://openjdk.java.net/jeps/338) ;
[simdjson](https://github.com/simdjson/simdjson) ;
[mison](https://www.microsoft.com/en-us/research/publication/mison-fast-json-parser-data-analytics/)

### WebAssembly Java integration

WebAssembly is a binary instruction format for a virtual machine, providing a portable compilation target for several languages.
Embedded in many web browsers, it interoperates well with JavaScript. Interoperability with other languages, including Java, is as yet more limited.

In this project you will investigate and enhance the integration of WebAssembly and JVM languages, with particular attention to allowing calls between them, in either or both directions.

Skills: Some understanding of low level (assembly) programming and virtual machines may be beneficial.

Reading:
[WebAssembly](https://webassembly.org/) ;
[TeaVM](http://teavm.org/) ;
[JWebAssembly](https://github.com/i-net-software/JWebAssembly) ;
[Wasmer](https://wasmer.io/)

### Software archaeology for the z-machine

[Software archaeology](https://en.wikipedia.org/wiki/Software_archaeology) is the study of legacy software, which is often abandoned, incomplete, poorly documented, or able to run only on hardware platforms or in software environments which are no longer widely available.
A variety of tools and techniques are available to analyse, document, reconstruct and execute such artifacts.

The Infocom [z-machine](https://en.wikipedia.org/wiki/Z-machine) is a virtual machine developed for early text adventure games,
including key works of the genre such as [Zork](https://www.technologyreview.com/2017/08/22/149560/the-enduring-legacy-of-zork/), which thanks to software archaeology is [playable online](http://textadventures.co.uk/games/view/5zyoqrsugeopel3ffhz_vq/zork).

Java has been used to replace or emulate older tools, including z-machine interpreters.
These Java tools are now becoming legacy artifacts in their own right as projects are abandoned, leading to a form of meta-archaeology to maintain them.

In this project you will study and apply software archaeology practices, using curation of the z-machine ecosystem as a case study,
and consider its relation to the Java ecosystem and the challenges of maintaining legacy software written in Java as it itself ages.

Skills: A background in history, anthropology, archaeology or librarianship may be beneficial, as will some knowledge of virtual machine architectures and build systems.

Reading:
[ifarchive](https://ifarchive.org/) ;
[Inform Fiction](https://inform-fiction.org/) ;
[ZILCH How-to](https://github.com/ZoBoRf/ZILCH-How-to) ;
[ZAX](https://github.com/mattkimmel/zax) ;
[Zplet](https://github.com/XelaRellum/ZPlet) ;
[ZMPP](https://github.com/wandora-team/zmpp-wandora)

### Code games for software recruitment

As the structural shortage of suitably skilled candidates continues to worsen, fresh attention is being paid to means of identifying and attracting technical talent to employers.
The use of games centred on programming as a recruitment tool is gaining traction in the industry as an alternative or complement to traditional means of candidate filtering.
At present, such games focus on core skills such as algorithms and datastructures, with some attention to trends such as machine learning.

In this project you will study the ecosystem of programming games and their platforms, with attention to their relevance for identifying the skills needed by Red Hat engineers.
You will provide guidance and recommendations on the design of a game or game platform that may better suit our needs than existing offerings, perhaps including designing or prototyping.

Note: For this project, the code provided with the candidate's application MUST take the form of an original bot for playing a code game such as those linked below. Any programming language may be used 

Skills: Experience with game design, technical recruitment or middleware skills training may be beneficial.

Reading:
[codingame](https://www.codingame.com/) ;
[battlesnake](https://play.battlesnake.com/) ;
[Halite](https://halite.io/) ;
[battlecode](https://battlecode.org/)

### Roll your own project

Internship candidates may also submit proposals of their own devising, in the form of a brief outline of the topic and a clear description of how it aligns with Red Hat's needs.
Topics may be original, or drawn from existing open source project roadmaps and JIRA issues.

## Application Procedure

Select one preferred project and optionally one reserve choice from the list above.
Send us your choices, along with a CV and some source code that you think demonstrates your software engineering skills well.
This should be in Java, unless the project topic specifically calls for another language.
The topic choices will be used to route your application to the relevant supervisor(s),
who will review your application and may then invite you to a technical interview.

New proposals may be added to this page until mid February.
In such case, earlier applicants may change their project preference to one of the new topics.

We like: links to github repos; originality; documentation; unit tests.  
We don't like: cover letters; code that doesn't compile; tests that fail; code you didn't write yourself (especially if it doesn't compile or pass its tests.)
Yes, we've seen it all before... 

For summer 2021 we expect to be operating entirely online, with interviews and subsequent project supervision taking place without physical contact.
Whilst our Newcastle office may reopen over the course of the summer, attendance onsite will then be optional not mandatory.

Deadline for applications: 12 noon, Monday 22nd February, 2021.
