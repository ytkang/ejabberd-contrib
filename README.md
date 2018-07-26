This is a forked repository of ejabberd-contrib.
- The only thing added into this repository is 
  ```
  mod_pottymouth/src/banword_gen_server.erl
  which is for checking ban words more flexable.
  for example,
  bloom_gen_server.erl check excatly same word
  ban word: "kkk"
  bloom check only "kkk"
  banword_gen_server check "kkkk", "kkkkkk", "kkk..." all words including "kkk"
  ```

- not use "etbloom" anymore. so you don't need to install bitarray. It is a rescue from install hell.