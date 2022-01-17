#   Консенсус (обзор)

 1. Византизм и проблема генералов во всех ее видах
 3. Paxos, Raft и друзья
 4. Proof-of-Work
 5. Proof-of-X

 Основные три предположения в любом консенсусе:
 1. асинхронная/синхронная сеть (это вопрос меры)
 2. сбои простые или византийские (когда могут лгать)
 3. ограниченный круг участников (permissioned) либо открытая сеть
 (permissionless)

 Ну и различные численные параметны тоже важны, например протокол с N^2 сообщений может не подойти при 1млн узлов.

 ##  Ссылки

   - труды L.Lamport http://lamport.azurewebsites.net/pubs/pubs.html#time-clocks
   - время и события в распределенных системах (Лампорт) https://lamport.azurewebsites.net/pubs/time-clocks.pdf
   - основа всех теорий репликации - машины состояний (кон автоматы) http://www.cs.cornell.edu/fbs/publications/SMSurvey.pdf
   - Проблема Византийских генералов - что если узлы не только дохнут, но и говорят неправду? (византизм) https://lamport.azurewebsites.net/pubs/byz.pdf
   https://www.cs.cornell.edu/courses/cs6410/2018fa/slides/18-distributed-systems-byzantine-agreement.pdf
   - PBFT - антивизантизм для сетевой файловой системы NFS http://pmg.csail.mit.edu/papers/osdi99.pdf
   - Сравнение Paxos, Raft простым языком https://arxiv.org/pdf/2004.05074.pdf
   - ConsensusDays 2021 https://research.protocol.ai/sites/consensusday21/programme/index.html
   - Какую сеть считать асинхронной - игра в определения https://decentralizedthoughts.github.io/2019-06-01-2019-5-31-models/
   - HotStuff - BFT консенсус для блокчейна https://arxiv.org/pdf/1803.05069.pdf
   (Proof of Stake в целом это попытка применить BFT к блокчейну, там много сложностей, в том числе крайне нерегулярные свойства открытой сети, где при этом очень много участников)
   - BitCoin и Proof of Work - идиотский алгоритм, который работает
   https://www.ussc.gov/sites/default/files/pdf/training/annual-national-training-seminar/2018/Emerging_Tech_Bitcoin_Crypto.pdf
