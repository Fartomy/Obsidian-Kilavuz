Obsidian URI bağlantıları, başka bir Obsidian kasasında ki bir nota bağlantı vermek için kullanılabilir. 

> [!WARNING]+ Uyarı 
>Tıklanacak olan bağlantının içeriği bu **Vault'da** değil başka bir vault'da olduğunda hata durumunda bağlantıyı kontrol etmeyi unutmayın. Ve de, bu ve bağlantısı verilmiş olan vault'un aynı dizinde olup olmadığını da kontrol ediniz. Son olarak farklı **işletim sistemlerinde** de bir sorunla karşılaşılması muhtemel çünkü ayarlanan bağlantı belirli bir işletim sisteminin **path** yoluna göre ayarlanmıştır. Bu yüzden farklı bir işletim sisteminde çalışmazsa şayet sorun bundan kaynaklanıyor olabilir. Yazılış şekillerine lütfen dikkat edin.[^1][^2][^3]

Yapılış şekli:

Üstünde çalıştığınız Vault'unuzda ki bir notunuza başka bir Vault'da ki notun bağlantısını şu şekilde verilebilir:

```md
[Not Bağlantısı](obsidian://open?path=D:%2Fpath%2Fto%2Ffile.md)
```

[Not Bağlantısı](obsidian://open?path=D:%2Fpath%2Fto%2Ffile.md)

Notunuza yol yerine **Vault adına** ve **dosya adına** göre de bağlayabilirsiniz:
```md
[Not Bağlantısı](obsidian://open?vault=main&file=main.md)
```
[Not Bağlantısı](obsidian://open?vault=main&file=main.md)

Yönlendirilmesi istenilen başka bir **Vault'da** ki notun **URL** linkini almak için;

- Yönlendirilmesi istenilen notun sol sekmeden (files) veyahut not açıksa üstte ki sekmeye (tabs) sağ tıklayıp `Copy Obsidian URL` butonuna tıklayın.
- Ardından yukarıda ki prototipi kullanarak `()` parantezlerin arasına bu bağlantıyı yapıştırın.

---
## Kodlama Standartı (Encoding/Escaping)

Değerlerinizin uygun şekilde URI kodlandığından emin olun. Örneğin, ==ileri eğik çizgi karakterleri== (/) `%2F` olarak kodlanmalıdır ve ==boşluk karakterleri== `%20` olarak kodlanmalıdır.

Bu özellikle önemlidir çünkü yanlış bir şekilde kodlanmış bir ==rezerve== karakter, URI'nin yorumlanmasını bozabilir. [Daha fazlası için](https://en.wikipedia.org/wiki/Percent-encoding)

[^1]:[Obsidian URI Linkleri](https://help.obsidian.md/Concepts/Obsidian+URI)
 [^2]:[Obsidian İşletim Sistemlerine Göre Path Durumları](https://vinzent03.github.io/obsidian-advanced-uri/getting_started)
 [^3]:[Obsidian İşletim Sistemlerine Göre Path Durumları - 2](https://help.obsidian.md/Concepts/Obsidian+URI)