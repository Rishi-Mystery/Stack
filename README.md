# Stack
#Stack by user input in python

stack = []
pointer = 1
value = 1

while(True):

    a = input("1. push \n2. pop \n3. peek \n4. clear \n5. end \n")
    
    if(a == "1" and pointer < 6):
      stack.append(value)
      value = value + 1
      pointer = pointer + 1
      print("\npush operation complete\n")

    elif(a == "1" and pointer == 6):
      print("\ncannot push, stack overflow!!\n")

    elif(a == "2" and pointer > 1):
      stack.pop()
      value = value - 1
      pointer = pointer - 1
      print("\npop operation complete\n")

    elif(a == "2" and pointer == 1 ):
      print("\ncannot pop, stack underflow!!\n")

    elif(a  ==  "3"):
      print("\n",stack, "\n")

    elif(a  ==  "4"):
      stack.clear()
      pointer = 1
      value = 1

    elif(a  ==  "5"):
      print("ended")
      break
