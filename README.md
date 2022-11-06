# **Proje 1**

## ***Insertion Sort Projesi***
Inseriton Sort Algoritmasını kabaca açıklayacak olursak; Algoritma her seferinde baştan başlayarak dizinin üzerinde ileri doğru ilerleyerek, dizinin bir elemanını alıp geriye doğru elemanlar ile bir bir kıyaslar ve her kıyaslamada eğer sıraladığı elemandan daha küçükse o elemanla yer değiştirerek bir geriye atar.

![Insertion Sort GIF](https://upload.wikimedia.org/wikipedia/commons/4/42/Insertion_sort.gif)
---
* **1. Problem** 
```
 [22,27,16,2,18,6] -> Insertion Sort
 ```
 1. *Yukarda verilen dizinin sort türüne göre aşamalarını yazınız.*
 2. *Big-O gösterimini yazınız.*
 3. *Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.* 
 4. *Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.*
---
* **2. Problem**
```
[7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.
```
---
* ***1. Problemin Çözümü***
1. 1. Adım: İlk sayımız(22) tek başına sıralanamaz. Artık veri şu şekildedir:
   ```
    22 | 27 16 2 18 6
   ```

   2. Adım: 22 ile 27 verisi karşılaştırma yapılır. 22, 27 küçük olduğundan ilk iki veri tamamlanır. Herhangi bir değişiklik yapılmaz. Artık veri şu şekildedir:
   ```
    22 27 | 16 2 18 6
   ```

   3. Adım: 22 27 sıralı veri ile 16 kıyaslanır. 16 22 ve 27'den küçük olduğu için verinin başına geçer ve verimiz şu şekilde olur:
   ```
    16 22 27 | 2 18 6
   ```
   4. Adım: 16 22 27 sıralı veri ile 2 kıyaslanır. 2 verideki en küçük sayı olacaktır. Bu nedenle verinin en başına geçer. Artık veri şu şekildedir:
   ```
    2 16 22 27 | 18 6 
   ```
   5. Adım: 2 16 22 27 sıralı veri ile 18 kıyaslanır. 18, 2 ve 16'dan büyük; 22 ve dolayısıyla 27'den de küçüktür. 18 verideki yerini alır. Artık veri şu şekildedir:
   ```
    2 16 18 22 27 | 6
   ```
   6. Adım: 2 16 18 22 27 sıralı veri ile 6 kıyaslanır. 6, 2'den büyük 16 ve dolayısıyla sonrakilerden küçüktür. 6 verideki yerini alır. Artık verimiz şu şekildedir:
   ```
    2 6 16 18 22 27 |
   ```
   7. Adım: verimiz artık sıralı ve şu şekildedir:
   ```
    2 6 16 18 22 27
   ```
2. Big-O gösterimi: O(n^2)
3. 
   * **Worst case:** Aradığımız sayının sonda olması, Tam tersi verilmiş dizi, bu durumda dizinin her bir elemanı bir gerisindekinden küçük olacaktır. Dolayısıyla 1. eleman için iç döngü 0, 2. eleman için geriye doğru 1, 3. eleman için 2 daha sonra 3 4 5 6… n kadar geriye hareket yapacaktır. Yani 0+1+2+3+4…..+n-1 = [n*(n-1)]/2 : O(n^2)
   * **Average case:** Aradığımız sayının ortada olması, Worst case ile best casein ortalamasını aldığımızda O(n^2) olarak buluruz.
   * **Best case:** Aradığımız sayının dizinin en başında olması. Tam sıralı dizi, n tane sayinin üzerinden birer defa geçer ve hiç birini geriye doğru ilerletme gereği olmadığı için bu tek geçişle kalır. Yani O(n) veya O(1) demek daha doğru olur.
4. 18, Veri setinin ortasında olduğu için average case kapsamına girer.
---
* ***2. Problemin Çözümü***
1. Adım:
   ```
    7 | 3 5 8 2 9 4 15 6
   ```
2. Adım:
   ```
    3 7 | 5 8 2 9 4 15 6
   ```
3. Adım:
   ```
    3 5 7 | 8 2 9 4 15 6
   ```
4. Adım:
   ```
    3 5 7 8 |  2 9 4 15 6
   ```
---
## ***Patika***
[patika.dev](www.patika.dev) 
## ***License***
[MIT](https://choosealicense.com/licenses/mit/)