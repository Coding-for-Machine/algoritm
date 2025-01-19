Python va Go Dasturlash Tilidagi Algoritmik Masalalar
<br>

Bu hujjat LeetCode uslubidagi stringlarga oid 100 ta masala va ularning qisqacha tavsifidan iborat. Har bir masalani Python yoki Go dasturlash tilida yechish mumkin.
<br>

1-10: Boshlang'ich String Masalalari
<br>

Reverse String: Berilgan stringni teskari aylantiring. Masalan, "hello" → "olleh".<br>
go-da
<hr>

```go
package main

import "fmt"

func revers_string(str string)string{
  runes = []runes(str)
  i, j = 0, len(runes)-1
  for i<j {
    runes[i], runes[j] = runes[j], runes[i]
    i+=1
    j-=1
  }
  return runes

}

func main() {
  reversed := revers_string("Hello, Go")
  fmt.Println(reversed)
}
```
pythond-da
<hr>

```python
def revers_string(string: str)->str:
  lists = list(string)
  i, j = 0, len(lists)-1
  while i<j:
    lists[i], lists[j] = lists[j], lists[i]
    i+=1
    j-=1
  return "".join(lists)
```
<br>

Palindrome Checker: String palindrome ekanligini tekshiring. Masalan, "racecar" palindrome hisoblanadi.
<br>
```python
def palindrom_str(string: str)->str:
  i, j = 0, len(string)-1
  while i<j:
    if string[i]!=string[j]:
      return False
      i, j = i+1, j-1
  return True
```
First Unique Character: Stringda birinchi marta uchraydigan noyob belgini toping.
<br>

Anagram Check: Ikkita string bir-birining anagrami ekanligini aniqlang.

(1)

```python
def anagram(s: str, t: str)->str:
  s1 = {}
  s2 = {}
  for i in s:
    s1[i]=s.get(i, 0)+1
  for i in t:
    s2[i]= s2.get(i, 0)+1
  return s1==s2
```
(2)

```python
from callections import Counter

def anagram(s: str, t: str)->str:
  s1 = Counter(s)
  s2 = Counter(t)
  return s1==s2
```

(3)

```python
def anagram(s: str, t: str)->str:
  return reversed(s1)==reversed(s2)
```

<br>

Count Vowels: Stringdagi unli harflar sonini hisoblang.
<br>

Longest Common Prefix: Stringlar ro'yxatidagi eng uzun umumiy prefiksni toping.
<br>

String Compression: Stringni qatorlab takrorlanadigan belgilarni sanab qisqartiring. Masalan, "aabcccccaaa" → "a2b1c5a3".
<br>

Valid Parentheses: Stringda qavslar balanslanganmi yoki yo'qligini tekshiring.
<br>

Remove Duplicates: Stringdan takrorlanadigan belgilarni o'chirib tashlang.
<br>

Substring Search: Berilgan substring asosiy string ichida bormi, aniqlang.
<br>

11-20: O'rta Darajadagi String Masalalari
<br>

Longest Palindromic Substring: String ichidagi eng uzun palindrom substringni toping.
<br>

Group Anagrams: Stringlar ro'yxatini anagramlar guruhiga ajrating.
<br>

Isomorphic Strings: Ikkita string izomorfik ekanligini tekshiring.
<br>

String Rotation: String boshqa stringning aylantirilgan ko'rinishi ekanligini aniqlang.
<br>

Count and Say: Stringni "hisobla va ayt" qoidasi asosida hosil qiling. Masalan, 1 → "11" → "21" → "1211".
<br>

Zigzag Conversion: Stringni zigzag tartibida yozing va qayta yig'ing.
<br>

String to Integer (Atoi): Stringni integerga aylantiring, agar bu mumkin bo'lsa.
<br>

Longest Substring Without Repeating Characters: Takrorlanmaydigan belgilar ketma-ketligidan eng uzunini toping.
<br>

Valid Palindrome II: Bitta belgi o'chirilganda string palindrome bo'ladimi, aniqlang.
<br>

Remove K Digits: String ko'rinishidagi sonni k ta raqam o'chirib eng kichik qiymatga keltiring.
<br>
21-30: Avans String Masalalari
<br>

String Permutations: Berilgan stringning barcha mumkin bo'lgan permutatsiyalarini hosil qiling.
<br>

Wildcard Matching: Stringni wildcard andozaga mosligini tekshiring. Masalan, "a?b*".
<br>

Minimum Window Substring: Asosiy string ichidagi substringni toping, unda boshqa stringdagi barcha belgilarning ko'rsatmalari mavjud bo'lishi kerak.
<br>

<br>
Repeated DNA Sequences: 10 ta belgidan iborat bir xil substringlarni toping.

Multiply Strings: Ikkita stringdagi sonlarni ko'paytiring.
<br>

Roman to Integer: Rim raqamini integerga aylantiring.
<br>

Integer to Roman: Integer qiymatini rim raqamiga aylantiring.
<br>

Valid Number: Stringni haqiqiy raqam ifodasi ekanligini aniqlang.
<br>

Compare Version Numbers: Ikki versiya raqamini solishtiring, masalan "1.0.1" > "1.0.0".
<br>

Decode String: Kodlangan stringni oching, masalan, "3[a2[c]]" → "accaccacc".
<br>
