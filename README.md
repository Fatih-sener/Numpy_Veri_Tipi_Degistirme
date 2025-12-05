# NumPy Veri Tipleri ve Tip Dönüşümü (Type Casting)

Bu script, NumPy dizilerindeki (arrays) `dtype` mekanizmasının çalışma mantığını gösterir. NumPy, homojen bir yapıya sahip olduğu için veri tiplerini otomatik olarak yönetir veya manuel optimizasyona izin verir.

## İncelenen Mekanizmalar
* **Otomatik Tip Algılama:** Tamsayılar için varsayılan `int32` veya `int64` ataması.
* **Upcasting (Yükseltme):** Bir dizi içinde tamsayı ve ondalıklı sayı (`5.0`) karışık verildiğinde, NumPy veri kaybını önlemek için tüm diziyi otomatik olarak `float` türüne çevirir.
* **Type Casting (`.astype`):** Veri tipini manuel olarak değiştirme (Örn: `float` -> `int`).
* **Memory Optimization:** `dtype="int8"` parametresi ile dizinin bellekte kapladığı alanı minimize etme (Büyük verilerde %87'ye varan tasarruf sağlar).
* **String/Unicode:** Sayısal olmayan verilerin (tarih/metin) NumPy tarafından nasıl etiketlendiği (`<U...`).
