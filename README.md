# Red Hat Newcastle Student Projects

Starting from 2021 this page replaces [https://developer.jboss.org/docs/DOC-17343](https://developer.jboss.org/docs/DOC-17343)
as the definitive source of information specifically on internship placements at Red Hat Newcastle for Newcastle MSc students.

### Not quite what you're looking for?
- For global information try [Red Hat Research](https://research.redhat.com)
- Legacy information for JBoss research projects is also available at
[https://developer.jboss.org/docs/DOC-12331](https://developer.jboss.org/docs/DOC-12331)
- [Google Summer of Code](https://summerofcode.withgoogle.com/) projects are at
  [https://docs.jboss.org/display/GSOC/Google+Summer+of+Code+2021+Ideas](https://docs.jboss.org/display/GSOC/Google+Summer+of+Code+2021+Ideas)

---

## Project Proposals

The following projects are offered to students for summer 2022.

'Specialist skills' identify advanced topics likely to be of relevance to the project. These may be things you wish to demonstrate you already have, making you a more attractive candidate for the project, or things you wish to learn, making the project more attractive to you.

### io_uring for JMS

The recently added io_uring interface to the linux kernel provides for scalable, high performance, asynchronous I/O operations.
The performance of Java based messaging systems can potentially benefit from this new API. 

In this project you will evaluate the use of io_uring from Java (via JNI) to provide
enhanced persistent messaging performance in
[Apache ActiveMQ Artemis](https://activemq.apache.org/components/artemis/).

Specialist skills: Messaging systems, JNI.

Reading: 
[What is io_uring?](https://unixism.net/loti/what_is_io_uring.html) ;
[Efficient IO with io_uring](https://kernel.dk/io_uring.pdf) ;
Netty transport
[blog](https://netty.io/news/2020/11/16/io_uring-0-0-1-Final.html) and
[src](https://github.com/netty/netty-incubator-transport-io_uring)

### WebAssembly Java integration

WebAssembly is a binary instruction format for a virtual machine, providing a portable compilation target for several languages.
Embedded in many web browsers, it interoperates well with JavaScript. Interoperability with other languages, including Java, is as yet more limited.

In this project you will investigate and enhance the integration of WebAssembly and JVM languages, with particular attention to allowing calls between them, in either or both directions.

Specialist skills: low level (assembly) programming, virtual machines.

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

Specialist skills: virtual machine architectures, build systems. A prior background in history, anthropology, archaeology or librarianship may also be beneficial.

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

Note: For this project, the code provided with the candidate's application MUST take the form of an original bot for playing a code game such as those linked below. Any programming language may be used.

Specialist skills: game design, technical recruitment, middleware skills training.

Reading:
[codingame](https://www.codingame.com/) ;
[battlesnake](https://play.battlesnake.com/) ;
[Halite](https://halite.io/) ;
[battlecode](https://battlecode.org/) ;
[microcorruption](https://microcorruption.com/login)

### Effectiveness of rebalancing a Kafka cluster

Apache Kafka is a distributed messaging platform capable of very high performance and horizontally scalable. In Kafka, messages are stored in Topics which are replicated and distributed across the Brokers which form the cluster. In a balanced cluster the Topics are evenly distributed amongst the Brokers. However, in practice, clusters become unbalanced due to either poor design, unpredictable workloads or the addition/removal of Brokers.

Tools exist to rebalance a Kafka cluster by either switching which Topic replica is the master, or by moving replicas to under-utilised Brokers. This latter operation can be expensive and take hours to migrate data from one Broker to another. During this time the cluster will be operating at reduced capacity because I/O and network bandwidth is being taken up with the rebalance.

In this project you will use Kafka running on Kubernetes to investigate two things. Firstly, what are the optimal (or good) values for tuning a rebalance to trade off speed vs impact. Secondly, and a stretch goal is to investigate the impact of a rebalance on a running cluster. For instance, how long will it take? Will the existing workload be affected? What are the financial implications if certain data transfers are charged for and others not?

Specialist skills: distrubuted systems, performance modelling.

Reading: [Kafka - The Definitive Guide](https://github.com/jitendra3109/ApacheKafka/blob/master/Docs/confluent-kafka-definitive-guide-complete.pdf); 
[Cruise Control introduction](https://www.youtube.com/watch?v=lf31udm9cYY);
[Strimzi - Running Kafka on Kubernetes](https://strimzi.io/)


### Project Panama evaluation

OpenJDK's [Project Panama](https://jdk.java.net/panama/) foreign function support offers a new approach to calling native libraries from Java. Existing integrations across a number of Red Hat projects use the older [JNI](https://docs.oracle.com/en/java/javase/17/docs/specs/jni/index.html) solution for this requirement.
As native libraries are used to increase scalability or accelerate performance critical code at the cost of more complex build processes, the choice of integration approach is of material interest to us and any opportunity for improvement is attractive.

In this project you will identify and evaluate opportunities for replacing JNI with panama across Red Hat's portfolio of open source projects, prototyping and benchmarking one or more solutions and reporting on issues found.

Specialist skills: C programming, micro benchmarking, build systems.


### eBPF for Java application observability

Observability and monitoring are key to operating reliable, performant cloud services. Red Hat's vertical integration across the operating system (RHEL), container platform (OpenShift), runtime (OpenJDK) and framework (Quarkus, Wildfly) provide us a wide-ranging opportunity for powerfully integrated, holistic solutions in this area.

Horizontally stratified tools e.g. [jfr](https://developers.redhat.com/blog/2020/08/25/get-started-with-jdk-flight-recorder-in-openjdk-8u#about_jdk_flight_recorder), whilst useful, may provide a narrower view compared to approaches that unify data from different layers of the stack. With this in mind, OpenJDK also contains instrumentation for integrating with [eBPF](https://ebpf.io/), an efficient in-kernel tracing solution with overhead low enough for production use.

In this project you will evaluate the opportunities that exist for using eBPF in relation to observability of cloud-native Java microservices.

Specialist skills: DevOps, performance engineering, cloud microservices.


### Bufferbloat in reactive microservices

Networked applications are known to suffer increased latency and jitter due to [bufferbloat](https://en.wikipedia.org/wiki/Bufferbloat), the excess buffering of data packets in network devices.

Reactive applications such as those built with [Quarkus](https://quarkus.io/guides/getting-started-reactive) have an event-driven queue and service architecture that broadly resembles a network architecture, with events or messages replacing TCP/IP packets. Whilst non-blocking execution is the initial focus of performance work for reactive code, this ignores the subtle, low-level details of how messages are buffered inside the libraries.

In the same way that TCP/IP's default sliding window algorithm is insufficient to fully address performance issues arising from bufferbloat, so too it may be that simple backpressue mechanisms are insufficient to maximise performance for reactive microservices. Additionally, large buffers can increase memory footprint, requiring larger, more expensive containers to be used in cloud deployments.

In this project you will investigate the internals of reactive libraries, develop benchmarks and testing methods to examine and tune message buffer sizes, timeouts and other default settings and policies at various levels of the stack, assessing the impact of these on application footprint and performance.

Specialist skills: reactive application architecture, performance engineering.


### Low-code reactive applications

Low-code platforms such as [appsmith](https://www.appsmith.com/) aim to increase developer productivity through visual tooling and code generation techniques. However, many such platforms continue to generate older style applications which ignore the many benefits of [reactive](https://www.reactivemanifesto.org/) application architecture.

[Quarkus](https://quarkus.io/about/) is a framework for Java microservices, with full support for reactive apps and a strong focus on developer joy and efficient tooling. However, whilst it makes writing code a fast, fun experience, it does still require that code to be written largely by hand.

Bringing together low-code tooling and Quarkus has the potential to further enhance developer productivity by automating more of the routine coding required for many applications, whilst simultaneously improving runtime efficiency through use of a reactive approach.

In this project you will explore the opportunities for new tools and frameworks to extend Quarkus with greater low-code application development capabilities.

Specialist skills: reactive applications, code generation.


### Roll your own project

Internship candidates may also submit proposals of their own devising, in the form of a brief outline of the topic and a clear description of how it aligns with Red Hat's needs.
Topics may be original, or drawn from existing open source project roadmaps and JIRA issues.

---

## Application Procedure

Select one preferred project and optionally one reserve choice from the list above.
Send us your choices, along with a CV and some source code that you think demonstrates your software engineering skills well.
This should be in Java, unless the project topic specifically calls for another language.
The topic choices will be used to route your application to the relevant supervisor(s),
who will review your application and may then invite you to a technical interview.

New proposals may be added to this page until mid February.
In such case, earlier applicants may change their project preference to one of the new topics.

We like: links to github repos; originality; documentation; unit tests.  
We don't like: cover letters; code that doesn't compile; tests that fail.

For summer 2022 we expect to be operating entirely online, with interviews and subsequent project supervision taking place without physical contact.
Depending on circumstances, there may also be the option of working from our Newcastle office.

Deadline for applications: 12 noon, Monday 21st February, 2022.
