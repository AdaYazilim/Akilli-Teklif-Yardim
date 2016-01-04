<h3>AkiliTeklifMesajAlici</h3>
DisTeklifAl servisini kullananların sistemlerinde tanımlaması gereken servistir. 
Bu doküman başlatılan Teklif isteğinin bildirimlerini dış sisteme aktaran servisin özelliklerini tanımlar. 

<h5>Hazırlanması Gereken Servis</h5>
<pre>
&lt;soapenv:Envelope xmlns:soapenv=&quot;http://schemas.xmlsoap.org/soap/envelope/&quot; xmlns:tem=&quot;http://tempuri.org/&quot;&gt;
   &lt;soapenv:Header/&gt;
   &lt;soapenv:Body&gt;
      &lt;tem:AkiliTeklifMesajAlici&gt;
         &lt;!--Optional:--&gt;
         &lt;tem:ekranKey&gt;?&lt;/tem:ekranKey&gt;
         &lt;!--Optional:--&gt;
         &lt;tem:fonksiyon&gt;?&lt;/tem:fonksiyon&gt;
         &lt;!--Optional:--&gt;
         &lt;tem:parametreler&gt;
            &lt;!--Zero or more repetitions:--&gt;
            &lt;tem:string&gt;?&lt;/tem:string&gt;
         &lt;/tem:parametreler&gt;
      &lt;/tem:AkiliTeklifMesajAlici&gt;
   &lt;/soapenv:Body&gt;
&lt;/soapenv:Envelope&gt;
</pre>

*Parametreler html encoding işlemi yapılarak gönderilir.

<h6>Gelebilecek Fonksiyon ve Parametreler</h6>
<table>
  <thead>
    <tr>
      <th>fonksiyon</th>
      <th>parametreler</th>
      <th>Açıklama</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>sunucuyaIstekGonderildi</td>
      <td>sirketKodu, ekranKey</td>
      <td>isteğin işlemciye iletildiğini bildirir</td>
    </tr>
    <tr>
      <td>sunucuyaIstekGonderilmedi</td>
      <td>sirketKodu, ekranKey</td>
      <td>isteğin işlemciye iletilemediğini bildirir</td>
    </tr>
    <tr>
      <td>adaBotMesajGeldi</td>
      <td>sirketKodu, ekranKey, mesaj</td>
      <td>Teklif hesaplamasının durumu hakkında bilgi verir/ Kullanıcıya sorulan sorular html olarak bu fonksiyonla gelir. Cevap gönderimi için "DisArkaPlanCevapEkle" servisi kullanılabilinir.</td>
    </tr>
    <tr>
      <td>donenCevapIsle</td>
      <td>sirketKodu, ekranKey, donenPoliceJson</td>
      <td>Hesaplama Sonucu bu fonksiyon ile gelir. Hesaplama sonuç nesnesi Json formatında parametre olarak gelir.</td>
    </tr>
  </tbody>
<table>

