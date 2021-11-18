#   Фаззинг и формальная верификация

 1. проблемы разработки протоколов и сетевого ПО, пример Markdown
    CommonMark https://commonmark.org,
    StrictMark http://doc.replicated.cc/%5EWiki/strictmark.sm
 2. вопросы спецификации и тестирования,
 3. формальная верификация алгоритмов,
    OT и coq в JetBrains https://itp2016.inria.fr/files/2016/06/chuprikov-slides.pdf,
    CRDT и Isabelle в Оксфорде https://github.com/trvedata/crdt-isabelle/blob/master/src/Convergence.thy https://martin.kleppmann.com/papers/crdt-isabelle-oopsla17.pdf
 4. фаззинг
     1. blackbox / whitebox / greybox,
          - AFL++ black/grey https://github.com/AFLplusplus/AFLplusplus,
          - libfuzzer grey https://github.com/google/fuzzing/blob/master/tutorial/libFuzzerTutorial.md,
          - Kernel fuzzer https://github.com/google/syzkaller,
          - доклад по фаззингу ядра Linux https://www.linuxfoundation.org/webinars/fuzzing-linux-kernel/,
     2. coverage coverage coverage - как считается, как максимизируется
 5. практическое использование
     1. эволюция проекта - как по шагам внедрить фаззинг в проекте,
         1. unit tests,
            table driven unit tests: https://dave.cheney.net/2019/05/07/prefer-table-driven-tests
         2. property tests
         3. fuzz tests,
            The Heartbleed OpenSSL bug https://en.wikipedia.org/wiki/Heartbleed,
            Fuzzing Heartbleed https://google.github.io/clusterfuzz/setting-up-fuzzing/heartbleed-example/,
            Fuzzing смарт контрактов https://github.com/crytic/echidna
         4. minimization
         5. loopback
     2. корпус - накопление и использование,
     3. CI
        JetBrains TeamCity https://www.jetbrains.com/teamcity/

