[16,21,11,8,12,22] şeklinde verilen sayı dizisini "Merge Sort" yöntemi ile sıralamamız istenmiş.
-Merge Sort sıralama yönteminde önce dizideki tüm elemanlar birer sayı dizisi olana kadar parçalanır ve sonradan tekrar birleştirilir.
-Verilen diziyi sürekli 2 ye şeklinde böleceğiz.

Step 1: [16,21,11] ve [8,12,22]
Step 2: [16,21] , [11] , [8,12] , [22]
Step 3: [16], [21], [11], [8], [12], [22] 

-Şimdi tekrar birleştiriyoruz ancak birleştirirken sıralayarak birleştiriyoruz.
- [16, 21]  [11] -- [8, 12] [22]
- [11, 16, 21] -- [8, 12, 22]
- [8, 11,12, 16, 21, 22]

- Big O gösterimini yazarken:
Step 1 -> n
Step 2 -> n/2
Step 3 -> n/4
....
Step (n-1) -> (n-1)/2^(n-2)

sum = n + n/2 + ... = n(1 + 1/2 + ...) = nlogn
O(nlogn)