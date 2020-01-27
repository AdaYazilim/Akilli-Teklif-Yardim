### SirketTanimBilgileriniAl

Ürün grubu bazında bazı sabit ayarları döndüren servistir.
Örnekte "Trafik" ürün Grubu için örnek istek yapılmış ve sistemde kayıtlı olunan Bir şirket için tanımlı ek bilgileri ve profillerdeki tanımlı ekbilgi ayarlamalarını getirdi.

<pre>
Ek bilgilerin Teklif alımında Anahtar Kelimeleri oluştururken;
"eb~{{ŞirketKodu}}~{{KategoriAd}}~{{ekBilgiId}}" veya "eb~{{ŞirketKodu}}~{{ekBilgiId}}"
formülü kullanılabilir.
</pre>

**Link:** "http://localhost/ada/AkilliTeklif.SirketTanimBilgileriniAl.aaws"

**Parametreler:** Ürün Grubu bilgisi

##### Örnek İstek:

["Trafik"]

##### **Örnek Cevap:**
<pre>
{
    [
        {
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
        }
    ]
}
</pre>

### SirketinSirketTanimBilgileriniAl

Ürün grubu ve şirket bazında bazı sabit ayarları döndüren servistir.
Örnekte "Trafik" ürün Grubu ve bir şirket için istek yapılmış ve sistemde kayıtlı olunan Bir şirket için tanımlı ek bilgileri ve profillerdeki tanımlı ekbilgi ayarlamalarını getirdi.

<pre>
Ek bilgilerin Teklif alımında Anahtar Kelimeleri oluştururken;
"eb~{{ŞirketKodu}}~{{KategoriAd}}~{{ekBilgiId}}" veya "eb~{{ŞirketKodu}}~{{ekBilgiId}}"
formülü kullanılabilir.
</pre>

**Link:** "http://localhost/ada/AkilliTeklif.SirketinSirketTanimBilgileriniAl.aaws"

**Parametreler:** Ürün Grubu bilgisi, Şirket Kodu Bilgisi

##### Örnek İstek:

["Trafik", "507"]

##### **Örnek Cevap:**
<pre>
{
    [
        {
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
        }
    ]
}
</pre>


### TeklifinSonKullanilanEkBilgileri

Bir teklifde, şirket için kullanılmş son ekbilgilerin olduğu ekbilgi profilini döndüren servistir.

<pre>
Ek bilgilerin Teklif alımında Anahtar Kelimeleri oluştururken;
"eb~{{ŞirketKodu}}~{{KategoriAd}}~{{ekBilgiId}}" veya "eb~{{ŞirketKodu}}~{{ekBilgiId}}"
formülü kullanılabilir.
</pre>

**Link:** "http://localhost/ada/AkilliTeklif.TeklifinSonKullanilanEkBilgileri.aaws"

**Parametreler:**  TeklifId ve ŞirketKodu

##### Örnek İstek:

[160,'054']

##### **Örnek Cevap:**
<pre>
{
    "Nesne": {
        "EkBilgiler": [
            {
                "Degerler": [
                    {
                        "Metin": "Değiştirme",
                        "Deger": ""
                    },
                    {
                        "Metin": "Peşin",
                        "Deger": "P"
                    },
                    {
                        "Metin": "Vadeli",
                        "Deger": "V"
                    }
                ],
                "Ozellikler": [],
                "Deger": "P",
                "Kosul": "",
                "Id": "OdemeSekli",
                "Aciklama": "Ödeme Tipi",
                "Kategori": {
                    "Ad": "OdemeBilgileri",
                    "Aciklama": "Ödeme Bilgileri"
                },
                "Tip": "Select"
            },
            ...
        ],
        "Ad": "En Son Kullanılmış Olan Ek Bilgiler"
    },
    "Basarili": true,
    "Mesaj": ""
}
</pre>

