# InsertionAndSelectionSort

## Proje 1.1
[22,27,16,2,18,6] -> **Insertion Sort**

Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.

 **Insertion Sort algoritmasında, dizinin ikinci elemanından başlayarak her eleman sıralanmış kısımdaki elemanlarla karşılaştırılır. Karşılaştırma sonucunda, sıralı kısımda kendisinden büyük olan elemanlar sağa kaydırılır ve doğru pozisyon bulunduğunda eleman oraya yerleştirilir. Bu işlem dizi tamamen sıralanana kadar tekrar edilir.**

```
[22,27,16,2,18,6] Örneğimizi ele alalım;
22 ve 27 zaten sıralı, dolayısıyla hiçbir işlem yapmaya gerek yok.
[22,27,16,2,18,6]
3. elemanı (16) ele alalım. 27, 16'dan büyük olduğu için sağa kaydırılır. 22, 16'dan büyük olduğu için sağa kaydırılır. Sonuç olarak 16, 22'nin yerine yerleştirilir.
[16,22,27,2,18,6] 
4. elemanı (2) ele alalım. 2 sayısı 16,22 ve 27'den küçük olduğu için en sola kaydırılır.
[2,16,22,27,18,6] 
5. elemanı (18) ele alalım. 18 sayısı 22 ve 27'den küçük olduğu için iki sola kaydırılıp 3. sıraya yerleştirilir.
[2,16,18,22,27,6] 
Son olarak 6. elemanı (6) ele alalım. 6 sayısı 16,18,22 ve 27'den küçük olduğu için dört sola kaydırılıp 2. sıraya yerleştirilir. 
Son sıralamamız bu şekilde olur.
[2,6,16,18,22,27] 
```

**Big-O gösterimi şu şekildedir;**
- En iyi durum: Dizi zaten sıralıysa, karşılaştırmalar minimal olur ve O(n)'de çalışır.
- En kötü ve ortalama durum: Dizi ters veya karışık bir sıradaysa, her eleman için daha fazla karşılaştırma ve kaydırma yapılır, bu da O(n²)'ye çıkar.

**Time Complexity**: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer?
```
[2,6,16,18,22,27] 
Dizimizin sıralanmış halinde 18 sayısı 4. sıradadır. Yani bu bir average case'dir.
```

## Proje 1.2

[7,3,5,8,2,9,4,15,6] dizisinin **Selection Sort**'a göre ilk 4 adımını yazınız. 

```
1. [2, 3, 5, 8, 7, 9, 4, 15, 6] 7 ve 2 yer değiştirir.
2. [2, 3, 5, 8, 7, 9, 4, 15, 6] (değişim yok)
3. [2, 3, 4, 8, 7, 9, 5, 15, 6] 5 ve 4 yer değiştirir.
4. [2, 3, 4, 5, 7, 9, 8, 15, 6] 8 ve 5 yer değiştirir.
```
