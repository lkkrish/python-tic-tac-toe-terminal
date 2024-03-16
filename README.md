structure = '''
      /   /
  _1_/_2_/_3_
 _4_/_5_/_6_
_7_/_8_/_9_
  /   /    '''
counter = 0
f =0
trun = "X"
data_container = list()
while counter < 10:
    if trun ==  "X":
        trun = "Y"
        
        changer = input("This is your trun player X please enter a number ")
        data_container.append(changer) 
        structure = structure.replace(changer,"X")
        print (structure)
    else :
         trun = "X"
         changer = input("This is your trun player y please enter a number ")
         structure = structure.replace(changer,"Y")
         
         print (structure)

    counter = counter + 1
    data_container.sort() 
    if data_container[0:3] == ['1', '2', '3']:
        print ("The winner is the player X")
        break


