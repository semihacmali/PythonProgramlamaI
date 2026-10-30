# PYTHON PROGRAMLAMA – ÖDEV YÖNERGESİ

**Ödev konuları:** ASCII Tablosu ve Temel Hesap Makinesi  
**Programlama dili:** Python 3  
**Ödev türü:** Bireysel uygulama  
**Teslim tarihi ve yöntemi:** Ders sorumlusu tarafından duyurulacaktır.

## Genel Kurallar

- Her ödev için ayrı bir Python dosyası oluşturunuz.
- Programlarınız Python 3 ile çalışmalıdır.
- Kodunuzu kendiniz yazınız; değişken adlarını anlaşılır seçiniz ve gerektiği yerde kısa açıklama satırları ekleyiniz.
- Her iki programı da çalıştırıp farklı girdilerle test ediniz.
- Teslim dosyalarının adları `odev1_ascii.py` ve `odev2_hesap_makinesi.py` olmalıdır.

---

## Ödev 1 – ASCII Tablosunu Ekrana Yazdırma

### Amaç

Python'da döngüleri, sayısal değerleri ve karakter dönüşümünü kullanarak ASCII karakter tablosu oluşturmak.

### Yapılacaklar

1. **0 ile 127 arasındaki (0 ve 127 dâhil)** tüm ASCII kodlarını bir döngü kullanarak ekrana yazdırınız.
2. Her satırda karakterin **ondalık ASCII kodu** ve **karşılığı olan karakter** gösterilmelidir.
3. Yazdırılabilir karakterler için `chr()` fonksiyonundan yararlanınız.
4. **0–31 ve 127** kodları kontrol karakteridir; bunlar doğrudan görüntülenmek yerine `Kontrol karakteri` şeklinde belirtilmelidir.
5. Tablo okunabilir olmalı, başlık ve sütun adları içermelidir.

### Örnek ekran çıktısı (kısaltılmış)

```text
ASCII KODU | KARAKTER
-----------|-------------------
0          | Kontrol karakteri
1          | Kontrol karakteri
...
32         | [boşluk]
33         | !
34         | "
35         | #
...
65         | A
66         | B
...
97         | a
...
127        | Kontrol karakteri
```

> **Not:** 32 kodu boşluk karakteridir. Görünür olması için `[boşluk]` şeklinde gösterilebilir. Bu örnek, çözüm kodu değil, beklenen çıktı biçimidir.

## Ödev 2 – `if` ile Temel Hesap Makinesi

### Amaç

Python'da kullanıcı girdisi alma, koşullu ifadeler (`if` / `elif` / `else`) ve aritmetik operatörlerle işlem yapma becerilerini geliştirmek.

### Yapılacaklar

1. Kullanıcıdan **iki sayı** alınız. Sayılar ondalıklı olabilir.
2. Kullanıcıdan gerçekleştirmek istediği **işlem operatörünü** alınız.
3. Aşağıdaki altı işlemi `if` / `elif` / `else` koşullarıyla gerçekleştiriniz:

   | Operatör | İşlem |
   |---|---|
   | `+` | Toplama |
   | `-` | Çıkarma |
   | `*` | Çarpma |
   | `/` | Bölme |
   | `**` | Üs alma |
   | `//` | Tam (taban) bölme |

4. İşlem sonucunu ekranda anlaşılır bir şekilde gösteriniz.
5. **Bölen sayı 0 ise**, `/` ve `//` işlemlerinde program hata vererek kapanmamalı; kullanıcıya açıklayıcı bir uyarı göstermelidir.
6. Listelenmeyen bir operatör girildiğinde `Geçersiz işlem` uyarısı veriniz.
7. Aritmetik işlemleri belirlemek için `eval()` kullanmayınız; **koşul ifadeleri** kullanılması zorunludur.

### Örnek çalışma 1

```text
Birinci sayıyı giriniz: 8
İkinci sayıyı giriniz: 3
İşlemi giriniz (+, -, *, /, **, //): **
Sonuç: 512.0
```

### Örnek çalışma 2

```text
Birinci sayıyı giriniz: 10
İkinci sayıyı giriniz: 0
İşlemi giriniz (+, -, *, /, **, //): /
Hata: Bir sayı sıfıra bölünemez.
```
### Örnek çalışma 3

```text
Birinci sayıyı giriniz: 10
İkinci sayıyı giriniz: 3
İşlemi giriniz (+, -, *, /, **, //): %
Geçersiz işlem.
```

> **Not:** Python'da `//` işlemi aşağı yuvarlayarak bölme yapar. Örneğin `10 // 3` sonucu `3`, `-10 // 3` sonucu `-4` olur.


## Teslim ve Kontrol Listesi

Teslim öncesinde aşağıdaki maddeleri kontrol ediniz:

- [ ] `odev1_ascii.py` dosyası 0–127 arası ASCII tablosunu oluşturuyor.
- [ ] `odev2_hesap_makinesi.py` altı işlem operatörünü destekliyor.
- [ ] Hesap makinesi sıfıra bölme girişlerinde hata vermeden uyarı gösteriyor.
- [ ] Her iki dosya Python 3 ile çalıştırılarak test edildi.
- [ ] **Dosyaları kendi Github Hesaplarınızda paylaşmak zorundasınız.**
