Original Source Code by Egor-Skriptunoff
Source Code : https://github.com/Egor-Skriptunoff/pure_lua_SHA
MIT License
------------------------------------------------
Ported to Hollywood by Fabio Falcucci
Completed : 03/11/2021
Version   : 1.0
Contact   : info@a-mc.biz
Patreon   : https://www.patreon.com/Allanon71
GitHub    : https://github.com/Allanon71
Twitter   : https://twitter.com/Allanon71
Dependancies      : - none -
Hollywood version : ported and tested with Hollywood 9.0
------------------------------------------------
NOTES
   Debugging was a hell mostly because LUA table indexes starts from 0 while
   in Hollywood they starts from 1, in most cases I've added a dummy entry on index 0.
   Also there was problems handling the \0 character.
   
   See function test_hash_lib() for examples.
   Uncomment last line to perform a global test.
   
   All sha and hmac functions are stored in the sha table as follow:
     sha
       .md5           supported natively by Hollywood but ported as an exercise
       .sha1
       .sha224
       .sha256
       .sha512_224
       .sha512_256
       .sha384
       .sha512
       .sha3_224
       .sha3_256
       .sha3_384
       .sha3_512
       .shake128
       .shake256
       .hmac
       .hex2bin
       .base642bin
       .bin2base64