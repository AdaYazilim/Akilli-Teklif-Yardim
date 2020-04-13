### DisDonenPoliceyiPolicelestir_Yardim
 
 "DisDonenPoliceyiPolicelestir" servislerinde kullanılabilinecek alanların bilgilerini döner.
 
**Link:**"http://localhost/ada/AkilliTeklif.DisDonenPoliceyiPolicelestir_Yardim.aaws"

**Parametreler:
** Ürün grubu
** Şirket Kodu
Şirket ve ürün kodu ile eşleşen alanlar dönmektedir.

##### Örnek İstek:
<pre>
[ "Trafik", "040"	]
</pre>

##### **Örnek Cevap:**
<pre>
{
	"Mesaj": "Genel Bilgilendirme",
	"Basarili": true,
  "KullanilabilirAlanlar":
    [
     {
            "Metin": "KrediKartiUstundekiIsim",
            "Deger": "Kart Sahibinin Adı Soyadı"
        },
        {
            "Metin": "KrediKartiNo",
            "Deger": "Kredi Kartı Numarası (1111-1111-1111-1111)"
        },
      ...
    ]
}
</pre>
