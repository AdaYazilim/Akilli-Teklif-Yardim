### TeklifDetayiAl
 
 Sistemde kayıtlı teklifi almak için kullanılır.
 
**Link:**"http://localhost/ada/AkilliTeklif.TeklifDetayiAl.aaws"

**Parametreler: teklif Id


##### Örnek İstek:
<pre>
[
  123 //Teklif Id
]
</pre>

##### **Örnek Cevap:**
<pre>
{
	"Nesne": {		
		"Teklif": {
			"donenPolicelerdeAlinsin": true,
			"Sigortalilar": [],
			"DonenPoliceler": [
			{
					"Basarili": true,
					"Alanlar": [
						{
							"Soru": "TeklifId",
							"Cevap": "471"
						},
						{
							"Soru": "TeklifIstegiId",
							"Cevap": "3635"
						},
						{
							"Soru": "SirketKodu",
							"Cevap": "517"
						},
						{
							"Soru": "UrunGrubu",
							"Cevap": "Kasko"
						},
						{
							"Soru": "KullaniciId",
							"Cevap": "111"
						},
						{
							"Soru": "KayitIstekTipi",
							"Cevap": "T"
						},
						{
							"Soru": "Tarih",
							"Cevap": "13.04.2020 16:53:42"
						},
						{
							"Soru": "Manuel",
							"Cevap": "0"
						},
						{
							"Soru": "Durum",
							"Cevap": "0"
						},
						{
							"Soru": "PolicelestirmeKayitId",
							"Cevap": "0"
						},
						{
							"Soru": "SirketAdi",
							"Cevap": "UNICO SİGORTA A.Ş."
						},
						{
							"Soru": "AcenteKullaniciAdi",
							"Cevap": "test"
						}
					],
					"Hatalar": [],
					"HesaplamaSonuclari": [
						{
							"TaksitTipiStr": null,
							"NetPrim": 100.76,
							"BrutPrim": 170.8,
							"Komisyon": 10.13,
							"KuralHatalari": null,
							"IndirimArttirimlar": [],
							"OdemePlani": {
								"VadeTarihiStr": null,
								"Tutar": 0.0,
								"Komisyon": 0.0
							}
						}
					],
					"Teminatlar": [
						{
							"Kod": "630",
							"Ad": "630 KASKO",
							"Bedel": 100.0
						},
						{
							"Kod": "ASU",
							"Ad": "ASU AKSESUAR TEMİNATI",
							"Bedel": 0.0
						},
						...
					],
					"SirketAcenteNo": null,
					"SirketTeklifNo": "111111",
					"SirketTecditNo": null
				},
				...
			],
			"TeklifId": 471,
			"TeklifIdString": "471",
			"UrunGrubu": "Kasko",
			"IslemContext": null,
			"Alanlar": {
				"Ad": {
					"Soru": "Ad",
					"Cevap": "Cavit"
				},
				"AracBedeli": {
					"Soru": "AracBedeli",
					"Cevap": "67.991"
				},
				"AracKodu": {
					"Soru": "AracKodu",
					"Cevap": "034340"
				},
				...
		}
	},
	"Basarili": true,
	"Mesaj": ""
}

</pre>
