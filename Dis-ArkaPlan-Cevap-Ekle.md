<h3>DisArkaPlanCevapEkle</h3>
"AkiliTeklifMesajAlici" Servisinize gelen "adaBotMesajGeldi" fonksiyonunu ile size gelen soruya göndermeniz gereken cevap için bu servisi kullanabilirsiniz.

"AkiliTeklifMesajAlici" servisinden gelen örnek soru isteği;
<pre>
&lt;soapenv:Envelope xmlns:soapenv=&quot;http://schemas.xmlsoap.org/soap/envelope/&quot; xmlns:tem=&quot;http://tempuri.org/&quot;&gt;
    &lt;soapenv:Header/&gt;
    &lt;soapenv:Body&gt;
        &lt;tem:AkiliTeklifMesajAlici&gt;
            &lt;tem:ekranKey&gt;14596fe1-cf7a-4675-aa90-25341f8d0577&lt;/tem:ekranKey&gt;
            &lt;tem:fonksiyon&gt;adaBotMesajGeldi&lt;/tem:fonksiyon&gt;
            &lt;tem:parametreler&gt;
                &lt;tem:string&gt;040&lt;/tem:string&gt;
                &lt;tem:string&gt;14596fe1-cf7a-4675-aa90-25341f8d0577&lt;/tem:string&gt;
                &lt;tem:string&gt;&amp;lt;div GelenSoruDiv=&amp;#39;14596fe1-cf7a-4675-aa90-25341f8d0577&amp;#39; &amp;gt;&amp;lt;img height=&amp;#39;150px&amp;#39; tmpMesaj=&amp;#39;captcha bekle&amp;#39; src=&amp;#39;GeciciDosyalar/Captcha/captcha__0000049415_471.jpg&amp;#39; /&amp;gt;Giriniz...&amp;lt;br/&amp;gt;&amp;lt;input type=&amp;#39;text&amp;#39; id=&amp;#39;txtBeklenenCevap_040&amp;#39; onkeyup=&amp;#39;Enter(event,captchaCevapla);&amp;#39; /&amp;gt;&amp;lt;input type=&amp;#39;button&amp;#39; value=&amp;#39;G&amp;#246;nder&amp;#39; onclick=&amp;#39;DisArkaPlanCevapEkle(&amp;quot;040&amp;quot;,&amp;quot;14596fe1-cf7a-4675-aa90-25341f8d0577&amp;quot;,&amp;quot;txtBeklenenCevap_040&amp;quot;, &amp;quot;e9300c23-eb41-46ec-a748-e6f4569ecf67&amp;quot;);&amp;#39; /&amp;gt;&amp;lt;/div&amp;gt;&lt;/tem:string&gt;
            &lt;/tem:parametreler&gt;
        &lt;/tem:AkiliTeklifMesajAlici&gt;
    &lt;/soapenv:Body&gt;
&lt;/soapenv:Envelope&gt;
</pre>

DisArkaPlanCevapEkle("040","14596fe1-cf7a-4675-aa90-25341f8d0577","txtBeklenenCevap_040", "e9300c23-eb41-46ec-a748-e6f4569ecf67");
**Link:**"http://localhost/ada/AkilliTeklif.DisArkaPlanCevapEkle.aaws"

**Parametreler:** cevap, uniqueId, ekranKey, sirketKodu, urunGrubu bilgieri gönderilir(Bu değerler size gelmiş olan soru htmlinde bulunmaktadır.)

<h5>Örnek İstek:</h5>
<pre>
  [$("#" + "txtBeklenenCevap_040").val(), "e9300c23-eb41-46ec-a748-e6f4569ecf67", "14596fe1-cf7a-4675-aa90-25341f8d0577", "040", "Trafik"]
</pre>

<h5> **Örnek Cevap:**</h5>
<pre>
{}
</pre>
