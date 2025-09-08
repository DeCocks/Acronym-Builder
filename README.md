# Acronym-Builder
Acronym Builder  Given a string containing one or more words, return an acronym of the words using the following constraints:      The acronym should consist of the first letter of each word capitalized

str="Search Engine Optimization"
print(str)
str= str.upper()
print(str)
lijst=str.split( )
lengtelijst=len(lijst)
tel = 0
result=""
while tel < lengtelijst:
        woord=lijst[tel]
        print(woord)
        eersteKar=woord[0]
        result+= eersteKar
        print(result)
        tel+=1
print("***"+result+"***")
