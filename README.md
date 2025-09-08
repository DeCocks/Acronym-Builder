Acronym Builder

Given a string containing one or more words, return an acronym of the words using the following constraints:

    The acronym should consist of the first letter of each word capitalized, unless otherwise noted.
    The acronym should ignore the first letter of these words unless they are the first word of the given string: a, for, an, and, by, and of.
    The acronym letters should be returned in order they are given.
    The acronym should not contain any spaces.




** start of main.py **

def build_acronym(s):
    
    print(s)
    s= s.upper()
    print(s)
    lijst=s.split( )
    lengtelijst=len(lijst)
    tel = 0
    result=""
    while tel < lengtelijst:
        woord=lijst[tel]
        print(woord)
        eersteKar=woord[0]
        if (woord=="A"or (woord=="FOR"and tel!=0) or (woord=="AN"and tel!=0)or woord=="AND"or (woord=="BY"and tel!=0)or woord=="OF"):
            print("doe niets")
        else:
            result+= eersteKar
            print(result)
        tel+=1

    s=result     


    return s


** end of main.py **

