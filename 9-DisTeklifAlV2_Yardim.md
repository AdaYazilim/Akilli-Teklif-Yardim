### DisTeklifAlV2_Yardim

**Link:**"http://localhost/ada/AkilliTeklif.DisTeklifAlV2_Yardim.aaws"

**Parametreler:** Ürün grubu
ürün kodu desteklenmediğinde, kullanılabilecek ürün kodları dönmektedir. boş göndererek desteklenen ürün kodlarını görüntüleyebilirsiniz.

##### Örnek İstek:
<pre>
[ "Trafik"	]
</pre>

##### **Örnek Cevap:**
<pre>
{
	"Mesaj": "Genel Bilgilendirme",
	"Basarili": true,
  "KullanilabilirAlanlar":
    [
      {
        "Metin": "UrunGrubu",
        "Deger": "Trafik"
      }, {
        "Metin": "KimlikNo",
        "Deger": "***********"
      },
      ...
    ],
    "TeklifSigortaliOrnekNesne": 
    {
      "Ad":"",
      "Soyad":"",
      "Telefon":"",
      ...
    }
}
</pre>


