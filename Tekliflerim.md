### TeklifleriAl
 
 Sistemde kayıtlı teklifleri almak için kullanılır.
 
**Link:**"http://localhost/ada/AkilliTeklif.TeklifleriAl.aaws"

**Parametreler:
<pre>
[
	{
		string UrunGrubu = "";//"Trafik" vs.
		string Query = "";//Teklif içinde geçen bir metin
		string TeklifIstegiQuery = "";//Teklif İsteği içinde geçen bir metin (Önerilmez.)
		string BaslangicTarihi = "";//"2019-12-20T00:00:00" teklif  başlangıç tarihi başlangıç
		string BitisTarihi = "";	//"2020-04-16T00:00:00" teklif başlangıç tarihi bitiş
	},
	-1//SonIslenenUpdateId, Sayfalama için kullanılır
]
</pre>



##### Örnek İstek:
<pre>
[
	{
		"Query": "",
		"TeklifIstegiQuery": "",
		"UrunGrubu": "",
		"BaslangicTarihi": "2019-04-12T00:00:00",
		"BitisTarihi": "2020-04-14T00:00:00",
		"OtomatikTeklifAlTip": "0"
	},
	-1
]
</pre>

##### **Örnek Cevap:**
<pre>
{
	"SonrakiSayfaVar": true,
	"SonIslenenUpdateId": 2634,
	"Teklifler": [
		{
			"donenPolicelerdeAlinsin": false,
			"Sigortalilar": [],
			"DonenPoliceler": [],
			"TeklifId": 471,
			"TeklifIdString": "471",
			"UrunGrubu": "Kasko",
			"IslemContext": null,
			"Alanlar": {
				"AcenteKullaniciAdi": {
					"Soru": "AcenteKullaniciAdi",
					"Cevap": "AAWUse"
				},
				"KimlikNo": {
					"Soru": "KimlikNo",
					"Cevap": "1503333653776"
				},
				"OtomatikTeklifAl": {
					"Soru": "OtomatikTeklifAl",
					"Cevap": "1"
				},
				"PlakaIlKodu": {
					"Soru": "PlakaIlKodu",
					"Cevap": "34"
				},
				"PlakaNo": {
					"Soru": "PlakaNo",
					"Cevap": "AT5577"
				},
				"Tarih": {
					"Soru": "Tarih",
					"Cevap": "13.04.2020 16:54:14"
				},
				"TeklifId": {
					"Soru": "TeklifId",
					"Cevap": "471"
				},
				"UrunGrubu": {
					"Soru": "UrunGrubu",
					"Cevap": "Kasko"
				}
			}
		},
    ...
    ]
  }
</pre>
