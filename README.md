# CodeWars_Delete_Vowels
Removing vowels from the received string from the user

#Trolls are attacking your comment section!
#A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.
#Your task is to write a function that takes a string and return a new string with all vowels removed.
#For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".

For the solution, we use the def function and the for loop.

def remove_vowels(comment):
    vowels = "aeiouyAEIOUYаеёиоуыэюяАЕЁИОУЫЭЮЯ"
    result = ""

    for word in comment:
        if word not in vowels:
            result += word
    return result

input_comment = str(input("Share your comment here: "))
result = remove_vowels(input_comment)
print(result)
