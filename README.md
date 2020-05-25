GitHub readme test
==================
this is the second title
------------------------
with no title

-----------------------
Carriage return test<br>
tast check <br>
`highlight` test<br>
[百度百科](www.baidu.com "百度百科")<br>

* *test1<br>
  * *test2<br>
    * *test3<br>
picture test：<br>
![test] (https://github.com/zddd312/zddd/blob/master/images/avatar.jpg)

-----------------------------------------------------------------------
code test:<br>
```C
void mp3_play(u8_num)
{
	int i;
	switch(u8_num)
	{
		case 1: song[6]=0x01;song[8]=0xf7;break;
		case 2: song[6]=0x02;song[8]=0xf6;break;
		case 3: song[6]=0x03;song[8]=0xf5;break;
		case 4: song[6]=0x04;song[8]=0xf4;break;
		case 5: song[6]=0x05;song[8]=0xf3;break;
		case 6: song[6]=0x06;song[8]=0xf2;break;
		case 7: song[6]=0x07;song[8]=0xf1;break;
		case 8: song[6]=0x08;song[8]=0xf0;break;
		default: ;
	}
	for(i=0;i<10;i++)
	{
		USART_SendData(USART2,song[i]);
		while (USART_GetFlagStatus(USART2, USART_FLAG_TC) == RESET);
	}
}
