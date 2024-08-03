[16,21,11,8,12,22] -> Merge Sort

![](https://private-user-images.githubusercontent.com/86906473/349045055-18a00de8-d167-47ff-8b6b-6359a7a59603.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjI2NzAxMzQsIm5iZiI6MTcyMjY2OTgzNCwicGF0aCI6Ii84NjkwNjQ3My8zNDkwNDUwNTUtMThhMDBkZTgtZDE2Ny00N2ZmLThiNmItNjM1OWE3YTU5NjAzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA4MDMlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwODAzVDA3MjM1NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTliNzhlOTA0MDM0MzgwMWNkNDQ3ZGUyMjA0NDQ2NDdkMjkxYTczY2FhNGZmOTlkMDM1YTI1NWYxOGE0YThjNTUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.GbdPXZpYkxk9H3ZEIYCsGT-LghN7sTSxKz4x3NI91BM)

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

Başlangıç dizisi: 16, 21, 11, 8, 12, 22

İlk bölme: 16, 21, 11 ve 8, 12, 22

Sol yarıyı bölme: 16, 21 ve 11

16, 21 bölme: 16 ve 21

16 ve 21 birleştirme: 16, 21

16, 21 ve 11 birleştirme: 11, 16, 21

Sağ yarıyı bölme: 8, 12 ve 22

8, 12 bölme: 8 ve 12

8 ve 12 birleştirme: 8, 12

8, 12 ve 22 birleştirme: 8, 12, 22

Son birleştirme: 11, 16, 21 ve 8, 12, 22

11 ve 8, 8 küçük: 8

11 ve 12, 11 küçük: 8, 11

16 ve 12, 12 küçük: 8, 11, 12

16 ve 22, 16 küçük: 8, 11, 12, 16

21 ve 22, 21 küçük: 8, 11, 12, 16, 21

Kalan eleman 22: 8, 11, 12, 16, 21, 22

Bu işlemler sonucunda sıralı dizi: 8, 11, 12, 16, 21, 22 elde edilir.

Big-O gösterimini yazınız.

a- diziyi bölme;

n

n/2

n/4 n/4

....

x adet 2'ye bölünme

2^x = n logn=x O(logn)

b- diziyi birleştirme;

Her seviyede O(n) zaman alır. Çünkü her seviyede n elemanını birleştirmek gereklidir.

Time complexity -> O(n)∗O(logn)=O(nlogn)'dir.