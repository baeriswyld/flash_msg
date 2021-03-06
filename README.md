# flash_msg

```
from flashmsg import flash_msg

--------------------------------------------------
#### Example 0
flash_msg(['Hello World'])

Output:
 *********************** 
 ***** Hello World ***** 
 *********************** 

--------------------------------------------------
# Example 1
flash_msg(msg=['Hello World',"I hope you find the flash message useful"],
          sign='#',
          bar_length=7,
          bar_name='Example 1')

Output:
 ############################################################################ 
 ####### Example 1 ####### Hello World                                ####### 
 ######################### I hope you find the flash message useful   ####### 
 ############################################################################ 


--------------------------------------------------
# Example 2
flash_msg(msg=['Very important message',"Clowns = Peter",'Specs: Shoes = 49, Costume=L'],
          sign="***",
          bar_length=2,
          bar_name='Fancy',
          color='red')

Output:
 ******************************************************* 
 ****** Fancy ****** Very important message       ****** 
 ******************* Clowns = Peter               ****** 
 ******************* Specs: Shoes = 49, Costume=L ****** 
 *******************************************************



--------------------------------------------------
# Example 3
import random
import string
from random import randint

def randomString(stringLength=10):
    """Generate a random string of fixed length """
    letters = string.ascii_lowercase
    return ''.join(random.choice(letters) for i in range(stringLength))


msg = [ randomString(randint(0, 50))  for i in range(10)]

flash_msg(msg=msg,
          sign="/*-//-*/",
          bar_length=2,
          bar_name='Stranger Things',
          color='green')

Output:
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-// 
 /*-//-*//*-//-*/ Stranger Things /*-//-*//*-//-*/ zzafthrdjhnqytpntowqwzkhrnpdsplrfzcysycahipbuuzaho /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// dmvnqpvbeefcdmxwmvszmrbpvlqtflfizedvlwowgiqxejyp   /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// yshxpnbmdgdzbmzvrxhpuxmyztitrlqnuycofhe            /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// xmakikkyhplqgolngidjowoodqaaxuoep                  /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// yyocmmplpbclnfupchckcifq                           /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// pd                                                 /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// cxrizdltioikxdvzthrzkpmabca                        /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// lktvubqhowwvkkpdjapkfwyvztvxaszgirrfuib            /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// kswlznwq                                           /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*// vvoxgndmxmriba                                     /*-//-*//*-//-*/ 
 /*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-//-*//*-// 