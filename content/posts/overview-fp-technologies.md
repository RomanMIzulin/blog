+++
title = 'Overview Fp Technologies'
date = 2024-10-02T15:41:08+04:00
draft = false
+++

The goal of this article is to research the most popular FP based technologies.
Maybe you will like and adapt some of them.

##### Disclaimer
I have to confess that after looking at projects and languages and theories behind them, I became adept of FP if not languages but definitely of practices.

# A little bit of historical context
This engaging talk has a lot of references to historical moments:
["Propositions as Types" by Philip Wadler - YouTube](https://youtu.be/IOiZatlZtGU?si=3a2duU8bKRotpmcJ)
### Lisp
The first implementation based on lambda calculus - math background. Not just engineered, but also with good theoretical background. Today ELisp is used for Emacs.   
### Haskell
The first purely functional academic language to become relatavely popular, is called [Haskell](https://www.haskell.org/), was created in 1990. Since then a lot new languages and technologies appeared. Let's observe the most popular open source projects written in mostly pure functional languages for last 30+ years.
### OCaml
OCaml was written in 1996 in France. It was inspired by a long line of research into ML, starting in the 1960s, and continues to have deep links to the academic community.
### ML (Meta Language)

# Top projects grouped by language

## Elixir
Appeared at 2012. Built on top of BEAM to make Erlang\OTP runtime more accessible, because Erlang is not user friendly really; and shares the same abstractions and OTP framework for building distributed, fault-tolerant applications. Originally dynamically typed, but it is actively looking forward for static typing [cnrs](https://www.ins2i.cnrs.fr/en/cnrsinfo/dynamic-static-elixir-begins-its-transformation). As Joe Armstrong said about types "no good type system save you from node failure" - that is why Erlang language is dynamicly typed. And it is one of the two languages in this list available on Leetcode, but(!) I would strongly recommend to use https://exercism.org/ for practice firstly. You can think about this language as more modern and easy to use language for BEAM runtime than original Erlang language. 
Why does it matter? Because Erlang really powers high load. You can find out more [here](https://elixir-lang.org/cases.html) about real world use cases of Erlang its VM called BEAM. Whats-app cloud handles 2 millions connection per a node for instance.
![[a.png|700]]
[x.com](https://x.com/guieevc/status/1002494428748140544)
It is simple language nevertheless a powerful one. Maybe Elixir has not really good theoretical fundament, but it is still good language and its author Jose Valim actively works on bringing type system with synergy of academid world. 
![[Screenshot from 2024-08-11 23-09-45.png|500]]
Picture from talk by creator of the lang Jose Valim about different levels of abstractions [Keynote: Gang of None? Design Patterns in Elixir - José Valim | ElixirConf EU 2024 - YouTube](https://youtu.be/agkXUp0hCW8?si=2Osk6MSEbgocakfq)

### [Phoenix: Top from stack overflow surveys](https://github.com/phoenixframework/phoenix)
Stars: **21k**\
One of the most if not the most popular FP frameworks that has won "the most admired web framework" at stackoverflow research for several years in a row.
[Stack Overflow Developer Survey 2023](https://survey.stackoverflow.co/2023/#section-admired-and-desired-web-frameworks-and-technologies)
Fullstack, Ruby inspired. Connects high load with easy of use.
There are big companies using this framework check related block at [Phoenix Framework](https://www.phoenixframework.org/)

### [analytics](https://github.com/plausible/analytics)
Stars: **19.1k**\
Simple, open source, lightweight (< 1 KB) and privacy-friendly web analytics alternative to Google Analytics. Serious niche and good moral idea.
All we can do - is to embrace such kind of projects.
> We are dedicated to making web analytics more privacy-friendly.

### [supabase/realtime](https://github.com/supabase/realtime)
Stars: 6.6k\
One of the projects of famous supabase project which leverages Phoenix from the first place. It makes use from BEAM through Elixir.

> This is a server built with Elixir using the  that enables the following functionality:
> - Broadcast: Send ephemeral messages from client to clients with low latency.
> - Presence: Track and synchronize shared state between clients.
> - Postgres Changes: Listen to Postgres database changes and send them to authorized clients.


## [Gleam](https://gleam.run)
Appeared at 2016. V1 was released at 4 Mar 2024, so it does not have popular projects yet, but it grows fast. Running on Erlang VM as Elixir, but statically typed in opposite of dynamically typed Elixir. Inspired by many languages and as author says "I stole the best ideas for this language.", Louis Pilfold. 
And I have to admit that coding in Gleam is pleasant experience. It is really easy to learn and fast Language server gives instant feedback on type coherence.
If you can choose among Erlang, Elixir and Gleam. You should deferentially look at  Gleam, but if you like Ruby look at Elixir of course.
Maybe it is true opensource sponsored language, in this meaning it is a good example contrasting to Elm.
Try it at [The Gleam Language Tour](https://tour.gleam.run/)

P.S. Remember Golang mascot? yeah... Now look at this piece of art.
![[Pasted image 20240812161117.png|200]]

### [Front end in  Gleam](https://github.com/lustre-labs/lustre)   
Lustre allows to write fullstack applications in Gleam reusing same types!
Basically it follows the same MVC Elm architecture.
 
## [Clojure](https://clojure.org/)
Appeared at 2007. There are a lot of talks on youtube about this language. 
Here are titans of Clojure world in terms of numbers of stars.
Used at Walmart Labs
	“Our Clojure system just handled its first Walmart black Friday and came out without a scratch.”

### [metabase](https://github.com/metabase/metabase)
Stars: **37.4k**\
Very popular tool for work with data for non-technical people. It let to get and visualize simple data without SQL, but for more complex queries SQL is required. One technical person can make views and all non technical part of a team can use it.

### [logseq](https://github.com/logseq/logseq)
Stars: **31.1k**\
A privacy-first, open-source platform for knowledge management and collaboration. 
Notion and Obsidian like alternative.

### [penpot](https://github.com/penpot/penpot)
Stars: **29.5k**\
The open-source tool for design and code collaboration.
Figma alternative.
By number of stars we can assume that IT world at least admired this tool.


## [Elm](https://elm-lang.org/)
Appeared at 2012. Extremely efficient and deligtful to use to build browser UI. Can be seen as more simple and compact child of Haskell and OCaml. Has good and simple type system.
There are elm-ui, elm-review popular libraries. And there is not much activity on official site actually, but languages is alive. It is in its afterhype period of time. In video below Evan told that he made compiler from Elm to SQL what sounds cool, but he really struggles to make sustainable financial model ["The Economics of Programming Languages" by Evan Czaplicki (Strange Loop 2023) - YouTube](https://www.youtube.com/watch?v=XZ3w_jec1v8)


## [Haskell](https://www.haskell.org/)
Academic influenced language appeared in 1990 with stable release at 2010. From the beginning made with good type design comparing to the most other popular languages where types were introduced on the go.
Highly admired by creator of ROC language - Richard Feldman. He also admired Elm as well.
This language has a lot of concepts, so it is a good idea to learn language to explore FP ideas in practice. 
And I would say that language is excellent for well understood problem that can be something formally described to leverage its strong type system.
Some researches say that there are better language than Haskell like Agda or Idris. Ok, but for many of FP languages Haskell is progenitor. 


### [ShellCheck](https://github.com/koalaman/shellcheck)
Stars: **35.6k**\
A static analysis tool for shell scripts adopted by: 
Travis CI, Codacy, Code Climate, Code Factor, CircleCI via the ShellCheck Orb
Github (only Linux), Trunk Check (universal linter; allows you to explicitly version your shellcheck install) via the shellcheck plugin
And you can use it for too if you work with bash/sh scripts.

###  [pandoc](https://github.com/jgm/pandoc)
Stars: **33.3k**\
Universal markup converter. Supports numerous format from/to. Practical and hepfull.

### [PostgREST](https://github.com/PostgREST/postgrest)
Stars: **22.7k**\
REST API with automatically generated OpenAPI for any Postgres database. Expose database schema with filters and make Postgres views for complex API endpoints.
If you often write CRUD API for database tables manually, it will save you somme time.

#### And more less popular projects
Like [hadolint: Dockerfile linter, validate inline bash, written in Haskell](https://github.com/hadolint/hadolint); Purescript, Unison, Idris languages implemented in Haskell.
I recommend to check ideas behinds those projects. Especially Unison's mind-blowing something naive idea about infinite computational resoures.

## ReasonML 
Seems like extreme niche at this moment, I mean it is used only as alternative to JS when working with React.

## Scala
Brings FP to Java land. Good path for whom looking for functional language to code and the best job opportunities. But definitely not the best in my humble opinion. 

### [Enso](https://github.com/enso-org/enso)
Stars: 7k\
Interesting analytical tool and  language with one-to-one visual counterpart.
And can be used for "Detecting Credit Card Fraud with Enso" as stated in their blog post.
![[enso.png]]

## Python with returns lib
Python is not functional language itself. And as I can relate does not want to be: look at lambda for instance. But this package allows to write more robust applications.
Link to lib: [GitHub - dry-python/returns: Make your functions return something meaningful, typed, and safe!](https://github.com/dry-python/returns/tree/master)

# In closing

You may wonder after all why then functional programming languages are not used everywhere if it is so good? So Richard gave a good answer to it: [Why Isn't Functional Programming the Norm? – Richard Feldman - YouTube](https://youtu.be/QyJZzq0v7Z4?si=R8jJpX7Amc2Ad-cI). 

# Also check this

- [Beating the Averages](https://paulgraham.com/avg.html)
- [Functional Programming in 40 Minutes • Russ Olsen • GOTO 2018 - YouTube](https://youtu.be/0if71HOyVjY?si=5eri2O_O04u-NBYb)
- [Why algebraic data types are important - Bartosz Milewski](https://www.youtube.com/watch?v=LkqTLJK2API)

