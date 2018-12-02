tried to use an interrupt and run into problems:
- interrupt works as expected
- if one interrupt is rised nothing else works:
  * light can't be switched
  * webserver isn't responding any more 
  -> maybe my interrupt is interrupted by another one?
  -> maybe the problem is that I use variables which are not volatile
  ok, if I just set a flag in the interrupt handler it works as expected
