# pwnable.tw_silver-bullet

read_input 함수에서 null byte overflow를 이용해서 beat함수를 you win!으로 만들 수 있으며 return address를 덮을 수 있다.     
return address를 바이너리의 puts함수 부분으로 돌리고 인자로 got를 주어서 libc릭을 한다.  
다시 한번 read로 인풋을 받아 마찬가지로 null byte overflow를 이용해 beat함수를 you win!으로 만들고  
return address를 system("/bin/sh")로 돌린다!
