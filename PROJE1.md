Proje 1
[22,27,16,2,18,6] -> Insertion Sort

Görev-1
Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.


Dizini küçükten büyüğe sıralamalıyız.
1- [2,27,16,22,18,6] -> Dizinin en küçük sayısı 2'dir. 22 ile yer değiştirir.
2- [2,6,16,22,18,27] -> İkinci küçük sayı 6'dır, 27 ile yer değiştirir.
3- [2,6,16,22,18,27] -> Üçüncü küçük sayı 16'dır, sıralaması doğrudur, işlem yapılmaz.
4- [2,6,16,18,22,27] -> Dördüncü sayı 18'dir, 22 ile yer değiştirir.
5- [2,6,16,18,22,27] -> Beşinci ve altıncı sayıların sıralaması doğrudur, işlem yapılmaz.


Görev-2
Big-O gösterimini yazınız.


Dizideki eleman sayısı=n
Big-O yöntemine göre sıralama yapılırken işlem sayısı da n'dir.
Son işlem sayısı 1 olana dek işlem devam eder.
[22,27,16,2,18,6] dizininde eleman sayısı 6'dır. 6 işlem yapılacaktır;
1- n -> 6 işlem,
2- En küçük(birinci) elemanı bulmak için (n-1) -> 6-1=5 işlem yapılacaktır.
3- İkinci elemanı bulmak için (n-2) -> 6-2=4 işlem yapılacaktır.
4- Üçüncü elemanı bulmak için (n-3) -> 6-3=3 işlem yapılacaktır.
5- Dördüncü elemanı bulmak için (n-4) -> 6-4=2 işlem yapılacaktır.
6- Başka işlem yapılmasına gerek yoktur zira altıncı eleman sonuncudur.

Bu algoritmada n+(n-1)+(n-2)+(n-3)+(n-4)+1 kadar(bu örnekte: 21) işlem yapılmıştır.
İşlemin formülü: [n(n+1)]/2'dir. Formülü sadeleştirilerek: (n²+n)/2 formülünü elde ederiz.
Big-O Notation'da domine eden fonksiyon, yani n² baz alınır.

Big-O değeri = O(n²)


Görev-3
Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız
Average case: Aradığımız sayının ortada olması
Worst case: Aradığımız sayının sonda olması
Best case: Aradığımız sayının dizinin en başında olması.

Avarage case: [22,27,16,18,2,6]
Worst case: [22,27,16,2,6,18]
Best case: [18,22,27,16,2,6]


Görev-4
[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.

1- [2,3,5,8,7,9,4,15,6] 7<->2
2- [2,3,5,8,7,9,4,15,6] (değişiklik yok)
3- [2,3,4,8,7,9,5,15,6] 5<->4
4- [2,3,4,5,7,9,8,15,6] 8<->5


www.patika.dev