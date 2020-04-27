### Araç Kullanım Tarzları

**Link:**"http://localhost/ada/TeklifSabitleri.AracKullanimTarzlari.aaws"

##### Örnek İstek:
<pre>
[]
</pre>

##### **Örnek Cevap:**
<pre>
[
    {
        "Metin": "Otomobil",
        "Deger": "01"
    },
    {
        "Metin": "Taksi",
        "Deger": "02"
    },
  ...
]
</pre>


<h3>Araç Kullanım Şekli</h3>

<table>
<tr>
<th>KullanimSekli</th>
<th>Açıklama</th>
</tr>
<tr>
<td>0</td>
<td>Hususi</td>
</tr>
<tr>
<td>1</td>
<td>Resmi</td>
</tr>
<tr>
<td>2</td>
<td>Ticari</td>
</tr>
</table>


### Sigorta Şirketleri

**Link:**"http://localhost/ada/TeklifSabitleri.SigortaSirketleri.aaws"

##### Örnek İstek:
<pre>
[]
</pre>

##### **Örnek Cevap:**
<pre>
[
    {
        "Metin": "AIG SİGORTA A.Ş.",
        "Deger": "005"
    },
    {
        "Metin": "AKDENİZ SİGORTA A.Ş.",
        "Deger": "024"
    },
    {
        "Metin": "AKSİGORTA A.Ş.",
        "Deger": "004"
    },
  ...
]
</pre>

### Tüm iller

**Link:**"http://localhost/ada/TeklifSabitleri.TumIller.aaws"

##### Örnek İstek:
<pre>
[]
</pre>

##### **Örnek Cevap:**
<pre>
[
  {"Id":0,"IlKodu":"1","IlceKodu":null,"BeldeKodu":null,"IlAdi":"ADANA","IlceAdi":null,"BeldeAdi":null},
  {"Id":0,"IlKodu":"2","IlceKodu":null,"BeldeKodu":null,"IlAdi":"ADIYAMAN","IlceAdi":null,"BeldeAdi":null},
  {"Id":0,"IlKodu":"3","IlceKodu":null,"BeldeKodu":null,"IlAdi":"AFYON KARAHİSAR","IlceAdi":null,"BeldeAdi":null},
  {"Id":0,"IlKodu":"4","IlceKodu":null,"BeldeKodu":null,"IlAdi":"AĞRI","IlceAdi":null,"BeldeAdi":null},
  ...
]
</pre>

### İlin İlçeleri

**Link:**"http://localhost/ada/TeklifSabitleri.TumIlceler.aaws"

##### Örnek İstek:
<pre>
[1]
</pre>

##### **Örnek Cevap:**
<pre>
[
    {
        "Id": 399963,
        "IlKodu": "1",
        "IlceKodu": "2",
        "BeldeKodu": "1832",
        "IlAdi": "ADANA",
        "IlceAdi": "ALADAĞ",
        "BeldeAdi": "AKÖREN"
    },
    {
        "Id": 399962,
        "IlKodu": "1",
        "IlceKodu": "2",
        "BeldeKodu": "2",
        "IlAdi": "ADANA",
        "IlceAdi": "ALADAĞ",
        "BeldeAdi": "ALADAĞ"
    },
  ...
]
</pre>


### Ülkeler

**Link:**"http://localhost/ada/TeklifSabitleri.TumUlkeler.aaws"

##### Örnek İstek:
<pre>
[]
</pre>

##### **Örnek Cevap:**
<pre>
[
	{
		"Id": 1,
		"No": 4,
		"Kod": "AF",
		"Ad": "Afganistan"
	},
	{
		"Id": 2,
		"No": 248,
		"Kod": "AX",
		"Ad": "Aland Adaları"
	},
	{
		"Id": 3,
		"No": 276,
		"Kod": "DE",
		"Ad": "Almanya"
	},
  ...
]
</pre>
