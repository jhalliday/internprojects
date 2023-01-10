# Red Hat Newcastle Student Projects

Starting from 2021 this page replaces [https://developer.jboss.org/docs/DOC-17343](https://developer.jboss.org/docs/DOC-17343)
as the definitive source of information specifically on internship placements at Red Hat Newcastle for Newcastle MSc students.

### Not quite what you're looking for?
- For global information try [Red Hat Research](https://research.redhat.com)
- Legacy information for JBoss research projects is also available at
[https://developer.jboss.org/docs/DOC-12331](https://developer.jboss.org/docs/DOC-12331)
- [Google Summer of Code](https://summerofcode.withgoogle.com/) projects are at
  [https://spaces.redhat.com/display/GSOC/GSOC+-+Google+Summer+Of+Code](https://spaces.redhat.com/display/GSOC/GSOC+-+Google+Summer+Of+Code)

---

## Project Proposals

The following projects are offered to students for summer 2023.

'Specialist skills' identify advanced topics likely to be of relevance to the project. These may be things you wish to demonstrate you already have, making you a more attractive candidate for the project, or things you wish to learn, making the project more attractive to you.


### WebAssembly Java integration

WebAssembly is a binary instruction format for a virtual machine, providing a portable compilation target for several languages.
Embedded in many web browsers, it interoperates well with JavaScript. Interoperability with other languages, including Java, is as yet more limited.

In this project you will investigate and enhance the integration of WebAssembly and JVM languages, with particular attention to allowing method calls and data sharing from Java to WASM code.

Specialist skills: low level (assembly) programming, virtual machines.

Reading:
[WebAssembly](https://webassembly.org/) ;
[Wasmer](https://wasmer.io/) ;
[GraalWASM](https://www.graalvm.org/latest/reference-manual/wasm/) ;
[Happy New Moon with Report](https://github.com/fishjd/HappyNewMoonWithReport)


### Code games for software recruitment

As the structural shortage of suitably skilled candidates continues to worsen, fresh attention is being paid to means of identifying and attracting technical talent to employers.
The use of games centred on programming as a recruitment tool is gaining traction in the industry as an alternative or complement to traditional means of candidate filtering.
At present, such games focus on core skills such as algorithms and datastructures, with some attention to trends such as machine learning.

In this project you will study the ecosystem of programming games and their platforms, with attention to their relevance for identifying the skills needed by Red Hat engineers.
You will provide guidance and recommendations on the design of a game or game platform that may better suit our needs than existing offerings, perhaps including designing or prototyping.

Note: For this project, the code provided with the candidate's application MUST take the form of an original bot for playing a code game such as those linked below. Any programming language may be used.

Specialist skills: game design, technical recruitment, middleware skills training.

Reading:
[codingame](https://www.codingame.com/) ;
[battlesnake](https://play.battlesnake.com/) ;
[Halite](https://halite.io/) ;
[battlecode](https://battlecode.org/) ;
[microcorruption](https://microcorruption.com/login)


### Observability database evaluation

Observability tooling is essential to DevOps teams and relies on databases capable of ingesting and indexing large volumes of observation data. With correlation of data from different signal types (logs, metrics, traces and profiles) becoming increasingly valued, such databases must be able to handle diverse data types and query patterns in a unified manner. Specialising storage solutions for one type of data e.g. time series metrics can bring benefits, but often at the cost of poorly handling other types of data. Thus unified observability databases face challenging and sometimes conflicting requirements.

In this project you will empirically evaluate and report on the data storage technologies in use across the observability tooling ecosystem, with an emphasis on identifying open source solutions suitable for combined storage of diverse signal types at scale.

Specialist skills: observability tools; databases, including distributed and no-sql.

Reading:
[OpenTelemetry](https://opentelemetry.io/docs/) ;
[FrostDB](https://www.polarsignals.com/blog/posts/2022/05/04/introducing-arcticdb/) ;
[Husky](https://www.datadoghq.com/blog/engineering/introducing-husky/) ;
[Phlare](https://grafana.com/oss/phlare/)


### Concurrency and actor frameworks on Project Loom

Project Loom brings lightweight threads to the Java platform. This opens the way to more efficient implementation of some patterns and approaches to programming concurrent systems that have previously been found useful in other languages but challenging to execute well in Java.
What higher-level constructs can Java now adopt from other languages and how will the availability of lightweight threads affect the relative attractiveness and performance of existing Java frameworks?

In this project you will investigate the concurrency programming abstractions available in the Java ecosystem and compare them to those found in other languages that already have a lightweight thread abstraction, such a golang's goroutines, Scala Actors, and Erlang processes.

Specialist skills: concurrent programming abstractions, polyglot programming.

Reading:
[Project Loom](https://openjdk.org/projects/loom/) ;
[Loom Presentation](https://speakerdeck.com/josepaumard/loom-is-blooming)


### Enhanced Flame Graph rendering

Flame Graphs are a popular mechanism for visualising stack trace data from software performance profiles. However, they are often poorly integrated with other developer tools, particularly source code browsers and editors.

In this project, you will enhance tools for rendering Flame Graphs of Java code profiles, to hyperlink frames to function source code.

Specialist skills: html/svg, profiling tools, source code management tools.

Reading:
[Flame Graphs](https://www.brendangregg.com/flamegraphs.html) ;
[async-profiler](https://github.com/jvm-profiling-tools/async-profiler/#flame-graph-visualization) ;
[Java Flight Recorder](https://docs.oracle.com/en/java/java-components/jdk-mission-control/8/user-guide/whats-new-jdk-mission-control.html#GUID-412659B5-9BA1-4895-B670-245D6823A8BC) ;
[Sourcegraph](https://about.sourcegraph.com/)


### Project Panama evaluation

OpenJDK's [Project Panama](https://jdk.java.net/panama/) foreign function support offers a new approach to calling native libraries from Java. Existing integrations across a number of Red Hat projects use the older [JNI](https://docs.oracle.com/en/java/javase/17/docs/specs/jni/index.html) solution for this requirement.
As native libraries are used to increase scalability or accelerate performance critical code at the cost of more complex build processes, the choice of integration approach is of material interest to us and any opportunity for improvement is attractive.

In this project you will identify and evaluate opportunities for replacing JNI with Panama across Red Hat's portfolio of open source projects, prototyping and benchmarking one or more solutions and reporting on issues found.

Specialist skills: C programming, micro-benchmarking, build systems.

### Low-code reactive applications

Low-code platforms such as [appsmith](https://www.appsmith.com/) aim to increase developer productivity through visual tooling and code generation techniques. However, many such platforms continue to generate older style applications which ignore the many benefits of [reactive](https://www.reactivemanifesto.org/) application architecture.

[Quarkus](https://quarkus.io/about/) is a framework for Java microservices, with full support for reactive apps and a strong focus on developer joy and efficient tooling. However, whilst it makes writing code a fast, fun experience, it does still require that code to be written largely by hand.

Bringing together low-code tooling and Quarkus has the potential to further enhance developer productivity by automating more of the routine coding required for many applications, whilst simultaneously improving runtime efficiency through use of a reactive approach.

In this project you will explore the opportunities for new tools and frameworks to extend Quarkus with greater low-code application development capabilities.

Specialist skills: reactive applications, code generation.


### Software archaeology for the z-machine

[Software archaeology](https://en.wikipedia.org/wiki/Software_archaeology) is the study of legacy software, which is often abandoned, incomplete, poorly documented, or able to run only on hardware platforms or in software environments which are no longer widely available.
A variety of tools and techniques are available to analyse, document, reconstruct and execute such artifacts.

The Infocom [z-machine](https://en.wikipedia.org/wiki/Z-machine) is a virtual machine developed for early text adventure games,
including key works of the genre such as [Zork](https://www.technologyreview.com/2017/08/22/149560/the-enduring-legacy-of-zork/), which thanks to software archaeology is [playable online](http://textadventures.co.uk/games/view/5zyoqrsugeopel3ffhz_vq/zork).

Java has been used to replace or emulate older tools, including z-machine interpreters.
These Java tools are now becoming legacy artifacts in their own right as projects are abandoned, leading to a form of meta-archaeology to maintain them.

In this project you will study and apply software archaeology practices, using curation of the z-machine ecosystem as a case study,
and consider its relation to the Java ecosystem and the challenges of maintaining legacy software written in Java as it itself ages.

Specialist skills: virtual machine architectures, build systems. A prior background in history, anthropology, archaeology or librarianship may also be beneficial.

Reading:
[ifarchive](https://ifarchive.org/) ;
[Inform Fiction](https://inform-fiction.org/) ;
[ZILCH How-to](https://github.com/ZoBoRf/ZILCH-How-to) ;
[ZAX](https://github.com/mattkimmel/zax) ;
[Zplet](https://github.com/XelaRellum/ZPlet) ;
[ZMPP](https://github.com/wandora-team/zmpp-wandora)


### Roll your own project

Internship candidates may also submit proposals of their own devising, in the form of a brief outline of the topic and a clear description of how it aligns with Red Hat's needs.
Topics may be original, or drawn from existing open source project roadmaps and JIRA/github issues.

---

## Application Procedure

Select one preferred project and optionally one reserve choice from the list above.
Send me your choices, along with a CV and some source code that you think demonstrates your software engineering skills well.
This should be in Java, unless the project topic specifically calls for another language.
The topic choices will be used to route your application to the relevant supervisor(s),
who will review your application and may then invite you to a technical interview.

We like: links to github repos; originality; documentation; unit tests.  
We don't like: cover letters; code that doesn't compile; tests that fail.

For summer 2023 we expect to be operating entirely online, with interviews and subsequent project supervision taking place without physical contact.
Depending on circumstances, there may also be the option of working from our Newcastle office.

Deadline for applications: 12 noon, Friday 24th February, 2023.
