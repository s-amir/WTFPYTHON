# WTFPYTHON
- ### walrus operator :=
  it used for assigne value to variable and to return the value like (a:=1)
  print (num:=1)  
  -usage : if (j:=1+3) > 4: print(11)  
  in this statement it assgine value to variable j and return it too  
  (better than using = operator)   
  x = (a := 696, 9)   
  x  
  (696, 9)  
  a  
  696
- ### Be careful with chained operations  
  False is False is False  
  True  
  HOW? > (False is False) and (False is False)
- ### is VS ==:  
  is check reference while == check value:  
  5 == 5.0 == 5 + 0j  --> True 
  5 is 5.0 is 5+ 0j --> False  (beacuse of type difference)
  
- ### y=(x for x in range(20000000000) if x % 2==0):  
  y=(x for x in range(20000000000) if x % 2==0)  
  print(list(y))
  now generator runs to print all it's value
- ### nested list with 2 approach
  print(['']*3)  
--> ['', '', '']  
row=['']*3  
board=[row]*3  
print(board)  
--> [['', '', ''], ['', '', ''], ['', '', '']]  
board[0][0]=1  
print(board)  
--> [[1, '', ''], [1, '', ''], [1, '', '']]
  >> so all first elemnts change synchrounsly because they point to the same object
  #### next aproach to not point to same object  
  board = [['']*3 for _ in range(3)]
  >> Now you can just change board[0][0] and just it!
