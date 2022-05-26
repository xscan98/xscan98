1.Media cifrelor unui numar:
num = 13579
z = [int(a) for a in str(num)]
print(z)
x=sum(z) / len(z)
print(x)
2.Sa se inlocuiasca fiecare caracter cu urmatorul din alfabet:
string = 'abcdefg'
new_string = ''.join(chr(ord(char)+1) for char in string)
print(new_string)
3.Se da un sir de nr, care e diferenta dintre max si minim; in sir de la 1 la 100 -
100-1=99 :
z=[1,2,3,4,5,100]
print(max(z))
print(min(z))
x=max(z)-min(z)
print(x)
4.Toate numerele impare si pare dintr-un sir:
list1 = [11, 23, 45, 23, 64, 22, 11, 24]
# iteration
for num in list1:
    # check
    if num % 2 == 0:
        print(num, end=" ")
for num in list1:
    if num % 2 ==1:
      print(num, end=" ")
5. Sir de caractere pe doua spatii consecutive se da space:
cuvant="acces"
splitat=2
if (cuvant[1] == cuvant[2]):
   print(cuvant[:splitat]+ " " + cuvant[splitat:])
6. Sa se scoada vocalele si sa se faca mirror
cuvant="acces"
vowels = ('a','e','i','o','u')
for x in cuvant.lower():
        if x in vowels:
            cuvant = cuvant.replace(x,"")
reversed=''.join(reversed(cuvant))
print(reversed)
7. Numere prime in matrice

import array as arr
a = arr.array('i', [2, 3, 4, 5])
print("Prime numbers are :", end=" ")
for i in a:
    num = i
j= 2
f= 1
while j < num:
if num % j == 0: f= 0
break j=j+ 1
    if f == 1:
        print(num,)
8. Cuvinte in ordine inversa
def wordReverse(str):
    i = len(str)-1
    start = end = i+1
    result = ''
    while i >= 0:
        if str[i] == ' ':
            start = i+1
            while start != end:
                result += str[start]
                start += 1
            result += ' '
end = i i -= 1
    start = 0
    while start != end:
        result += str[start]
        start += 1
    return result
# Driver Code
str = 'I AM A GEEK'
print(wordReverse(str))
9. Numere inlocuite de semnul exclamarii
cuvant="Ana are 2 mere 3"
numere = ('2','3','4')
for x in cuvant():
        if x in vowels:
            cuvant = cuvant.replace(x,"!")
print(cuvant)
10. Numarul de spatii dintr-un sir de caractere
cuvant="ala bala porto cala"

print(cuvant.find(" "))
11. Dubleaza vocalele
cuvant="laringe"
vowels = ('a','e','i','o','u')
for x in cuvant:
        if x in vowels:
            cuvant = cuvant.replace(x,x+x)
print(cuvant)
12. Sa se calculeze media numerelor dintr-un sir si sa se determine care element
din acest sir este cel mai apropiat de medie.
a_list = [1, 5, 8, 100]
average = sum(a_list) / len(a_list)
absolute_difference_function = lambda list_value : abs(list_value - average)
closest_value = min(a_list, key=absolute_difference_function)
print(closest_value)
13.De cate ori apare litera “a” intr-un sir.
cuvant="alabalaportocala"
print (cuvant.count("a"))
14.De cate ori apare cifra doi intr-un numar
cuvant="25231422"
print (cuvant.count("2"))
15. se dau 5 variabile, acestea trebuie sortate fara a utiliza vectori
numar=input((" Baga numaru 1 baiatu "))
numar2=input((" Baga numaru 2 baiatu "))
numar3=input((" Baga numaru 3 baiatu "))
numar4=input((" Baga numaru 4 baiatu "))
numar5=input((" Baga numaru 5 baiatu "))
print(sorted([numar,numar2,numar3,numar4,numar5]))
16.Se da un sir de valori numerice, sa se elimine elementele prime
a = [5,7,22,67,123]
b=[]
for s in a:
       for i in range(2, s):
           if(s % i==0):
               break;
           if(i==s-1):
b.append(s)
for ss in b:
    while ss in a:
        a.remove(ss)
print(a)
17.Sa se elemine elementul minim si elementul maxim dintr-un sir
mylist = [1, 4, 0, 3, 2]
mylist.remove(max(mylist))
mylist.remove(min(mylist))

18. Fibonacci number
import math as m
def is_Perfect_Square(K):
    s = int(m.sqrt(K))
    return s * s == K
def is_Fibonacci(R):
    return is_Perfect_Square(5 * R * R + 4) or is_Perfect_Square(5 * R * R - 4)
for J in range(1, 22):
     if (is_Fibonacci(J) == True):
         print ("Number:", J, ": Yes, the given number is a Fibonacci_Number")
     else:
         print ("Number:", J, ": No, the given number is not a Fibonacci_Number")
19. Se da un sir cu 5 valori numerice. Sa se afiseze toate permutarile posibile ale
acestui sir
from itertools import permutations
perm = permutations([1, 2, 3])
for i in list(perm):
    print (i)
20. Se da un sir de caractere. Sa se inlocuiasca toate literele mari cu litere
mici. Ex: 'Ana are mEre' -> 'ana are mere'
 propozitie= " Sa UrC cu Capra StANcA"
print(propozitie.lower())
21. Sa se calculeze oglinditul unui numar.
n = 725
c3 = n % 10
c2 = (n // 10) % 10
c1 = n // 100
invers = c3 * 100 + c2 * 10 + c1
print("Răsturnatul =", invers)
22. Sa se verifice daca un numar dat este palindrom
numar=input((" Baga numaru baiatu"))
if(numar==numar[::-1]):
      print("ai ciocanit spre ciocanesti, Jhonutz")
else:
      print("Da ce ai facut Bobitza?")
