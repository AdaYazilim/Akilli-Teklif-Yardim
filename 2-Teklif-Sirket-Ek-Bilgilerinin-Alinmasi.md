###TeklifiAlYeniTeklif

Ürün grubu bazında bazı sabit ayarları döndüren servistir.
Örnekte "Trafik" ürün Grubu için örnek istek yapılmış ve sistemde kayıtlı olunan Bir şirket için tanımlı ek bilgileri ve profillerdeki tanımlı ekbilgi ayarlamalarını getirdi.

**Link:**"http://localhost/ada/AkilliTeklif.TeklifiAlYeniTeklif.aaws"

**Parametreler:** Ürün Grubu bilgisi

##### Örnek İstek:

["Trafik"]

##### **Örnek Cevap:**
<pre>
{
    "Nesne": {
        "SirketBilgileri": [{
            "EkBilgiProfilleri": [{
                "EkBilgiler": [{
                    "Degerler": [{
                        "Metin": "Nakit",
                        "Deger": "1"
                    }, {
                        "Metin": "Taksitli",
                        "Deger": "2"
                    }],
                    "Deger": "1",
                    "Kosul": "",
                    "Id": "OdemeTipi",
                    "Aciklama": "Ödeme Tipi?",
                    "Kategori": {
                        "Ad": "GENEL",
                        "Aciklama": "Genel"
                    },
                    "Tip": "Select"
                }, {
                    "Degerler": [{
                        "Metin": "Trafik Sigortası Yeni",
                        "Deger": "0"
                    }, {
                        "Metin": "TrabzonSpor Trafik",
                        "Deger": "1"
                    }, {
                        "Metin": "SivasSpor Trafik",
                        "Deger": "2"
                    }, {
                        "Metin": "BeşiktAŞK Trafik",
                        "Deger": "3"
                    }],
                    "Deger": "3",
                    "Kosul": "",
                    "Id": "Tarife",
                    "Aciklama": "Tarife?",
                    "Kategori": {
                        "Ad": "GENEL",
                        "Aciklama": "Genel"
                    },
                    "Tip": "Select"
                }, {
                    "Degerler": [{
                        "Metin": "Hususi",
                        "Deger": "Hususi"
                    }, {
                        "Metin": "Ticari",
                        "Deger": "Ticari"
                    }, {
                        "Metin": "Resmi",
                        "Deger": "Resmi"
                    }],
                    "Deger": "Hususi",
                    "Kosul": "",
                    "Id": "KullanimAmaci",
                    "Aciklama": "Kullanım Amacı?",
                    "Kategori": {
                        "Ad": "GENEL",
                        "Aciklama": "Genel"
                    },
                    "Tip": "Select"
                }],
                "Ad": "Boş Profil"
            }],
            "Kod": "507",
            "Ad": "ANADOLU ANONİM TÜRK SİGORTA ŞİRKETİ",
            "Offline": false,
            "Uzak": false,
            "PolicelestirmeVar": false
        }],
        "Teklif": {
            "donenPolicelerdeAlinsin": true,
            "Alanlar": {
                "BaslangicTarihi": {
                    "Soru": "BaslangicTarihi",
                    "Cevap": "31.12.2015"
                },
                "BitisTarihi": {
                    "Soru": "BitisTarihi",
                    "Cevap": "31.12.2016"
                },
                "KullaniciId": {
                    "Soru": "KullaniciId",
                    "Cevap": "1"
                },
                "UrunGrubu": {
                    "Soru": "UrunGrubu",
                    "Cevap": "Trafik"
                }
            },
            "DonenPoliceler": [],
            "UrunGrubu": "Trafik",
            "TeklifId": 0,
            "TeklifIdString": ""
        },
        "KomisyonGormeYetkisiVar": true
    },
    "Basarili": true,
    "Mesaj": ""
}
</pre>
