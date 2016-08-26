###DisTeklifAl


Teklif için girilmesi gereken ek bilgiler teklif alanlarında gönderilmelidir. Ek Bilgi ayrıntılarına 2-Teklif-Sirket-Ek-Bilgilerinin-Alinmasi dokümanından ulaşabilirsiniz.
Eğer şirket bazlı olarak Tüm ekbilgilerin bir profile bağlı gitmesini istiyorsanız  "ekbilgiProfil_{{ŞirketKodu}}" Metini için Değeri o profilin adı olarak tanımlamalısınız.
Profilden farklı olarak bir ek Bilgi değeri tanımlama istiyorsanız alanlara "eb~{{ŞirketKodu}}~{{ekBilgiId}}" şeklinde tanımlayabilirsiniz.
eğer iki türlüde tanımlama yapmazsanız sistem bu alanlara herhangi bir şekilde mühahale etmeyecek ve sistemde default ne ise o olarak kalacaktır.

Bu servisi çağırdığınızda dönen Cevapta bulunan 
'Basarili' değeri true ise, 'SirketKodlari' alanında belirtilen kodlar için <b>hesalama işlemleri başlatılmış</b> demektir. 
Eğer 'Basarili' değeri false ise, yapılmış istek için herhangi bir <b>hesaplama işlemi yapılmayacaktır</b>. 
'Mesaj' ve 'Mesajlar' incelenerek ilgili veri girişi/düzeltme işlemlerinin yapılarak isteğin tekrarlanması gerekmektedir. Cevapta ki 'SirketKodlari' alanı gönderilmiş olan şirket Kodlarndan az olabilir. Bu durum yetkisiz şirketin kodunun gönderilmiş olmasından kaynaklanmaktadır.


Örnekte, Trafik teklifinin istek ve cevabı verilmiştir.

Cevap, Hesaplama sonuçlarını barındırmaz. Hesaplamalar yapılırken ve tamamlandığında gerekli bilgilerin Bu servisi çağıran sisteme aktarılması için o sistemde "AkiliTeklifMesajAlici" servisi tanımlamalısınız.
tanımlayacağınız servisi AAW sisteminde gerekli parametreyi ayarladığınızda; <b>Hesaplanmaya başlayan</b> tekliflerin  Mesaj, Soru ve Hesaplama sonuçları bu servis üzerinden size iletilecektir.
"AkiliTeklifMesajAlici" servisinin tanımlanması ile ilgili "AkiliTeklifMesajAlici" dokümanını inceleyebilirsiniz.

**Link:**"http://localhost/ada/AkilliTeklif.DisTeklifAl.aaws"

**Parametreler:** Teklif Alanları, İstek Gönderilecek Şirketler, Ekran Key

##### Örnek İstek:
<pre>
[
[{
	"Metin": "AracMotorNo",
	"Deger": "***********"
}, {
	"Metin": "KimlikNo",
	"Deger": "***********"
}, {
	"Metin": "EPosta",
	"Deger": "test@eposta.com"
}, {
	"Metin": "TelefonNo",
	"Deger": "5559998877"
}, {
	"Metin": "BagliPolice",
	"Deger": ""
}, {
	"Metin": "ManuelTaksit",
	"Deger": ""
}, {
	"Metin": "ZktmsPoliceNo",
	"Deger": ""
}, {
	"Metin": "ManuelBrutPrim",
	"Deger": ""
}, {
	"Metin": "BagliPoliceAciklama",
	"Deger": ""
}, {
	"Metin": "AracTescilSeriNo",
	"Deger": "******"
}, {
	"Metin": "IlceKodu",
	"Deger": "***"
}, {
	"Metin": "SorguKimlikNo",
	"Deger": ""
}, {
	"Metin": "UrunGrubu",
	"Deger": "Trafik"
}, {
	"Metin": "TescilTarihi",
	"Deger": "30.12.2010"
}, {
	"Metin": "OncekiPoliceAcenteNo",
	"Deger": "******"
}, {
	"Metin": "SorguPlakaIlKodu",
	"Deger": ""
}, {
	"Metin": "BeldeAdi",
	"Deger": "KONAK"
}, {
	"Metin": "MarkaAdi",
	"Deger": "HYUNDAI"
}, {
	"Metin": "SorguAracTescilKodu",
	"Deger": ""
}, {
	"Metin": "ManuelKomisyon",
	"Deger": ""
}, {
	"Metin": "BaslangicTarihi",
	"Deger": "30.12.2015"
}, {
	"Metin": "Policelesti",
	"Deger": 0
}, {
	"Metin": "OncekiPoliceYenilemeNo",
	"Deger": "0"
}, {
	"Metin": "ZktmsYenilemeNo",
	"Deger": ""
}, {
	"Metin": "OncekiPolicePoliceNo",
	"Deger": "*********"
}, {
	"Metin": "PlakaNo",
	"Deger": "******"
}, {
	"Metin": "ZktmsAcenteKodu",
	"Deger": ""
}, {
	"Metin": "OncekiPoliceSirketKodu",
	"Deger": "007"
}, {
	"Metin": "KullanimSekli",
	"Deger": "0"
}, {
	"Metin": "AracSasiNo",
	"Deger": "*****************"
}, {
	"Metin": "PlakaIlKodu",
	"Deger": "35"
}, {
	"Metin": "IlKodu",
	"Deger": "35"
}, {
	"Metin": "ManuelSirketKodu",
	"Deger": ""
}, {
	"Metin": "BitisTarihi",
	"Deger": "30.12.2016"
}, {
	"Metin": "TipAdi",
	"Deger": "GETZ 1.4"
}, {
	"Metin": "IlAdi",
	"Deger": "İZMİR"
}, {
	"Metin": "ModelYili",
	"Deger": "2008"
}, {
	"Metin": "Manuel",
	"Deger": ""
}, {
	"Metin": "Ad",
	"Deger": "JALE"
}, {
	"Metin": "BeldeKodu",
	"Deger": "871"
}, {
	"Metin": "KullanimTarzi",
	"Deger": "01"
}, {
	"Metin": "TeklifId",
	"Deger": "3352"
}, {
	"Metin": "SorguPlakaNo",
	"Deger": ""
}, {
	"Metin": "Soyad",
	"Deger": "ERKAMAN"
}, {
	"Metin": "sorumlu",
	"Deger": " "
}, {
	"Metin": "satici",
	"Deger": " "
}, {
	"Metin": "AracKodu",
	"Deger": "177180"
}, {
	"Metin": "sorumluPrk",
	"Deger": ""
}, {
	"Metin": "saticiPrk",
	"Deger": ""
}, {
	"Metin": "IlceAdi",
	"Deger": "KONAK"
}, {
	"Metin": "KullaniciId",
	"Deger": "1"
}, {
	"Metin": "taliAcentePrk",
	"Deger": ""
}, {
	"Metin": "TrafigeCikisTarihi",
	"Deger": "01.01.2008"
}, {
	"Metin": "taliAcente",
	"Deger": ""
}, {
	"Metin": "SorguAracTescilSeriNo",
	"Deger": ""
}, {
	"Metin": "ZktmsSirketKodu",
	"Deger": ""
}, {
	"Metin": "AracTescilKodu",
	"Deger": "**"
}, {
	"Metin": "ekbilgiProfil_004",
	"Deger": "En Son Kullanılmış Olan Ek Bilgiler"
}, {
	"Metin": "eb~004~detayliTramerSorgusuYap",
	"Deger": "1"
}], ["004", "045"], "4dec50dc-42a0-48ec-80a8-4322ccaf059c"]
</pre>

##### **Örnek Cevap:**
<pre>
{
	"SirketKodlari": ["004", "045"],
	"OncekiCevaplar": [],
	"TeklifId": 3352,
	"Mesaj": "",
	"Basarili": true,
	"Tipi": 0,
	"Mesajlar": [],
	"Obj": null
}
</pre>
