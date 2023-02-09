* Qi
   * Community
       * Community Outreach
           * The initial author gave a talk at RacketCon
           * An early adopter advocated for the project
           * An early adopter advocated for the project
           * An early adopter advocated for the project
           * An interactive tutorial was written using racket templates
           * The Qi design challenge was organized
           * The wiki was created
           * A Developer's Guide containing developer documentation was written
           * A weekly meetup for the project was started
           * Advent of Code was solved using Qi
       * Community Feedback
           * Core Suggestions
               * Improvements to the switch form were suggested
               * Improvements to switch were implemented
               * A design example was provided to motivate adding closures (the clos form) to Qi
               * The name clos was suggested for this form
               * Many options for proper macro extensibility were suggested
               * An illustrative example to motivate design improvements to the `feedback` form of the language was provided
               * There was a suggestion to restrict fancy-app's (a templatized function application library) scope in Qi to avoid tricky bugs in handling user input
               * It was pointed out that fanout does not accept arbitrary Racket expressions for N
               * An optimized implementation was suggested for fanout
               * A recipe for hosting backup documentation in case the package index is unavailable was provided
               * A way to measure load-time latency was suggested
               * There was a suggestion to use indirect documentation links to reduce build times
               * Some improvements were suggested to reduce memory consumption in building docs
           * Bugs
               * An installation issue was reported
               * A broken link in the documentation was reported
               * A confusing error message in the threading form was reported and a way to handle it was suggested
               * An elusive bug was identified that was causing performance degradation in the threading form
               * A hygiene issue related to the same bug was identified that could have caused other bugs in the future
           * Outreach Opportunities
               * The initial author was invited to give a talk at RacketCon
               * The initial author received feedback on drafts of the talk
               * A Q&A was held after the talk
               * There was a suggestion to write a tutorial
               * There was a suggestion to distribute a Qi template using racket templates
               * The idea of a Qi-themed event was suggested
               * There was a suggestion to create a wiki for Qi
               * The project benefited from general support from the Racket community
   * Core Features
       * Performance
           * The partition implementation was optimized
           * Benchmarking scripts were added
           * The performance benchmarks were audited for accuracy
           * The benchmarks were fixed according to the audit
           * The core macro was refactored into separate expansion and compilation stages
           * The number of dependencies was reduced
           * These tools were used to identify and remove all heavy dependencies and dramatically reduce load-time latency
           * The performance of any?, all?, and none? were significantly improved
       * Implementation
           * The initial implementation was written
           * A flow-oriented debugger was added
           * Some bugs in switch were fixed
           * An implementation for the prefix matching macro extensibility scheme was provided
           * "First class" macro extensibility was implemented, allowing users to seamlessly extend the syntax of the language
           * The suggested error message fix was implemented
           * fancy-app was restricted to just the fine-grained application form
           * The fancy-app PR was reviewed
           * fanout was modified to support arbitrary expressions for N and have an optimized implementation
           * partition was added, which is a generalized version of the sieve form
           * The ability to support the _ template in the function position was added
           * Support for keyword arguments to add bindings in lambda forms of the language was added
           * Uses of deprecated macro form ~or were updated to ~or*
       * Design
           * The language was designed
           * A simple macro extensibility based on prefix matching was designed, to allow users to extend the syntax of the language in a rudimentary way
           * The design of `feedback` was improved
           * The PR improving the design of `feedback` was reviewed
           * The fanout PR was reviewed
           * The partition PR was reviewed
           * The load-time latency PR was reviewed
       * Tool Support
           * A quickscript for entering unicode in DrRacket was written
           * A quickscript for interactive evaluation in DrRacket was added to support the Qi tutorial
       * Dev Tools
           * CI was set up for the project repository
           * Performance benchmarking was added to CI
           * A dependency profiler tool was written to identify heavy dependencies
           * A script to measure load-time latency following that approach was written
           * The benchmarks runner config was modified to avoid reporting success when it failed
       * Docs
           * Documentation was written for Qi
           * The backup docs workflow following the recipe was added
           * Some formatting and typos in the docs were fixed
           * The package config was modified so that Qi appears in the languages section of the docs
       * Organization
           * The repo was migrated to an organization account
           * The package was decomposed into lib/test/doc packages
           * The unused let/flow and let/switch macros were removed
           * The organization of some tests was improved
   * Extensions
       * The first library extending Qi functionality was written

Notes:
- Design of `feedback` may not be "Design" if it involved "Implementation" work.
- Review could be its own Core category.
- Core macro refactoring could be "Implementation" or "Performance" (I
have it in "Performance" now)
- Dev Docs could be "Docs"
- Lots of other highly subjective things :)
