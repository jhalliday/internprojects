# Red Hat Newcastle Student Projects

Starting from 2021 this page replaces [https://developer.jboss.org/docs/DOC-17343](https://developer.jboss.org/docs/DOC-17343)
as the definitive source of information specifically on internship placements at Red Hat Newcastle for students at local Universities.

### Not quite what you're looking for?
- For global information try [Red Hat Research](https://research.redhat.com)
- Legacy information for JBoss research projects is also available at
[https://developer.jboss.org/docs/DOC-12331](https://developer.jboss.org/docs/DOC-12331)
- [Google Summer of Code](https://summerofcode.withgoogle.com/) projects are at
  [https://spaces.redhat.com/display/GSOC/GSOC+-+Google+Summer+Of+Code](https://spaces.redhat.com/display/GSOC/GSOC+-+Google+Summer+Of+Code)

---

## Project Proposals

The following projects are offered to students for summer 2024.

'Specialist skills' identify advanced topics likely to be of relevance to the project. These may be things you wish to demonstrate you already have, making you a more attractive candidate for the project, or things you wish to learn, making the project more attractive to you.


### WebAssembly Java integration

WebAssembly is a binary instruction format for a virtual machine, providing a portable compilation target for several languages.
Embedded in many web browsers, it interoperates well with JavaScript. Interoperability with other languages, including Java, is as yet more limited.

In this project you will investigate and enhance the integration of WebAssembly and JVM languages, with particular attention to allowing method calls and data sharing between Java and WASM code.

Specialist skills: low level (assembly) programming, virtual machines.

Reading:
[WebAssembly](https://webassembly.org/) ;
[Wasmer](https://wasmer.io/) ;
[Extism](https://extism.org/) ;
[GraalWASM](https://www.graalvm.org/latest/reference-manual/wasm/)

### Transaction interoperability in WebAssembly

WebAssembly provides a compilation target for code written in multiple languages including C, C++, and Rust, and uniquely standardizes the mechanism for function call interoperability and data sharing regardless of the component languages used.

Transaction standards define how components and business logic from different vendors can interoperate to guarantee data integrity. XA, a C-based API specification, is widely implemented by databases, message queues and application runtime platforms.

As an emerging platform, WebAssembly lacks such transaction support at present, limiting its usefulness in enterprises accustomed to this functionality.

In this project, with a focus on the premium open-source transaction manager Narayana, you will investigate how XA distributed transactions can be provided in the WebAssembly ecosystem, with a emphasis on interoperation between components written in different languages.

Specialist skills: polyglot programming, distributed transactions, database drivers, virtual machines.

Reading:
[WebAssembly](https://webassembly.org/) ;
[Extism](https://extism.org/) ;
[Narayana](https://www.narayana.io/)

### Transactional Microservices in Webassembly

WebAssembly (WASM) is emerging as a language neutral compilation target for server-side microservices frameworks, offering good portability and small deployment footprints. Its web and database support is evolving rapidly, building on WASI, WASIX and the WASM component model. At this early stage many opportunities exist to add further foundational capabilities to the platform and shape its future.

Microprofile’s Long-Running Action (LRA) protocol provides an open, interoperable standard for implementing transactional microservices. Enhancing existing WASM web support with LRA capabilities would increase its utility for business applications.

In this project, the student will craft an LRA participant in a language of their preference and use WebAssembly to make it available on the web, providing the world's first such example of using the platform in this way.

Specialist skills: polyglot programming, web services, distributed transactions, LRA protocol.

Reading:
[WebAssembly](https://webassembly.org/) ;
[Spin](https://developer.fermyon.com/spin/v2/index) ;
[Narayana](https://www.narayana.io/) ;
[LRA](https://download.eclipse.org/microprofile/microprofile-lra-1.0-M1/microprofile-lra-spec.html)

### Project Panama evaluation

OpenJDK's [Project Panama](https://jdk.java.net/panama/) foreign function and memory support offers a new approach to calling native libraries from Java.
Whilst the project is aimed initially at providing an alternative to [JNI](https://docs.oracle.com/en/java/javase/17/docs/specs/jni/index.html) for access to C code, it also has potential for facilitating interoperability with other formats such as WebAssembly's [component model](https://github.com/WebAssembly/component-model) ABI or memory layout mechanisms such as [Apache Arrow](https://arrow.apache.org/).

In this project you will evaluate the use of Panama's API and tooling for these alternative use cases and develop guidance and tool support for its use in such tasks.

Specialist skills: machine architecture and in-memory data representation, C programming, WebAssembly.

Reading:
[JEP 454: Foreign Function & Memory API](https://openjdk.org/jeps/454)

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
[Lux AI](https://www.lux-ai.org/) ;
[battlecode](https://battlecode.org/) ;
[microcorruption](https://microcorruption.com/login)


### Enhanced Flame Graph rendering

Flame Graphs are a popular mechanism for visualising stack trace data from software performance profiles. However, they are often poorly integrated with other developer tools, particularly source code browsers and editors.

In this project, you will enhance tools for rendering Flame Graphs of Java code profiles, to hyperlink frames to function source code.

Specialist skills: html/svg, profiling tools, source code management and CI/CD tools, IDE plugins.

Reading:
[Flame Graphs](https://www.brendangregg.com/flamegraphs.html) ;
[async-profiler](https://github.com/jvm-profiling-tools/async-profiler/#flame-graph-visualization) ;
[Java Flight Recorder](https://docs.oracle.com/en/java/java-components/jdk-mission-control/8/user-guide/whats-new-jdk-mission-control.html#GUID-412659B5-9BA1-4895-B670-245D6823A8BC) ;
[Sourcegraph](https://about.sourcegraph.com/)

### Observability signal correlation

Efficient use of observability signals, which consist of logs, metrics, traces and profiling data, is key to managing software systems in production.
Emerging trends in observability operations place an increasing emphasis on the value of correlating these signal types to investigate issues,
but supporting this requirement fully involves adding new functionality to observability signal generation mechanisms.

In this project you will investigate and improve observability signal correlation in the JVM ecosystem,
with a focus on trace ids and code profiling tools.

Specialist Skills: Observability, DevOps, JVM platform (C/C++) programming, eBPF.

Reading:
[OpenTelemetry](https://opentelemetry.io/) ;
[async-profiler](https://github.com/jvm-profiling-tools/async-profiler/) ;
[Java Flight Recorder](https://docs.oracle.com/en/java/java-components/jdk-mission-control/8/user-guide/)



### FinOps and profiling datastore design.

For cost-efficient cloud computing utilization, the disciplines of DevOps and finance must be combined to understand spending and manage resources.
Within the emerging field of Cloud FinOps, data generated by code profilers can be combined with cloud CPU cost data to give stakeholders new insights.
However, this requires integrating data traditionally held in separate systems and presenting it in a matter intelligible to users with different backgrounds and expectations.

In this project you will investigate the tools and standards available for data managment in the area of FinOps and devise storage and query approaches focussed on attributing costs to code at a fine-grained (i.e. function call) level.

Specialist Skills: Accounting, Observability.

Reading:
[OpenCost](https://www.opencost.io/)



### Create your own project

Internship candidates may also submit proposals of their own devising, in the form of a brief outline of the topic and a clear description of how it aligns with Red Hat's needs.
Topics may be original, or drawn from existing open source project roadmaps and JIRA/github issues.

---

## Application Procedure

Select one preferred project and optionally one reserve choice from the list above.
Send me your choices, along with a CV and a portfolio of source code that you think demonstrates your software engineering skills well.
Submitted work should be in Java, unless the selected project topic specifically calls for another language.
The topic choices will be used to route your application to the relevant supervisor(s),
who will review your application and may then invite you to a technical interview.

Note that initial code review is typically a harder step than the subsequent interview.
Allow sufficient preparation time to assemble a suitable portfolio of work for your application.
Applications may include university coursework, but preferably should not consist entirely of such structured exercises.
Ensure you have the necessary rights to all the work submitted. In particular, DO NOT submit work done in the course of employment unless it is explicitly open source or you have the employer's permission to disclose it.

We like: links to github repos; originality; documentation; unit tests.

We don't like: cover letters; code that doesn't compile; tests that fail.

For summer 2024 we expect to be operating entirely online.
Depending on circumstances, there may also be the option of working from our Newcastle office.

**Deadline for applications: 12 noon, Friday 16th February, 2024.**

---

## Interview Process

If your application is good enough, you'll be invited to interview. This will be an online discussion with the supervisor of your preferred project and perhaps some of their engineering team, lasting up to 30 minutes. In most cases this will be the only interview you need to do.

The interview structure depends on the supervisor, but will be largely technical and usually cover:

- Your educational and professional background, particularly any software engineering experience with the language of the selected project.
- The code you submitted with your application, particularly with regard to your design and implementation decisions and approach to testing. You may be asked to describe how you would tackle a new requirement or feature, but live coding will not be required.
- What Red Hat does and how placement projects at Red Hat Newcastle operate.
- The project topic you've selected, what we hope to achieve, how you will contribute and what you'll learn. Whilst the project is a learning experience, you will still be expected to demonstrate some basic understanding of the topic you've chosen and describe how you may approach the work.
- Any other questions you have.

Candidates may prepare for interview by:
- Reviewing their submitted code to ensure it's well understood.
- Reading about, or experimenting with software relevant to, the selected project topic.

