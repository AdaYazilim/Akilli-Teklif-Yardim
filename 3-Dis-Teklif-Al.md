### Genel Mimari
Teklif için girilmesi gereken ek bilgiler teklif alanlarında gönderilmelidir. Ek Bilgi ayrıntılarına 2-Teklif-Sirket-Ek-Bilgilerinin-Alinmasi dokümanından ulaşabilirsiniz.
Eğer şirket bazlı olarak Tüm ekbilgilerin bir profile bağlı gitmesini istiyorsanız  "ekbilgiProfil_{{ŞirketKodu}}" Metini için Değeri o profilin adı olarak tanımlamalısınız.
Profilden farklı olarak bir ek Bilgi değeri tanımlama istiyorsanız alanlara "eb~{{ŞirketKodu}}~{{ekBilgiId}}" şeklinde tanımlayabilirsiniz.
eğer iki türlüde tanımlama yapmazsanız sistem bu alanlara herhangi bir şekilde mühahale etmeyecek ve sistemde default ne ise o olarak kalacaktır.

Bu servisi çağırdığınızda dönen Cevapta bulunan 
'Basarili' değeri true ise, 'SirketKodlari' alanında belirtilen kodlar için <b>hesalama işlemleri başlatılmış</b> demektir. 
Eğer 'Basarili' değeri false ise, yapılmış istek için herhangi bir <b>hesaplama işlemi yapılmayacaktır</b>. 
'Mesaj' ve 'Mesajlar' incelenerek ilgili veri girişi/düzeltme işlemlerinin yapılarak isteğin tekrarlanması gerekmektedir. Cevapta ki 'SirketKodlari' alanı gönderilmiş olan şirket Kodlarndan az olabilir. Bu durum yetkisiz şirketin kodunun gönderilmiş olmasından kaynaklanmaktadır.

Cevap, Hesaplama sonuçlarını barındırmaz. Hesaplamalar yapılırken ve tamamlandığında gerekli bilgilerin Bu servisi çağıran sisteme aktarılması için o sistemde "AkiliTeklifMesajAlici" servisi tanımlamalısınız.
tanımlayacağınız servisi AAW sisteminde gerekli parametreyi ayarladığınızda; <b>Hesaplanmaya başlayan</b> tekliflerin  Mesaj, Soru ve Hesaplama sonuçları bu servis üzerinden size iletilecektir.
"AkiliTeklifMesajAlici" servisinin tanımlanması ile ilgili "AkiliTeklifMesajAlici" dokümanını inceleyebilirsiniz.



### DisTeklifAlV2

**Link:**"http://localhost/ada/AkilliTeklif.DisTeklifAlV2.aaws"

**Parametreler:** Teklif Bilgileri, İstek Gönderilecek Şirketler, Ekran Key

**Header Parametreleri;**
Dönüş bilgilerini alacağınız "AkilliTeklifMesajAlici" servisinin linkini adayazılıma doğrudan tanımlatabileceğiniz gibi;
servis isteğine "ServisLink" ve "ServisSoapAction" keyli HttpHeaderlar olarakta ekleyebilirsiniz.

Teklif Bilgileri yapısı;
<pre>
       List<MetinDeger> Alanlar// kullanılabilecek alan listesi için; "DisTeklifAlV2_Yardim" servisini inceleyebilirsiniz.
       List<TeklifSigortali> Sigortalilar// nesne yapısı için; "DisTeklifAlV2_Yardim" servisini inceleyebilirsiniz.
</pre>

##### Örnek İstek:
<pre>
[
	{
		"Alanlar": [{
			"Metin": "UrunGrubu",
			"Deger": "Trafik"
		}, {
			"Metin": "KimlikNo",
			"Deger": "1111111111"
		}, {
			"Metin": "PlakaIlKodu",
			"Deger": "45"
		}, {
			"Metin": "PlakaNo",
			"Deger": "KT54627"
		}, {
			"Metin": "AracTescilKodu",
			"Deger": "AB"
		}, {
			"Metin": "AracTescilSeriNo",
			"Deger": "123456"
		}, {
			"Metin": "ekbilgiProfil_540",
			"Deger": "Otomatik"
		}, {
			"Metin": "eb~540~detayliTramerSorgusuYap",
			"Deger": "1"
		}],
		"Sigortalilar":[]// nesne yapısı için; "DisTeklifAlV2_Yardim" servisini inceleyebilirsiniz.
	}
, ["540","045"], "4dec50dc-42a0-48ec-80a8-4322ccaf059c"]

</pre>

##### **Örnek Cevap:**
<pre>
{
	"SirketKodlari": ["540", "045"],
	"OncekiCevaplar": [],
	"TeklifId": 3352,
	"Mesaj": "",
	"Basarili": true,
	"Tipi": 0,
	"Mesajlar": [],
	"Obj": null
}
</pre>




### DisTeklifAl

Yalnızca teklif bilgillerini gönderebilirsiniz. Ek sigortalı tanımlması yapmanız gerekiyorsa "DisTeklifAlV2" servisini kullanınız.

Örnekte, Trafik teklifinin istek ve cevabı verilmiştir.


**Link:**"http://localhost/ada/AkilliTeklif.DisTeklifAl.aaws"

**Parametreler:** Teklif Alanları, İstek Gönderilecek Şirketler, Ekran Key

##### Örnek İstek:
<pre>

[
	{
		"Alanlar": [{
			"Metin": "UrunGrubu",
			"Deger": "Trafik"
		}, {
			"Metin": "KimlikNo",
			"Deger": "1111111111"
		}, {
			"Metin": "PlakaIlKodu",
			"Deger": "45"
		}, {
			"Metin": "PlakaNo",
			"Deger": "KT54627"
		}, {
			"Metin": "AracTescilKodu",
			"Deger": "AB"
		}, {
			"Metin": "AracTescilSeriNo",
			"Deger": "123456"
		}, {
			"Metin": "ekbilgiProfil_540",
			"Deger": "Otomatik"
		}, {
			"Metin": "eb~540~detayliTramerSorgusuYap",
			"Deger": "1"
		}]
	}
, ["540","045"], "4dec50dc-42a0-48ec-80a8-4322ccaf059c"]

</pre>

##### **Örnek Cevap:**
<pre>
{
	"SirketKodlari": ["540", "045"],
	"OncekiCevaplar": [],
	"TeklifId": 3352,
	"Mesaj": "",
	"Basarili": true,
	"Tipi": 0,
	"Mesajlar": [],
	"Obj": null
}
</pre>
