import random
numOfCharacters = int(input("How many characters does your password need? Minimum 8 characters. "))
numLCase = 0
numUCase = 0
numSpecC = 0
numNums = 0
randomLC = ""
randomUC = ""
randomSC = ""
randomNum = ""
listofLCase = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v","w", "x", "y", "z"]
listofUCase = ["A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V","W", "X", "Y", "Z"]
listofSpecC = ["`", "`", "!", "@", "#", "$", "%", "^", "&", "*", "(", ")", "-", "_", "+", "=", "[", "{", "}", "]", "|", ",", "<", ">", ".", "?", "/"]
listofNums = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]
pList =[]
addCharacter = ""
password = ""
def numOfEachCharacters(total):
    global numLCase
    global numUCase
    global numSpecC
    global numNums
    numLCase = random.randint(2, numOfCharacters-6)
    numUCase = random.randint(2, numOfCharacters-numLCase-4)
    numSpecC = random.randint(2, numOfCharacters-numLCase-numUCase-2)
    numNums = numOfCharacters-numLCase-numUCase-numSpecC
    return numLCase
    return numUCase
    return numSpecC
    return numNums
def makepList():
    global pList
    for i in range(numLCase):
        randomLC = random.randint(0,25)
        pList.append(listofLCase[randomLC])
    for i in range(numUCase):
        randomUC = random.randint(0,25)
        pList.append(listofUCase[randomUC])
    for i in range (numSpecC):
        randomSC = random.randint(0,26)
        pList.append(listofSpecC[randomSC])
    for i in range (numNums):
        randomNum = random.randint(0,9)
        pList.append(listofNums[randomNum])
    return pList
def makePassword():
    global password
    random.shuffle(pList)
    password = "".join(pList)
    return password

numOfEachCharacters(numOfCharacters)
makepList()
print(makePassword())
