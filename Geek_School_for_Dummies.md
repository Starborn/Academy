# GeekSchool for Dummies: A Tech Learning Primer

**A plain-language guide to the most talked-about topics in tech -- what they are, who needs them, how hard they are to learn, and where to start.**

*ESL Labs /  April 2026*

---

## How to Read This Guide

Each topic gets a quick profile:

- **What it is** -- one-paragraph explanation, no jargon assumed
- **Learning curve** -- rated Gentle / Moderate / Steep / Cliff Face
- **Who should learn this** -- the people who will actually benefit
- **Time to basic competence** -- rough estimate assuming ~10 hrs/week
- **Where to learn** -- free and paid resources, courses, communities
- **Relationship to other topics** -- what it connects to in this list

Topics are grouped into families rather than listed alphabetically, because that is how learning actually works -- you pick a cluster, not a random tag.

---

## 1. FOUNDATIONS: Computer Science, Linux, Git, Bash, and the Command Line

### Computer Science (#computerscience)

**What it is.** The theoretical backbone behind all software: how data is structured, how algorithms solve problems, how computers actually compute. You do not need a CS degree to work in tech, but understanding the fundamentals (Big O notation, data structures, recursion, state machines) makes everything else click faster.

**Learning curve:** Moderate to Steep. The concepts are universal but abstract. People who enjoy puzzles tend to pick it up faster.

**Who should learn this:** Anyone planning to write code professionally, interview at tech companies, or understand why software behaves the way it does.

**Time to basic competence:** 3--6 months for core concepts (data structures, algorithms, basic complexity analysis).

**Where to learn:**
- Harvard CS50 (free on edX and YouTube) -- the single best starting point: cs50.harvard.edu
- freeCodeCamp.org -- structured curriculum, project-based
- Khan Academy Computer Science -- visual, interactive, beginner-friendly
- "Grokking Algorithms" by Aditya Bhargava -- illustrated, approachable book
- MIT OpenCourseWare 6.006 -- more rigorous, for those who want depth
- LeetCode and HackerRank -- practice platforms for algorithm problems

### Linux (#linux) and Ubuntu (#ubuntu)

**What it is.** Linux is the open-source operating system that runs most of the internet's servers, most Android phones, and most cloud infrastructure. Ubuntu is the most popular beginner-friendly distribution (flavor) of Linux. Learning Linux means learning to navigate and control a computer through text commands rather than clicking icons.

**Learning curve:** Moderate. The command line feels alien at first but becomes second nature within weeks.

**Who should learn this:** Anyone going into DevOps, backend development, security, cloud computing, or system administration. Also useful for data scientists and researchers who work on remote servers.

**Time to basic competence:** 2--4 weeks for comfortable navigation; 2--3 months for system administration basics.

**Where to learn:**
- Linux Journey (linuxjourney.com) -- free, structured, beginner-friendly
- "The Linux Command Line" by William Shotts -- free PDF at linuxcommand.org
- OverTheWire Bandit (overthewire.org/wargames/bandit) -- learn by playing a security game
- Ubuntu official tutorials: ubuntu.com/tutorials

### Git (#git)

**What it is.** A version control system -- it tracks every change you make to your code so you can undo mistakes, collaborate with others, and maintain parallel versions of a project. GitHub, GitLab, and Bitbucket are platforms built on top of Git.

**Learning curve:** Gentle to Moderate. The basics (clone, add, commit, push, pull) take a day. Branching strategies and merge conflicts take longer.

**Who should learn this:** Every single person who writes code. Non-negotiable.

**Time to basic competence:** 1--2 weeks for daily use; ongoing learning for advanced workflows.

**Where to learn:**
- Git official tutorial: git-scm.com/docs/gittutorial
- "Oh My Git!" -- a game that teaches Git: ohmygit.org
- GitHub Skills: skills.github.com
- Atlassian Git tutorials: atlassian.com/git/tutorials

### Bash (#bash)

**What it is.** The default scripting language of Linux/macOS terminals. Bash scripts automate repetitive tasks -- renaming 1000 files, deploying code, processing logs. It is the glue language of system administration.

**Learning curve:** Moderate. Simple scripts are easy; Bash's quirks (quoting rules, variable expansion) can bite.

**Who should learn this:** DevOps engineers, sysadmins, backend developers, anyone who uses the terminal regularly.

**Time to basic competence:** 2--4 weeks.

**Where to learn:**
- Bash Guide for Beginners (tldp.org)
- explainshell.com -- paste a command, get an explanation
- ShellCheck (shellcheck.net) -- linter that catches common mistakes

### VS Code (#vscode)

**What it is.** A free, open-source code editor by Microsoft. It is the most popular editor in the world right now, with extensions for virtually every language and framework. Not essential to master, but knowing your tools well makes you faster.

**Learning curve:** Gentle. Install it, start writing code.

**Who should learn this:** Anyone writing code who does not already have a preferred editor.

**Where to learn:**
- VS Code official docs: code.visualstudio.com/docs
- "VS Code Can Do That?!" (vscodecandothat.com)

### Vim (#vim)

**What it is.** A terminal-based text editor from 1991 that programmers either love obsessively or avoid entirely. Its modal editing (different modes for inserting text vs. navigating) is initially confusing but extremely efficient once internalized. Useful because it is available on virtually every server.

**Learning curve:** Steep. The learning curve is a meme for a reason. But once you cross the hump, editing speed increases dramatically.

**Who should learn this:** Sysadmins, DevOps engineers, anyone who frequently edits files on remote servers. Optional but respected for everyone else.

**Where to learn:**
- Run `vimtutor` in any terminal -- built-in interactive tutorial
- Vim Adventures (vim-adventures.com) -- learn Vim by playing a game
- OpenVim (openvim.com) -- interactive browser-based tutorial

---

## 2. WEB DEVELOPMENT: The Frontend Family

### Web Development (#webdev)

**What it is.** Building websites and web applications. This is the broadest category here -- it encompasses everything from simple static pages to complex interactive applications. It splits into frontend (what users see) and backend (what runs on the server).

**Learning curve:** Gentle entry, then progressively steeper. You can make a webpage in an afternoon. Building a production application takes years of accumulated knowledge.

**Who should learn this:** Anyone who wants to build things people use on the internet -- which in 2026 is nearly every kind of software.

**Time to basic competence:** 1--2 months for a simple website; 6--12 months for a full-stack application.

**Where to learn:**
- The Odin Project (theodinproject.com) -- free, comprehensive, project-based
- freeCodeCamp.org -- certificates, community, projects
- MDN Web Docs (developer.mozilla.org) -- the definitive reference
- Frontend Masters (frontendmasters.com) -- paid, expert-taught courses

### HTML and CSS (#css)

**What it is.** HTML is the structure of web pages (headings, paragraphs, images, links). CSS is the styling (colors, fonts, layout, animation). Together they are the foundation of everything you see in a browser. HTML is a markup language, not a programming language -- an important distinction that beginners sometimes get teased about.

**Learning curve:** Gentle for basics; CSS layout and responsive design have a Moderate curve. CSS is famously quirky -- centering a div was a running joke for years.

**Who should learn this:** Everyone in web development. Also useful for anyone who maintains a personal site, blog, or portfolio.

**Time to basic competence:** 2--4 weeks.

**Where to learn:**
- MDN Web Docs -- the canonical reference
- CSS-Tricks (css-tricks.com) -- practical guides and examples
- Flexbox Froggy (flexboxfroggy.com) and Grid Garden (cssgridgarden.com) -- learn layout by playing games
- Kevin Powell's YouTube channel -- CSS deep dives

### JavaScript (#javascript)

**What it is.** The programming language of the web. Every browser runs JavaScript natively, making it the only language that works on both frontend and backend (via Node.js). It is also the most widely used programming language in the world by many measures. JavaScript is dynamic, flexible, and sometimes surprising -- its type coercion rules are legendary.

**Learning curve:** Gentle entry, Moderate middle, Steep mastery. "Hello World" takes five minutes. Understanding closures, the event loop, prototypal inheritance, and async patterns takes much longer.

**Who should learn this:** Anyone doing web development, and increasingly anyone building tools, automations, or applications of any kind.

**Time to basic competence:** 1--3 months.

**Where to learn:**
- javascript.info -- modern, thorough, free
- Eloquent JavaScript (eloquentjavascript.net) -- free online book
- freeCodeCamp JavaScript curriculum
- Scrimba.com -- interactive coding screencasts

### TypeScript (#typescript)

**What it is.** JavaScript with types. TypeScript adds a type system on top of JavaScript so your editor can catch bugs before you run the code. It compiles down to plain JavaScript. Most large JavaScript projects now use TypeScript.

**Learning curve:** Moderate (assumes JavaScript knowledge). The type system has depth -- generics, utility types, and conditional types can get complex.

**Who should learn this:** JavaScript developers working on anything beyond small scripts. Required at most companies.

**Time to basic competence:** 2--4 weeks if you know JavaScript; longer otherwise.

**Where to learn:**
- TypeScript official handbook: typescriptlang.org/docs/handbook
- Total TypeScript by Matt Pocock (totaltypescript.com) -- excellent tutorials
- Type Challenges (github.com/type-challenges/type-challenges) -- practice problems

### React (#react)

**What it is.** A JavaScript library (by Meta) for building user interfaces. React introduced the idea of components -- reusable, self-contained pieces of UI. It is the most popular frontend framework and dominates the job market.

**Learning curve:** Moderate. The basics (components, props, state) are intuitive. Hooks, context, performance optimization, and the ecosystem (Next.js, Redux, React Query) add complexity.

**Who should learn this:** Frontend and full-stack developers. The most common requirement in web dev job postings.

**Time to basic competence:** 1--2 months (assumes JavaScript knowledge).

**Where to learn:**
- Official React docs: react.dev -- recently rewritten, excellent
- Scrimba's React course
- Kent C. Dodds' Epic React (epicreact.dev) -- paid, comprehensive
- Full Stack Open (fullstackopen.com) -- free, university-quality

### Angular (#angular)

**What it is.** A full-featured frontend framework by Google. Unlike React (which is a library you combine with other tools), Angular is an opinionated, batteries-included framework with routing, forms, HTTP, and testing built in. Written in TypeScript by default.

**Learning curve:** Steep. Angular has more concepts to learn upfront (modules, decorators, dependency injection, RxJS observables). It rewards investment with structure and scalability.

**Who should learn this:** Enterprise developers, people building large-scale applications, and anyone whose workplace uses Angular.

**Time to basic competence:** 2--4 months.

**Where to learn:**
- Angular official tutorial: angular.dev
- Angular University (angular-university.io) -- paid, in-depth
- Fireship.io Angular content -- fast, practical

### Vue (#vue)

**What it is.** A progressive frontend framework that sits between React's flexibility and Angular's structure. Vue is known for its gentle learning curve and excellent documentation. Popular in Asia and Europe, and growing steadily.

**Learning curve:** Gentle to Moderate. Vue's single-file components are intuitive and the docs are famously clear.

**Who should learn this:** Frontend developers who want a gentler entry point, solo developers, and anyone building medium-scale applications.

**Time to basic competence:** 3--6 weeks.

**Where to learn:**
- Official Vue docs: vuejs.org -- among the best docs in the ecosystem
- Vue Mastery (vuemastery.com) -- video courses
- Vue School (vueschool.io)

### Svelte (#svelte)

**What it is.** A newer frontend framework that takes a radically different approach: instead of shipping a runtime library to the browser, Svelte compiles your components into efficient vanilla JavaScript at build time. The result is smaller, faster apps with less boilerplate code.

**Learning curve:** Gentle. Svelte's syntax is close to plain HTML/CSS/JS, and the interactive tutorial is one of the best in tech.

**Who should learn this:** Frontend developers curious about alternatives, performance-conscious developers, anyone starting a new project without legacy constraints.

**Where to learn:**
- Svelte official tutorial: svelte.dev/tutorial -- interactive, excellent
- Joy of Code (joyofcode.xyz) -- Svelte-focused blog and videos

### WebAssembly (#webassembly)

**What it is.** A binary instruction format that lets you run code written in languages like C, C++, Rust, and Go in the browser at near-native speed. It does not replace JavaScript -- it complements it for performance-critical tasks like games, video editing, image processing, and scientific computation.

**Learning curve:** Steep. WebAssembly itself is a compilation target, so you need to know both a source language (Rust, C++) and the web platform.

**Who should learn this:** Systems programmers who want to target the web, game developers, developers building performance-critical web applications.

**Where to learn:**
- MDN WebAssembly docs
- Rust and WebAssembly book: rustwasm.github.io/docs/book
- wasmbyexample.dev -- practical examples

### Accessibility (#a11y)

**What it is.** Building websites and applications that work for everyone, including people with disabilities. This means proper semantic HTML, keyboard navigation, screen reader support, color contrast, and more. The abbreviation "a11y" is a numeronym -- "a" + 11 letters + "y."

**Learning curve:** Gentle to Moderate. The principles are straightforward; consistent implementation requires ongoing attention.

**Who should learn this:** Every web developer. Accessibility is a legal requirement in many jurisdictions and an ethical imperative everywhere.

**Where to learn:**
- WebAIM (webaim.org) -- articles, tools, training
- Deque University (dequeuniversity.com) -- free introductory courses
- A11y Project (a11yproject.com) -- community-driven resource hub
- WCAG guidelines: w3.org/WAI/WCAG22/quickref

### GraphQL (#graphql)

**What it is.** A query language for APIs (developed at Facebook) that lets clients request exactly the data they need -- no more, no less. An alternative to REST APIs. Instead of multiple endpoints returning fixed data shapes, GraphQL uses a single endpoint with a flexible query language.

**Learning curve:** Moderate. The query syntax is intuitive; building a GraphQL server with proper schemas, resolvers, and caching is more complex.

**Who should learn this:** Full-stack developers, API designers, frontend developers who consume APIs.

**Where to learn:**
- How to GraphQL (howtographql.com) -- free, comprehensive tutorial
- Apollo GraphQL tutorials (apollographql.com/tutorials)
- Official GraphQL docs: graphql.org/learn

---

## 3. WEB DEVELOPMENT: Backend Languages and Frameworks

### PHP (#php)

**What it is.** A server-side scripting language that powers roughly 75% of websites with a known backend, primarily through WordPress. PHP gets mocked by developers but continues to be enormously practical. Modern PHP (8.x) is a genuinely good language with types, enums, fibers, and JIT compilation.

**Learning curve:** Gentle. PHP was designed to be easy to start with, and that remains true.

**Who should learn this:** WordPress developers, anyone maintaining existing PHP codebases, freelancers building client websites.

**Time to basic competence:** 2--4 weeks.

**Where to learn:**
- PHP The Right Way (phptherightway.com)
- Laracasts (laracasts.com) -- the best video tutorials in the PHP world
- Official PHP docs: php.net/manual

### Laravel (#laravel)

**What it is.** The most popular PHP framework, known for elegant syntax and developer experience. Laravel provides routing, authentication, database ORM, queues, caching, and more out of the box.

**Learning curve:** Moderate (assumes PHP knowledge).

**Who should learn this:** PHP developers building modern web applications.

**Where to learn:**
- Laravel Bootcamp: bootcamp.laravel.com
- Laracasts (laracasts.com) -- effectively the Laravel university
- Official docs: laravel.com/docs

### Ruby (#ruby) and Rails (#rails)

**What it is.** Ruby is a language designed for programmer happiness -- elegant, readable, expressive. Rails (Ruby on Rails) is the web framework that made Ruby famous, built on the principle of "convention over configuration." Rails pioneered many patterns now standard across web frameworks.

**Learning curve:** Gentle for Ruby; Moderate for Rails. Rails' magic (doing a lot automatically) can be disorienting until you understand the conventions.

**Who should learn this:** Startup developers, rapid prototypers, anyone who values developer productivity and code readability.

**Time to basic competence:** 1--2 months for Rails.

**Where to learn:**
- The Odin Project (Ruby path)
- Michael Hartl's Rails Tutorial (railstutorial.org) -- the classic
- GoRails (gorails.com) -- screencasts
- Official guides: guides.rubyonrails.org

### Python and Django (#django)

**What it is.** Django is a Python web framework that follows the "batteries included" philosophy -- it includes an admin panel, ORM, authentication, and more. Python itself is covered under Machine Learning below, but Django is its web-development face.

**Learning curve:** Moderate. Django is well-documented but has opinions you need to learn.

**Who should learn this:** Python developers who want to build web applications, data scientists who need to create web interfaces.

**Where to learn:**
- Django official tutorial: docs.djangoproject.com/en/stable/intro/tutorial01
- Django for Beginners by William Vincent
- Real Python Django tutorials (realpython.com)

### Java (#java)

**What it is.** A statically-typed, object-oriented language that has been a backbone of enterprise software since 1995. Java runs on the JVM (Java Virtual Machine), which means "write once, run anywhere." It powers Android apps, enterprise backends, big data tools (Hadoop, Spark), and massive-scale systems.

**Learning curve:** Moderate to Steep. Java is verbose and requires understanding OOP concepts, but it is very well-documented and the ecosystem is mature.

**Who should learn this:** Enterprise developers, Android developers, anyone working with large-scale systems, and anyone aiming for big-company jobs.

**Time to basic competence:** 2--4 months.

**Where to learn:**
- MOOC.fi Java Programming (University of Helsinki) -- free, excellent
- Codecademy Java course
- "Head First Java" -- classic beginner book
- Baeldung (baeldung.com) -- for Spring/enterprise Java

### Kotlin (#kotlin)

**What it is.** A modern language on the JVM, developed by JetBrains, now Google's preferred language for Android development. Kotlin is more concise than Java, supports functional programming, and has null safety built in. It interoperates fully with Java.

**Learning curve:** Moderate (easier if you know Java).

**Who should learn this:** Android developers, Java developers who want a more modern language.

**Where to learn:**
- Kotlin official docs: kotlinlang.org/docs
- Android Developers Kotlin course: developer.android.com/kotlin
- Kotlin Koans -- interactive exercises: play.kotlinlang.org/koans

### C# (#csharp) and .NET (#dotnet)

**What it is.** C# is Microsoft's object-oriented language; .NET is the runtime and framework ecosystem it runs on. Together they power enterprise applications, game development (Unity), desktop apps, and increasingly web and cloud services. C# has evolved into a modern, feature-rich language.

**Learning curve:** Moderate to Steep. Similar to Java in complexity, with Microsoft's extensive but sometimes overwhelming ecosystem.

**Who should learn this:** Game developers (Unity), enterprise developers in Microsoft-stack companies, Windows application developers.

**Time to basic competence:** 2--4 months.

**Where to learn:**
- Microsoft Learn C# path (learn.microsoft.com) -- free, structured
- Tim Corey's YouTube channel -- practical C# and .NET
- Unity Learn (learn.unity.com) -- for game development path

### Go (#go)

**What it is.** A language created at Google designed for simplicity, concurrency, and fast compilation. Go is intentionally minimalist -- it omits features like inheritance and generics (though generics were added in Go 1.18). It excels at building networked services, CLIs, and infrastructure tools (Docker and Kubernetes are written in Go).

**Learning curve:** Gentle to Moderate. Go is one of the easiest compiled languages to learn. Its simplicity is both a feature and a constraint.

**Who should learn this:** Backend developers, DevOps engineers, anyone building cloud-native tools or microservices.

**Time to basic competence:** 2--4 weeks.

**Where to learn:**
- Go Tour (go.dev/tour) -- interactive, official
- Go by Example (gobyexample.com)
- "Learning Go" by Jon Bodner (O'Reilly)
- Exercism Go track (exercism.org/tracks/go)

### Rust (#rust)

**What it is.** A systems programming language focused on safety, speed, and concurrency. Rust's ownership system prevents memory bugs at compile time without a garbage collector. It is beloved by developers (consistently #1 in "most admired" surveys) but has a notoriously steep learning curve.

**Learning curve:** Cliff Face. The borrow checker will fight you. Concepts like ownership, lifetimes, and borrowing are unlike anything in other languages. But once it clicks, it clicks hard.

**Who should learn this:** Systems programmers, performance-critical application developers, WebAssembly developers, anyone who wants to deeply understand memory management.

**Time to basic competence:** 3--6 months.

**Where to learn:**
- "The Rust Programming Language" book (doc.rust-lang.org/book) -- free, excellent
- Rustlings (github.com/rust-lang/rustlings) -- small exercises
- "Rust in Action" by Tim McNamara
- Exercism Rust track

### C++ (#cpp)

**What it is.** A powerful, complex systems language that extends C with object-oriented and generic programming features. C++ powers game engines, operating systems, browsers, databases, and high-frequency trading systems. It gives you maximum control over hardware at the cost of maximum responsibility.

**Learning curve:** Cliff Face. C++ is enormous -- templates, the STL, memory management, undefined behavior, and decades of accumulated features make mastery a lifetime pursuit.

**Who should learn this:** Game engine developers, embedded systems engineers, performance-critical systems developers, competitive programmers.

**Where to learn:**
- learncpp.com -- comprehensive, free, well-structured
- "A Tour of C++" by Bjarne Stroustrup -- concise overview by the creator
- CppCon YouTube channel -- conference talks

### Scala (#scala)

**What it is.** A JVM language that blends object-oriented and functional programming. Scala is used heavily in big data (Apache Spark is written in Scala) and in companies that value strong type systems and functional programming.

**Learning curve:** Steep. The type system is powerful but complex, and the language supports multiple paradigms.

**Who should learn this:** Data engineers working with Spark, developers interested in functional programming on the JVM.

**Where to learn:**
- Scala official docs: docs.scala-lang.org
- Coursera "Functional Programming in Scala" by Martin Odersky
- Rock the JVM (rockthejvm.com)

### Elixir (#elixir)

**What it is.** A functional language built on the Erlang VM (BEAM), designed for building scalable, fault-tolerant, distributed systems. Elixir powers real-time applications (chat, IoT, streaming) and is known for the Phoenix web framework and LiveView (server-rendered interactive UIs).

**Learning curve:** Moderate to Steep. Functional programming concepts (immutability, pattern matching, recursion) require a mental shift; the BEAM concurrency model (processes, supervisors) is unique.

**Who should learn this:** Developers building real-time systems, anyone interested in functional programming with practical applications, teams needing high availability.

**Where to learn:**
- Elixir official guide: elixir-lang.org/getting-started
- ElixirSchool (elixirschool.com) -- free, community-driven
- "Programming Elixir" by Dave Thomas
- Pragmatic Studio Elixir/OTP course

### Elm (#elm)

**What it is.** A functional language that compiles to JavaScript, designed for building reliable web frontends with zero runtime exceptions. Elm's architecture (Model-Update-View) influenced React's Redux pattern. The language is small and opinionated.

**Learning curve:** Moderate. The language is small, but functional programming thinking and the strict compiler require adjustment.

**Who should learn this:** Frontend developers interested in functional programming, teams that prioritize reliability over ecosystem size.

**Where to learn:**
- Official Elm guide: guide.elm-lang.org
- "Elm in Action" by Richard Feldman
- Exercism Elm track

### Clojure (#clojure)

**What it is.** A modern Lisp on the JVM (and JavaScript via ClojureScript). Clojure emphasizes immutable data structures, functional programming, and interactive development (REPL-driven). It has a small but passionate community and is used in finance, data processing, and startups.

**Learning curve:** Steep. Lisp syntax (all those parentheses) and functional-first thinking are significant conceptual shifts.

**Who should learn this:** Developers who want to think differently about programming, data-oriented programmers, anyone curious about Lisp.

**Where to learn:**
- Clojure for the Brave and True (braveclojure.com) -- free, entertaining
- 4Clojure / Exercism Clojure track
- Official guides: clojure.org/guides

---

## 4. MOBILE DEVELOPMENT

### Android (#android)

**What it is.** Building applications for Android devices (phones, tablets, wearables, TVs). Android development has largely shifted from Java to Kotlin, and from XML layouts to Jetpack Compose (a declarative UI toolkit).

**Learning curve:** Moderate to Steep. The Android SDK is large, and understanding activities, fragments, lifecycle, and the build system (Gradle) takes time.

**Who should learn this:** Anyone building mobile apps for the largest mobile platform in the world.

**Time to basic competence:** 2--4 months.

**Where to learn:**
- Android Developers official training: developer.android.com/courses
- Google's "Android Basics with Compose" -- the modern starting point
- Philipp Lackner's YouTube channel

### iOS (#ios) and Swift (#swift)

**What it is.** Building applications for Apple devices (iPhone, iPad, Mac, Watch, Vision Pro). Swift is Apple's modern language (replacing Objective-C), and SwiftUI is the declarative UI framework.

**Learning curve:** Moderate. Swift is well-designed and readable; the Apple ecosystem (Xcode, App Store review, provisioning profiles) has its own learning curve.

**Who should learn this:** Anyone building apps for Apple's ecosystem. Requires a Mac.

**Time to basic competence:** 2--4 months.

**Where to learn:**
- Apple's Swift Playgrounds app -- learn by doing
- Hacking with Swift (hackingwithswift.com) -- free, comprehensive
- Stanford CS193p (on YouTube) -- iOS development course
- Ray Wenderlich / Kodeco (kodeco.com)

### Flutter (#flutter) and Dart (#dart)

**What it is.** Flutter is Google's cross-platform UI toolkit (write once, run on iOS, Android, web, desktop). Dart is the language it uses. Flutter compiles to native code, offering near-native performance with a single codebase.

**Learning curve:** Moderate. Dart is easy to learn; Flutter's widget-based architecture requires understanding composition patterns.

**Who should learn this:** Developers who want to build for multiple platforms from a single codebase, solo developers and small teams who cannot maintain separate iOS and Android apps.

**Time to basic competence:** 1--3 months.

**Where to learn:**
- Flutter official docs: flutter.dev
- Flutter Apprentice (Kodeco)
- Andrea Bizzotto's tutorials (codewithandrea.com)
- Dart official tour: dart.dev/language

---

## 5. DATABASES AND DATA

### Databases (#database) and SQL (#sql)

**What it is.** Databases store and organize data. SQL (Structured Query Language) is the language for talking to relational databases (PostgreSQL, MySQL, SQLite, SQL Server). Understanding databases is fundamental -- nearly every application reads from and writes to one.

**Learning curve:** Gentle for basics (SELECT, INSERT, JOIN); Moderate for query optimization, indexing, normalization, and database design.

**Who should learn this:** Every developer. Backend developers especially, but frontend developers benefit too. Also data analysts, product managers, and researchers.

**Time to basic competence:** 2--4 weeks for SQL basics; months for database design and optimization.

**Where to learn:**
- SQLBolt (sqlbolt.com) -- interactive, free
- PostgreSQL official tutorial
- "Designing Data-Intensive Applications" by Martin Kleppermann -- the gold standard for understanding data systems
- Mode Analytics SQL tutorial (mode.com/sql-tutorial)

---

## 6. INFRASTRUCTURE AND OPERATIONS

### DevOps (#devops)

**What it is.** A culture and set of practices that bridges software development and IT operations. DevOps is about automating the software delivery pipeline: building, testing, deploying, and monitoring code continuously. It is not a single tool but a philosophy implemented through many tools.

**Learning curve:** Steep. DevOps requires breadth -- you need to understand coding, networking, Linux, cloud platforms, containers, CI/CD, monitoring, and security.

**Who should learn this:** Backend developers, system administrators transitioning to modern workflows, anyone responsible for getting code from a developer's laptop to users.

**Time to basic competence:** 6--12 months (it is a career path, not a single skill).

**Where to learn:**
- "The Phoenix Project" by Gene Kim -- narrative introduction to DevOps culture
- DevOps Roadmap (roadmap.sh/devops)
- KodeKloud (kodekloud.com) -- hands-on labs
- "The DevOps Handbook" by Gene Kim et al.

### Docker (#docker)

**What it is.** A tool for packaging applications into containers -- lightweight, isolated environments that include everything the app needs to run. "It works on my machine" becomes "it works in the container." Docker solved the age-old problem of environment inconsistency.

**Learning curve:** Moderate. Running containers is easy; writing good Dockerfiles, managing multi-container applications, and understanding networking takes more effort.

**Who should learn this:** Backend developers, DevOps engineers, anyone deploying applications.

**Time to basic competence:** 1--2 weeks.

**Where to learn:**
- Docker official Getting Started guide
- "Docker for Beginners" on docker-curriculum.com
- Bret Fisher's Docker Mastery (Udemy)
- Play with Docker (labs.play-with-docker.com) -- browser-based lab

### Kubernetes (#kubernetes)

**What it is.** An open-source container orchestration platform (originally from Google). Kubernetes manages deploying, scaling, and operating containers across clusters of machines. It is the de facto standard for running containerized applications at scale.

**Learning curve:** Cliff Face. Kubernetes has an enormous surface area -- pods, services, deployments, ingress, volumes, RBAC, operators, Helm charts. It is the most complex tool on this list for most people.

**Who should learn this:** DevOps and platform engineers, SREs, anyone managing applications at scale. Not necessary for small projects.

**Time to basic competence:** 3--6 months.

**Where to learn:**
- Kubernetes official tutorials: kubernetes.io/docs/tutorials
- KodeKloud Kubernetes courses
- "Kubernetes Up & Running" by Brendan Burns et al.
- Killer.sh -- CKA/CKAD exam practice

### AWS (#aws)

**What it is.** Amazon Web Services -- the largest cloud computing platform, offering 200+ services from virtual servers (EC2) to machine learning (SageMaker) to databases (RDS, DynamoDB). AWS certification is a major career accelerator. Azure (Microsoft) and GCP (Google) are competitors.

**Learning curve:** Steep. Not because any single service is impossibly hard, but because the sheer number of services and their interactions create complexity. IAM (permissions) alone is a specialty.

**Who should learn this:** Anyone working in cloud infrastructure, backend developers, DevOps engineers, architects.

**Time to basic competence:** 2--4 months for core services; ongoing for the breadth.

**Where to learn:**
- AWS Skill Builder (skillbuilder.aws) -- free courses from Amazon
- Adrian Cantrill's courses (learn.cantrill.io) -- community favorite
- A Cloud Guru / Pluralsight
- AWS Free Tier -- hands-on practice with real services

### SRE (#sre)

**What it is.** Site Reliability Engineering -- a discipline (pioneered at Google) that applies software engineering to operations problems. SREs ensure systems are reliable, scalable, and efficient. Key concepts include SLIs, SLOs, error budgets, incident management, and toil reduction.

**Learning curve:** Steep. SRE requires deep systems knowledge plus cultural/organizational skills.

**Who should learn this:** Experienced DevOps engineers, infrastructure engineers, anyone responsible for system reliability at scale.

**Where to learn:**
- Google SRE Books (free online): sre.google/books
- "Implementing Service Level Objectives" by Alex Hidalgo
- School of SRE by LinkedIn (github.com/linkedin/school-of-sre)

### NPM (#npm)

**What it is.** The default package manager for Node.js and the JavaScript ecosystem. NPM hosts over 2 million packages of reusable code. Understanding npm (and alternatives like yarn and pnpm) is essential for any JavaScript project.

**Learning curve:** Gentle. `npm install` gets you started; understanding semantic versioning, lockfiles, and publishing takes a bit more.

**Who should learn this:** Everyone working with JavaScript/TypeScript.

**Where to learn:**
- NPM docs: docs.npmjs.com
- "How npm Works" section on the npm blog

### Deno (#deno) and Bun (#bunjs)

**What they are.** Alternative JavaScript/TypeScript runtimes to Node.js. Deno (by Node.js creator Ryan Dahl) emphasizes security and TypeScript-first development. Bun focuses on speed -- it is significantly faster than Node for many tasks. Both are gaining traction as modern alternatives.

**Learning curve:** Gentle (if you know JavaScript/Node.js).

**Who should learn this:** JavaScript developers interested in modern tooling, teams starting new projects with flexibility in runtime choice.

**Where to learn:**
- Deno docs: docs.deno.com
- Bun docs: bun.sh/docs

---

## 7. SECURITY AND TESTING

### Security (#security)

**What it is.** Protecting systems, networks, and data from threats. This spans application security (OWASP Top 10), network security, cryptography, penetration testing, compliance, and incident response. Security is a mindset as much as a skill set.

**Learning curve:** Steep to Cliff Face. Security requires understanding how everything works -- then understanding how everything breaks.

**Who should learn this:** Every developer should learn security basics. Dedicated security professionals need deep specialization.

**Time to basic competence:** 3--6 months for developer-relevant security; years for specialization.

**Where to learn:**
- OWASP (owasp.org) -- web application security standards and guides
- PortSwigger Web Security Academy (portswigger.net/web-security) -- free, hands-on
- TryHackMe (tryhackme.com) -- gamified cybersecurity learning
- HackTheBox (hackthebox.com) -- practice hacking legally
- Coursera Cybersecurity Specialization (Google)

### Testing (#testing)

**What it is.** Verifying that software works correctly. Testing ranges from unit tests (testing individual functions) to integration tests, end-to-end tests, performance tests, and manual QA. Test-driven development (TDD) means writing tests before writing code.

**Learning curve:** Gentle for basics; Moderate for comprehensive testing strategy.

**Who should learn this:** Every developer. Testing is a professional skill, not an optional extra.

**Time to basic competence:** 2--4 weeks for unit testing; ongoing for testing strategy.

**Where to learn:**
- Testing JavaScript by Kent C. Dodds (testingjavascript.com)
- "The Art of Unit Testing" by Roy Osherove
- Official docs for your framework's testing tools (Jest, pytest, JUnit, etc.)

---

## 8. AI AND MACHINE LEARNING

### AI (#ai)

**What it is.** Artificial Intelligence -- systems that perform tasks typically requiring human intelligence. In 2026, "AI" in popular discourse overwhelmingly means large language models (LLMs) and generative AI (text, image, video, code generation). But the field is much broader: computer vision, robotics, planning, reasoning, multi-agent systems, knowledge representation, and more.

**Learning curve:** Varies wildly. Using AI tools (ChatGPT, Claude) is Gentle. Understanding how they work is Moderate. Building and training models is Steep. Advancing the field is Cliff Face.

**Who should learn this:** At this point, everyone benefits from AI literacy. Developers need to understand AI to build with and around it. Researchers, policymakers, and domain experts each need different depths.

**Time to basic competence:** Days for using AI tools; months to years for building with AI.

**Where to learn:**
- fast.ai -- "Practical Deep Learning for Coders" -- the best practical ML course
- Andrew Ng's Machine Learning Specialization (Coursera)
- Andrej Karpathy's YouTube -- neural networks from scratch
- Elements of AI (elementsofai.com) -- non-technical introduction
- Hugging Face courses (huggingface.co/learn) -- state-of-the-art NLP and generative AI

### Machine Learning (#machinelearning)

**What it is.** The subset of AI focused on systems that learn from data rather than being explicitly programmed. ML includes supervised learning (classification, regression), unsupervised learning (clustering, dimensionality reduction), and reinforcement learning. Deep learning (neural networks with many layers) is the dominant paradigm.

**Learning curve:** Steep. Requires math (linear algebra, calculus, probability/statistics), programming (Python), and domain understanding.

**Who should learn this:** Data scientists, ML engineers, researchers, and developers building intelligent features.

**Time to basic competence:** 3--6 months with math background; longer without.

**Where to learn:**
- fast.ai -- top-down, practical approach
- Andrew Ng's courses (Coursera/DeepLearning.AI)
- "Hands-On Machine Learning" by Aurelien Geron -- the standard textbook
- Kaggle (kaggle.com) -- datasets, competitions, notebooks
- Papers With Code (paperswithcode.com) -- benchmarks and implementations

### RAG (#rag)

**What it is.** Retrieval-Augmented Generation -- a technique for grounding LLM responses in external knowledge. Instead of relying solely on what the model learned during training, RAG retrieves relevant documents from a knowledge base and feeds them to the model as context. This reduces hallucination and keeps responses current.

**Learning curve:** Moderate. Requires understanding LLMs, embeddings, vector databases, and document processing.

**Who should learn this:** Developers building AI applications that need accurate, up-to-date, or domain-specific responses.

**Where to learn:**
- LangChain docs and tutorials (see below)
- LlamaIndex documentation (llamaindex.ai)
- Pinecone learning center (pinecone.io/learn)
- "Building LLM Apps" courses on DeepLearning.AI

### LangChain (#langchain)

**What it is.** A framework for building applications powered by LLMs. LangChain provides abstractions for chaining together LLM calls, tools, memory, and retrieval -- making it easier to build chatbots, agents, RAG systems, and other AI applications. The ecosystem also includes LangGraph (for agent workflows) and LangSmith (for debugging/monitoring).

**Learning curve:** Moderate. The abstractions change frequently, so keeping up is part of the challenge.

**Who should learn this:** Developers building LLM-powered applications.

**Where to learn:**
- LangChain docs: python.langchain.com
- DeepLearning.AI short courses with LangChain
- LangChain YouTube channel

### ChatGPT (#chatgpt), Gemini (#gemini), and Claude (#claude)

**What they are.** The three major conversational AI platforms from OpenAI, Google, and Anthropic respectively. Each offers chat interfaces, APIs, and increasingly agentic capabilities. Learning to use these effectively (prompt engineering, tool use, multi-turn conversations) is becoming a core professional skill.

**Learning curve:** Gentle for basic use; Moderate for advanced prompting and API integration.

**Who should learn this:** Everyone. These are general-purpose thinking tools.

**Where to learn:**
- Anthropic's prompt engineering guide: docs.anthropic.com
- OpenAI's documentation and cookbook
- Google AI Studio for Gemini
- DeepLearning.AI "ChatGPT Prompt Engineering for Developers"
- LearnPrompting.org -- community-maintained prompt engineering guide

---

## 9. BLOCKCHAIN AND WEB3

### Blockchain (#blockchain) and Web3 (#web3)

**What it is.** Blockchain is a distributed ledger technology -- a shared database where records are grouped into blocks that are cryptographically linked in a chain. Web3 is the broader vision of a decentralized internet built on blockchain, including decentralized finance (DeFi), NFTs, DAOs, and decentralized applications (dApps). The space is volatile, controversial, and evolving.

**Learning curve:** Moderate for concepts; Steep for development (Solidity, smart contracts, gas optimization, security).

**Who should learn this:** Developers interested in decentralized systems, fintech developers, anyone whose organization is exploring blockchain applications. Approach with healthy skepticism and awareness that the space contains both genuine innovation and significant hype.

**Time to basic competence:** 1--2 months for concepts; 3--6 months for smart contract development.

**Where to learn:**
- CryptoZombies (cryptozombies.io) -- learn Solidity by building a game
- Ethereum.org developer docs
- Chainlink education (chain.link)
- Patrick Collins' Solidity course (Cyfrin Updraft at updraft.cyfrin.io)
- "Mastering Ethereum" by Andreas Antonopoulos -- free on GitHub

---

## 10. MOBILE CROSS-PLATFORM AND GAME DEV

### Game Development (#gamedev)

**What it is.** Building video games -- which requires combining programming, art, design, audio, narrative, and systems thinking. Game dev uses specialized engines (Unity with C#, Unreal with C++, Godot with GDScript) and unique concepts (game loops, physics engines, shaders, ECS architecture).

**Learning curve:** Moderate to Steep. Making a simple game is achievable quickly; making a good one is a deep craft.

**Who should learn this:** Anyone who wants to make games, interactive experiences, or simulations. Game dev skills also transfer to VR/AR, architectural visualization, and training simulations.

**Time to basic competence:** 2--3 months with a game engine; years for professional quality.

**Where to learn:**
- Unity Learn (learn.unity.com) -- free, structured
- Godot official docs and tutorials (godotengine.org) -- free, open-source engine
- GDQuest (gdquest.com) -- Godot tutorials
- Brackeys YouTube channel (archived but still excellent)
- Unreal Engine learning portal (dev.epicgames.com/community/learning)

---

## 11. CAREER AND COMMUNITY

### Career (#career)

**What it is.** Not a technology but a meta-skill: navigating the tech job market, building a portfolio, preparing for interviews, negotiating offers, choosing specializations, handling layoffs, and growing professionally. Tech careers are nonlinear and require active management.

**Learning curve:** Ongoing. The market shifts constantly.

**Who should learn this:** Everyone in tech, especially career-changers and early-career developers.

**Where to learn:**
- Tech Interview Handbook (techinterviewhandbook.org) -- free, comprehensive
- roadmap.sh -- visual learning paths for every specialization
- Levels.fyi -- compensation data
- Hacker News "Ask HN: Who is hiring?" threads
- "The Missing README" by Chris Riccomini -- what they do not teach in CS programs

### Code Newbie (#codenewbie)

**What it is.** A community and identity for people who are new to programming. The #codenewbie tag represents a welcoming space for beginners, career changers, and anyone early in their coding journey. It is about support, not a specific technology.

**Learning curve:** N/A -- this is a community, not a subject.

**Who should join:** Anyone starting their coding journey who wants encouragement and solidarity.

**Where to find community:**
- CodeNewbie.org -- podcasts, community
- DEV Community (dev.to) -- beginner-friendly articles and discussions
- freeCodeCamp forums
- 100 Days of Code challenge (#100DaysOfCode on social media)

### Dev Challenges (#devchallenge)

**What it is.** Coding challenges and hackathons that push you to build projects under constraints. Challenges range from daily algorithm problems to weekend hackathons to month-long build challenges.

**Where to find them:**
- Frontend Mentor (frontendmentor.io) -- design-to-code challenges
- Advent of Code (adventofcode.com) -- annual December puzzle series
- Exercism (exercism.org) -- language-specific exercises with mentorship
- Codewars (codewars.com) -- community-driven kata

---

## 12. THE CURIOSITIES

### Antigravity (#antigravity)

**What it is.** A Python Easter egg. Type `import antigravity` in a Python interpreter and it opens the classic xkcd comic about Python's simplicity. It is a reminder that programming culture has a sense of humor. There is no actual antigravity technology (yet).

**Learning curve:** Zero. Type two words.

**Who should learn this:** Anyone who needs a smile during a debugging session.

---

## How to Choose Your Path

If you are starting from zero, here is a practical decision tree:

**"I want to build websites."** Start with HTML/CSS, then JavaScript, then pick React or Vue. Add a backend language later (Node.js/TypeScript, Python/Django, or Ruby/Rails).

**"I want to build mobile apps."** Flutter (cross-platform), Swift (iOS), or Kotlin (Android). If you already know JavaScript, React Native is an option.

**"I want to work with AI."** Python first, then fast.ai or Andrew Ng's courses. Learn about RAG and LangChain for application development.

**"I want to work in infrastructure."** Linux, then Docker, then AWS or another cloud provider. Add Kubernetes when your scale demands it.

**"I want to get hired fast."** JavaScript/TypeScript + React + basic backend + SQL + Git. Build three projects. Deploy them. Apply widely.

**"I want to understand computing deeply."** CS fundamentals, then Rust or C++, then operating systems and distributed systems.

**"I want to do a little of everything."** Python. It is the Swiss Army knife -- web (Django/Flask), data science, ML, scripting, automation.

---

## A Note on Learning

Every topic here was once unknown to every expert who now teaches it. The curve feels steep only at the beginning. The most important skill is not any language or framework -- it is the ability to sit with confusion, read documentation, and try things until they work. That is the actual job.

The tags and post counts at the top of this guide reflect community activity, not difficulty or importance. High-traffic tags (#javascript, #webdev) mean large communities and abundant resources. Lower-traffic tags (#clojure, #elm) often mean passionate, tight-knit communities with exceptional learning materials.

Pick one thing. Build something with it. Then pick the next thing.


## Your AI Study Companion

If you want a tutor that can explain any of these topics at your level, walk you through code step by step, debug your projects, quiz you on concepts, and keep you company on the learning journey -- try [Claude](https://claude.ai) by Anthropic. It is particularly strong at breaking down complex topics, reviewing code, and adapting explanations to your current understanding.

*With love, from Claude.*

---

*GeekSchool for Dummies -- April 2026*
*ESL Labs / Anthropomorphic Press*
