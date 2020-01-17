<template>
  <div class="jumbotron jumbotron-fluid" style="padding: 0.5em; background-image: url(teren.jpg); background-repeat:no-repeat; background-size:90%; height: 900px; background-position: left">
    <h1 class="display-2" style="font-family:Cuprum; text-align:center; margin-right:100px; color: black; font-size:90px;"><b>{{ myteam }} </b>
    </h1>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:793px;">
  <img id="fw1" src="playertemplate.png" style="position: absolute;">
   <select id="selectfw1" v-on:change="counterfw1(); showButton(); bodovifw1();" onchange="document.getElementById('fw1').src = this.value;" style="font-size:20px; position:absolute; left:826px; width:284px;">
    <option value="playertemplate.png">Odaberite Napadača</option>
    <option value="bpetkovic.png">Bruno Petković (Dinamo Zagreb)</option>
    <option value="mgavranovic.png">Mario Gavranović (Dinamo Zagreb)</option>
    <option value="skulenovic.png">Sandro Kulenović (Dinamo Zagreb)</option>
    <option value="kandric.png">Komnen Andrić (Dinamo Zagreb)</option>
    <option value="rbaturina.png">Roko Baturina (Dinamo Zagreb)</option>
    <option value="lsipos.png">Leon Šipoš (Dinamo Zagreb)</option>
    <option value="mjakolis.png">Marin Jakoliš (Hajduk Split)</option>
    <option value="mdelic.png">Ivan Delić (Hajduk Split)</option>
    <option value="lkrekovic.png">Leon Kreković (Hajduk Split)</option>
    <option value="amcolak.png">Antonio-Mirko Čolak (Rijeka)</option>
    <option value="jpuljic.png">Jakov Puljić (Rijeka)</option>
    <option value="mbabic.png">Matko Babić (Rijeka)</option>
    <option value="mmatulja.png">Matija Matulja (Rijeka)</option>
    <option value="mmaric.png">Mirko Marić (Osijek)</option>
    <option value="amance.png">Antonio Mance (Osijek)</option>
    <option value="jmbakogu.png">Jerry Mbakogu (Osijek)</option>
    <option value="jspoljaric.png">Josip Špoljarić (Osijek)</option>
    <option value="ddrenabeljo.png">Dion Drena Beljo (Osijek)</option>
    <option value="cndiaye.png">Cherif Ndiaye (Gorica)</option>
    <option value="lzwolinski.png">Lukasz Zwolinski (Gorica)</option>
    <option value="mbudimir.png">Mario Budimir (Lokomotiva Zagreb)</option>
    <option value="ituci.png">Indrit Tuci (Lokomotiva Zagreb)</option>
    <option value="lmaruzin.png">Loren Maružin (Lokomotiva Zagreb)</option>
    <option value="mdelic.png">Mateas Delić (Slaven Belupo)</option>
    <option value="mmladen.png">Mihael Mladen (Slaven Belupo)</option>
    <option value="fetoundi.png">Franck Etoundi (Slaven Belupo)</option>
    <option value="mateus.png">Mateus (Slaven Belupo)</option>
    <option value="ikrstanovic.png">Ivan Krstanović (Slaven Belupo)</option>
    <option value="akaluderovic.png">Andrija Kaluđerović (Inter Zaprešić)</option>
    <option value="imamut.png">Ivan Mamut (Inter Zaprešić)</option>
    <option value="mvasilj.png">Mario Vasilj (Inter Zaprešić)</option>
    <option value="wtchuameni.png">William Tchuameni (Inter Zaprešić)</option>
    <option value="bbilobrk.png">Borna Bilobrk (Inter Zaprešić)</option>
    <option value="mbencic.png">Mihael Benčić (Inter Zaprešić)</option>
    <option value="mcuze.png">Mario Ćuže (Istra 1961)</option>
    <option value="klaukzemis.png">Karolis Laukžemis (Istra 1961)</option>
    <option value="rperickomsic">Robert Perić-Komšić (Istra 1961)</option>
    <option value="afuentes.png">Adrian Fuentes (Istra 1961)</option>
    <option value="vlisakovich.png">Vitali Lisakovich (Varaždin)</option>
    <option value="lbenko.png">Leon Benko (Varaždin)</option>
    <option value="dglavina.png">Dominik Glavina (Varaždin)</option>
    <option value="vlisakovich.png">Vitali Lisakovich (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:500px;">
  <img id="fw2" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectfw2" v-on:change="counterfw2(); showButton(); bodovifw2();" onchange="document.getElementById('fw2').src = this.value" style="font-size:20px; position:absolute; left:1119px; top:27px; width:284px;">
    <option value="playertemplate.png">Odaberite Lijevo Krilo</option>
    <option value="morsic.png">Mislav Oršić (Dinamo Zagreb)</option>
    <option value="iatiemwen.png">Iyayi Atiemwen (Dinamo Zagreb)</option>
    <option value="amarin.png">Antonio Marin (Dinamo Zagreb)</option>
    <option value="jairo.png">Jairo da Silva (Hajduk Split)</option>
    <option value="idolcek.png">Ivan Dolček (Hajduk Split)</option>
    <option value="agorgon.png">Alexander Gorgon (Rijeka)</option>
    <option value="mvuk.png">Matej Vuk (Rijeka)</option>
    <option value="pbockaj.png">Petar Bočkaj (Osijek)</option>
    <option value="mndockyt.png">Merveil Ndockyt (Osijek)</option>
    <option value="mpilj.png">Marin Pilj (Osijek)</option>
    <option value="klovric.png">Kristijan Lovrić (Gorica)</option>
    <option value="msroler.png">Martin Šroler (Gorica)</option>
    <option value="muzuni.png">Myrto Uzuni (Lokomotiva Zagreb)</option>
    <option value="ddrozdek.png">Domagoj Drožđek (Lokomotiva Zagreb)</option>
    <option value="jmajic.png">Josip Majić (Lokomotiva Zagreb)</option>
    <option value="sserderov.png">Serder Serderov (Inter Zaprešić)</option>
    <option value="dbusnja.png">Denis Bušnja (Istra 1961)</option>
    <option value="jmaganjic.png">Josip Maganjić (Istra 1961)</option>
    <option value="lvuk.png">Leonard Vuk (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:1085px;">
  <img id="fw3" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectfw3" v-on:change="counterfw3(); showButton(); bodovifw3();" onchange="document.getElementById('fw3').src = this.value" style="font-size:20px; position:absolute; left:534px; top:54px; width:284px;">
    <option value="playertemplate.png">Odaberite Desno Krilo</option>
    <option value="dkadzior.png">Damian Kadzior (Dinamo Zagreb)</option>
    <option value="ihajrovic.png">Izet Hajrović (Dinamo Zagreb)</option>
    <option value="seduok.png">Samuel Eduok (Hajduk Split)</option>
    <option value="ftahiraj.png">Francesco Tahiraj (Hajduk Split)</option>
    <option value="macosty.png">Maxwell Acosty (Rijeka)</option>
    <option value="rmuric.png">Robert Murić (Rijeka)</option>
    <option value="egrezda.png">Eros Grezda (Osijek)</option>
    <option value="jmathieu.png">Justin Mathieu (Gorica)</option>
    <option value="mdvornekovic.png">Matija Dvorneković (Gorica)</option>
    <option value="lkastrati.png">Lirim Kastrati (Lokomotiva Zagreb)</option>
    <option value="edeocleciano.png">Emerson Deocleciano (Lokomotiva Zagreb)</option>
    <option value="bbogojevic.png">Bruno Bogojević (Slaven Belupo)</option>
    <option value="falidema.png">Festim Alidema (Slaven Belupo)</option>
    <option value="jmitrovic.png">Josip Mitrović (Inter Zaprešić)</option>
    <option value="sgrzan.png">Šime Gržan (Istra 1961)</option>
    <option value="mmunivrana.png">Mario Munivrana (Istra 1961)</option>
    <option value="asane.png">Arona Sane (Istra 1961)</option>
    <option value="mmehdikani.png">Mehdi Mehdikani (Varaždin)</option>
    <option value="tturcin.png">Tomislav Turčin (Varaždin)</option>
    <option value="mkolaric.png">Matija Kolarić (Varaždin)</option>
    <option value="nhavelka.png">Niko Havelka (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:520px; top:370px;">
  <img id="mf1" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectmf1" v-on:change="countermf1(); showButton(); bodovimf1();" onchange="document.getElementById('mf1').src = this.value" style="font-size:20px; position:absolute; left:1099px; bottom:32px; width:284px;">
    <option value="playertemplate.png">Odaberite Veznjaka</option>
    <option value="dolmo.png">Dani Olmo (Dinamo Zagreb)</option>
    <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
    <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
    <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
    <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
    <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
    <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
    <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
    <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
    <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
    <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
    <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
    <option value="fbradarić.png">Filip Bradarić (Hajduk Split)</option>
    <option value="dnejasmic.png">Darko Nejašmić (Hajduk Split)</option>
    <option value="sjuric.png">Stanko Jurić (Hajduk Split)</option>
    <option value="akalik.png">Anthony Kalik (Hajduk Split)</option>
    <option value="fandrijasevic.png">Franko Andrijašević (Rijeka)</option>
    <option value="thalilovic.png">Tibor Halilović (Rijeka)</option>
    <option value="diglesias.png">Dani Iglesias (Rijeka)</option>
    <option value="dpavicic.png">Domagoj Pavičić (Rijeka)</option>
    <option value="sloncar.png">Stjepan Lončar (Rijeka)</option>
    <option value="ilepinjica.png">Ivan Lepinjica (Rijeka)</option>
    <option value="lcapan.png">Luka Capan (Rijeka)</option>
    <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
    <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
    <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
    <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
    <option value="mzaper.png">Mihael Žaper (Osijek)</option>
    <option value="bmioc.png">Benedik Mioč (Osijek)</option>
    <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
    <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
    <option value="jsuk.png">Joey Suk (Gorica)</option>
    <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
    <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
    <option value="mmaloca.png">Martin Maloča (Gorica)</option>
    <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
    <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
    <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
    <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
    <option value="farezina.png">Filip Arezina (Lokomotiva Zagreb)</option>
    <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
    <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
    <option value="ecokaj.png">Enis Čokaj (Lokomotiva Zagreb)</option>
    <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
    <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
    <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
    <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
    <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
    <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
    <option value="ijajalo.png">Ivan Jajalo (Slaven Belupo)</option>
    <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
    <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
    <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
    <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
    <option value="jljubic.png">Juraj Ljubić (Inter Zaprešić)</option>
    <option value="robeng.png">Regan Obeng (Istra 1961)</option>
    <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
    <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
    <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
    <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
    <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
    <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
    <option value="tburic.png">Toni Burić (Istra 1961)</option>
    <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
    <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
    <option value="ktezak.png">Karlo Tezak (Varaždin)</option>
    <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
    <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
    <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
    <option value="iroca.png">Ivan Roca (Varaždin)</option>
    <option value="kfucak.png">Kristian Fucak (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:795px; top:380px;">
  <img id="mf2" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectmf2" v-on:change="countermf2(); showButton(); bodovimf2();" onchange="document.getElementById('mf2').src = this.value" style="font-size:20px; position:absolute; left:824px; bottom:15px; width:284px;">
    <option value="playertemplate.png">Odaberite Veznjaka</option>
    <option value="dolmo.png">Dani Olmo (Dinamo Zagreb)</option>
    <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
    <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
    <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
    <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
    <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
    <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
    <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
    <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
    <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
    <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
    <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
    <option value="fbradarić.png">Filip Bradarić (Hajduk Split)</option>
    <option value="dnejasmic.png">Darko Nejašmić (Hajduk Split)</option>
    <option value="sjuric.png">Stanko Jurić (Hajduk Split)</option>
    <option value="akalik.png">Anthony Kalik (Hajduk Split)</option>
    <option value="fandrijasevic.png">Franko Andrijašević (Rijeka)</option>
    <option value="thalilovic.png">Tibor Halilović (Rijeka)</option>
    <option value="diglesias.png">Dani Iglesias (Rijeka)</option>
    <option value="dpavicic.png">Domagoj Pavičić (Rijeka)</option>
    <option value="sloncar.png">Stjepan Lončar (Rijeka)</option>
    <option value="ilepinjica.png">Ivan Lepinjica (Rijeka)</option>
    <option value="lcapan.png">Luka Capan (Rijeka)</option>
    <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
    <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
    <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
    <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
    <option value="mzaper.png">Mihael Žaper (Osijek)</option>
    <option value="bmioc.png">Benedik Mioč (Osijek)</option>
    <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
    <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
    <option value="jsuk.png">Joey Suk (Gorica)</option>
    <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
    <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
    <option value="mmaloca.png">Martin Maloča (Gorica)</option>
    <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
    <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
    <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
    <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
    <option value="farezina.png">Filip Arezina (Lokomotiva Zagreb)</option>
    <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
    <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
    <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
    <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
    <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
    <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
    <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
    <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
    <option value="ijajalo.png">Ivan Jajalo (Slaven Belupo)</option>
    <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
    <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
    <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
    <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
    <option value="jljubic.png">Juraj Ljubić (Inter Zaprešić)</option>
    <option value="robeng.png">Regan Obeng (Istra 1961)</option>
    <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
    <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
    <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
    <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
    <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
    <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
    <option value="tburic.png">Toni Burić (Istra 1961)</option>
    <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
    <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
    <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
    <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
    <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
    <option value="iroca.png">Ivan Roca (Varaždin)</option>
    <option value="kfucak.png">Kristian Fucak (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:1075px; top:370px;">
  <img id="mf3" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectmf3" v-on:change="countermf3(); showButton(); bodovimf3();" onchange="document.getElementById('mf3').src = this.value" style="font-size:20px; position:absolute; left:544px; top:-5px; width:284px;">
    <option value="playertemplate.png">Odaberite Veznjaka</option>
    <option value="dolmo.png">Dani Olmo (Dinamo Zagreb)</option>
    <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
    <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
    <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
    <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
    <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
    <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
    <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
    <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
    <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
    <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
    <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
    <option value="fbradarić.png">Filip Bradarić (Hajduk Split)</option>
    <option value="dnejasmic.png">Darko Nejašmić (Hajduk Split)</option>
    <option value="sjuric.png">Stanko Jurić (Hajduk Split)</option>
    <option value="akalik.png">Anthony Kalik (Hajduk Split)</option>
    <option value="fandrijasevic.png">Franko Andrijašević (Rijeka)</option>
    <option value="thalilovic.png">Tibor Halilović (Rijeka)</option>
    <option value="diglesias.png">Dani Iglesias (Rijeka)</option>
    <option value="dpavicic.png">Domagoj Pavičić (Rijeka)</option>
    <option value="sloncar.png">Stjepan Lončar (Rijeka)</option>
    <option value="ilepinjica.png">Ivan Lepinjica (Rijeka)</option>
    <option value="lcapan.png">Luka Capan (Rijeka)</option>
    <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
    <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
    <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
    <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
    <option value="mzaper.png">Mihael Žaper (Osijek)</option>
    <option value="bmioc.png">Benedik Mioč (Osijek)</option>
    <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
    <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
    <option value="jsuk.png">Joey Suk (Gorica)</option>
    <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
    <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
    <option value="mmaloca.png">Martin Maloča (Gorica)</option>
    <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
    <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
    <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
    <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
    <option value="farezina.png">Filip Arezina (Lokomotiva Zagreb)</option>
    <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
    <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
    <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
    <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
    <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
    <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
    <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
    <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
    <option value="ijajalo.png">Ivan Jajalo (Slaven Belupo)</option>
    <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
    <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
    <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
    <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
    <option value="jljubic.png">Juraj Ljubić (Inter Zaprešić)</option>
    <option value="robeng.png">Regan Obeng (Istra 1961)</option>
    <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
    <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
    <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
    <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
    <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
    <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
    <option value="tburic.png">Toni Burić (Istra 1961)</option>
    <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
    <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
    <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
    <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
    <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
    <option value="iroca.png">Ivan Roca (Varaždin)</option>
    <option value="kfucak.png">Kristian Fucak (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:350px; top:535px;">
  <img id="df1" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectdf1" v-on:change="counterdf1(); showButton(); bodovidf1();" onchange="document.getElementById('df1').src = this.value" style="font-size:20px; position:absolute; left:1269px; top:-143px; width:284px;">
    <option value="playertemplate.png">Odaberite Lijevog Beka</option>
    <option value="fmoubandje.png">Francois Moubandje (Dinamo Zagreb)</option>
    <option value="mleovac.png">Marin Leovac (Dinamo Zagreb)</option>
    <option value="dcolina.png">David Čolina (Hajduk Split)</option>
    <option value="pmamic.png">Petar Mamić (Rijeka)</option>
    <option value="talys.png">Talys (Osijek)</option>
    <option value="lmarin.png">Luka Marin (Osijek)</option>
    <option value="mcabraja.png">Marijan Čabraja (Gorica)</option>
    <option value="mspicic.png">Matija Špičić (Gorica)</option>
    <option value="smarkovic.png">Stipo Marković (Lokomotiva Zagreb)</option>
    <option value="srozman.png">Siniša Rožman (Lokomotiva Zagreb)</option>
    <option value="bgoda.png">Bruno Goda (Slaven Belupo)</option>
    <option value="mradivojevic.png">Miloš Radivojević (Slaven Belupo)</option>
    <option value="svego.png">Stjepan Vego (Inter Zaprešić)</option>
    <option value="icelikovic.png">Ivan Čeliković (Inter Zaprešić)</option>
    <option value="mpavic.png">Markus Pavić (Istra 1961)</option>
    <option value="sgonzalez.png">Sergio Gonzalez (Istra 1961)</option>
    <option value="prubic.png">Petar Rubić (Istra 1961)</option>
    <option value="imilicevic.png">Ivan Miličević (Varaždin)</option>
    <option value="dstefulj.png">Daniel Štefulj (Varaždin)</option>
    <option value="ksambolec.png">Karlo Sambolec (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:630px; top:540px;">
  <img id="df2" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectdf2" v-on:change="counterdf2(); showButton(); bodovidf2();" onchange="document.getElementById('df2').src = this.value" style="font-size:20px; position:absolute; left:989px; top:-121px; width:284px;">
    <option value="playertemplate.png">Odaberite Stopera</option>
    <option value="dperic.png">Dino Perić (Dinamo Zagreb)</option>
    <option value="ktheophilecatherine.png">Kevin Theophile-Catherine (Dinamo Zagreb)</option>
    <option value="edilaver.png">Emir Dilaver (Dinamo Zagreb)</option>
    <option value="jgvardiol.png">Joško Gvardiol (Dinamo Zagreb)</option>
    <option value="jsutalo.png">Josip Šutalo (Dinamo Zagreb)</option>
    <option value="bfranjic.png">Bartol Franjić (Dinamo Zagreb)</option>
    <option value="ssimic.png">Stefan Simić (Hajduk Split)</option>
    <option value="aismajli.png">Ardian Ismajli (Hajduk Split)</option>
    <option value="mvuskovic.png">Mario Vušković (Hajduk Split)</option>
    <option value="svucur.png">Stipe Vučur (Hajduk Split)</option>
    <option value="sradic.png">Stipe Radić (Hajduk Split)</option>
    <option value="ldellova.png">Lumbardh Dellova (Hajduk Split)</option>
    <option value="hsmolcic.png">Hrvoje Smolčić (Rijeka)</option>
    <option value="ngalovic.png">Nino Galović (Rijeka)</option>
    <option value="jescoval.png">Joao Escoval (Rijeka)</option>
    <option value="lsimic.png">Lorenco Šimić (Rijeka)</option>
    <option value="dvelkovski.png">Darko Velkovski (Rijeka)</option>
    <option value="jcelikovic.png">Jasmin Čeliković (Rijeka)</option>
    <option value="lmikulica.png">Luka Mikulica (Rijeka)</option>
    <option value="mskoric.png">Mile Škorić (Osijek)</option>
    <option value="amajstorovic.png">Ante Majstorović (Osijek)</option>
    <option value="bsutalo.png">Boško Šutalo (Osijek)</option>
    <option value="guti.png">Guti (Osijek)</option>
    <option value="dloncar.png">Danijel Lončar (Osijek)</option>
    <option value="sradeljic.png">Stjepan Radeljić (Osijek)</option>
    <option value="ajovicic.png">Aleksandar Jovičić (Gorica)</option>
    <option value="kkrizmanic.png">Krešimir Krizmanić (Gorica)</option>
    <option value="msteenvoorden.png">Matthew Steenvoorden (Gorica)</option>
    <option value="mjcelic.png">Maks Juraj Čelić (Gorica)</option>
    <option value="nljubisavljevic.png">Nemanja Ljubisavljević (Gorica)</option>
    <option value="dkolinger.png">Denis Kolinger (Lokomotiva Zagreb)</option>
    <option value="jmersinaj.png">Jon Mersinaj (Lokomotiva Zagreb)</option>
    <option value="mleskovic.png">Marko Lešković (Lokomotiva Zagreb)</option>
    <option value="msuto.png">Mate Šuto (Lokomotiva Zagreb)</option>
    <option value="lsmoljo.png">Luka Smoljo (Lokomotiva Zagreb)</option>
    <option value="bmikulic.png">Božo Mikulić (Slaven Belupo)</option>
    <option value="vmedimorec.png">Vinko Međimorec (Slaven Belupo)</option>
    <option value="mzirdum.png">Matko Zirdum (Slaven Belupo)</option>
    <option value="knowak.png">Krystian Nowak (Slaven Belupo)</option>
    <option value="tbozic.png">Tomislav Božić (Slaven Belupo)</option>
    <option value="fhlevnjak.png">Filip Hlevnjak (Slaven Belupo)</option>
    <option value="nsoldo.png">Nikola Soldo (Inter Zaprešić)</option>
    <option value="dgrgic.png">Damir Grgić (Inter Zaprešić)</option>
    <option value="msavic.png">Milan Savić (Inter Zaprešić)</option>
    <option value="itatomirovic.png">Ivan Tatomirović (Inter Zaprešić)</option>
    <option value="inekic.png">Ivan Nekić (Inter Zaprešić)</option>
    <option value="igrozdek.png">Ivan Grožđek (Inter Zaprešić)</option>
    <option value="pbosancic.png">Petar Bosančić (Istra 1961)</option>
    <option value="jtomasevic.png">Josip Tomašević (Istra 1961)</option>
    <option value="arufati.png">Agron Rufati (Istra 1961)</option>
    <option value="rpaez.png">Rafa Paez (Istra 1961)</option>
    <option value="fprce.png">Franjo Prce (Varaždin)</option>
    <option value="mstolnik.png">Marko Stolnik (Varaždin)</option>
    <option value="msenic.png">Matej Senić (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:948px; top:540px;">
  <img id="df3" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectdf3" v-on:change="counterdf3(); showButton(); bodovidf3();" onchange="document.getElementById('df3').src = this.value" style="font-size:20px; position:absolute; left:671px; top:-94px; width:284px;">
    <option value="playertemplate.png">Odaberite Stopera</option>
    <option value="dperic.png">Dino Perić (Dinamo Zagreb)</option>
    <option value="ktheophilecatherine.png">Kevin Theophile-Catherine (Dinamo Zagreb)</option>
    <option value="edilaver.png">Emir Dilaver (Dinamo Zagreb)</option>
    <option value="jgvardiol.png">Joško Gvardiol (Dinamo Zagreb)</option>
    <option value="jsutalo.png">Josip Šutalo (Dinamo Zagreb)</option>
    <option value="bfranjic.png">Bartol Franjić (Dinamo Zagreb)</option>
    <option value="ssimic.png">Stefan Simić (Hajduk Split)</option>
    <option value="aismajli.png">Ardian Ismajli (Hajduk Split)</option>
    <option value="mvuskovic.png">Mario Vušković (Hajduk Split)</option>
    <option value="svucur.png">Stipe Vučur (Hajduk Split)</option>
    <option value="sradic.png">Stipe Radić (Hajduk Split)</option>
    <option value="hsmolcic.png">Hrvoje Smolčić (Rijeka)</option>
    <option value="ngalovic.png">Nino Galović (Rijeka)</option>
    <option value="jescoval.png">Joao Escoval (Rijeka)</option>
    <option value="lsimic.png">Lorenco Šimić (Rijeka)</option>
    <option value="dvelkovski.png">Darko Velkovski (Rijeka)</option>
    <option value="jcelikovic.png">Jasmin Čeliković (Rijeka)</option>
    <option value="lmikulica.png">Luka Mikulica (Rijeka)</option>
    <option value="mskoric.png">Mile Škorić (Osijek)</option>
    <option value="amajstorovic.png">Ante Majstorović (Osijek)</option>
    <option value="bsutalo.png">Boško Šutalo (Osijek)</option>
    <option value="guti.png">Guti (Osijek)</option>
    <option value="dloncar.png">Danijel Lončar (Osijek)</option>
    <option value="sradeljic.png">Stjepan Radeljić (Osijek)</option>
    <option value="ajovicic.png">Aleksandar Jovičić (Gorica)</option>
    <option value="kkrizmanic.png">Krešimir Krizmanić (Gorica)</option>
    <option value="msteenvoorden.png">Matthew Steenvoorden (Gorica)</option>
    <option value="mjcelic.png">Maks Juraj Čelić (Gorica)</option>
    <option value="nljubisavljevic.png">Nemanja Ljubisavljević (Gorica)</option>
    <option value="dkolinger.png">Denis Kolinger (Lokomotiva Zagreb)</option>
    <option value="jmersinaj.png">Jon Mersinaj (Lokomotiva Zagreb)</option>
    <option value="mleskovic.png">Marko Lešković (Lokomotiva Zagreb)</option>
    <option value="msuto.png">Mate Šuto (Lokomotiva Zagreb)</option>
    <option value="bmikulic.png">Božo Mikulić (Slaven Belupo)</option>
    <option value="vmedimorec.png">Vinko Međimorec (Slaven Belupo)</option>
    <option value="mzirdum.png">Matko Zirdum (Slaven Belupo)</option>
    <option value="knowak.png">Krystian Nowak (Slaven Belupo)</option>
    <option value="tbozic.png">Tomislav Božić (Slaven Belupo)</option>
    <option value="fhlevnjak.png">Filip Hlevnjak (Slaven Belupo)</option>
    <option value="nsoldo.png">Nikola Soldo (Inter Zaprešić)</option>
    <option value="dgrgic.png">Damir Grgić (Inter Zaprešić)</option>
    <option value="msavic.png">Milan Savić (Inter Zaprešić)</option>
    <option value="itatomirovic.png">Ivan Tatomirović (Inter Zaprešić)</option>
    <option value="inekic.png">Ivan Nekić (Inter Zaprešić)</option>
    <option value="igrozdek.png">Ivan Grožđek (Inter Zaprešić)</option>
    <option value="pbosancic.png">Petar Bosančić (Istra 1961)</option>
    <option value="jtomasevic.png">Josip Tomašević (Istra 1961)</option>
    <option value="arufati.png">Agron Rufati (Istra 1961)</option>
    <option value="rpaez.png">Rafa Paez (Istra 1961)</option>
    <option value="fprce.png">Franjo Prce (Varaždin)</option>
    <option value="mstolnik.png">Marko Stolnik (Varaždin)</option>
    <option value="msenic.png">Matej Senić (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:1240px; top:540px;">
  <img id="df4" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectdf4" v-on:change="counterdf4(); showButton(); bodovidf4();" onchange="document.getElementById('df4').src = this.value" style="font-size:20px; position:absolute; left:379px; top:-67px; width:284px;">
    <option value="playertemplate.png">Odaberite Desnog Beka</option>
    <option value="pstojanovic.png">Petar Stojanović (Dinamo Zagreb)</option>
    <option value="smoharrami.png">Sadegh Moharrami (Dinamo Zagreb)</option>
    <option value="thrvoj.png">Tin Hrvoj (Dinamo Zagreb)</option>
    <option value="jjuranovic.png">Josip Juranović (Hajduk Split)</option>
    <option value="jbasic.png">Josip Bašić (Hajduk Split)</option>
    <option value="itomecak.png">Ivan Tomečak (Rijeka)</option>
    <option value="mraspopovic.png">Momčilo Raspopović (Rijeka)</option>
    <option value="isilva.png">Igor Silva (Osijek)</option>
    <option value="agrgic.png">Alen Grgić (Osijek)</option>
    <option value="tsorsa.png">Tomislav Šorša (Osijek)</option>
    <option value="ttodoroski.png">Todor Todoroski (Osijek)</option>
    <option value="mmuhammed.png">Musa Muhammed (Gorica)</option>
    <option value="pperisa.png">Patrik Periša (Gorica)</option>
    <option value="fkaracic.png">Fran Karačić (Lokomotiva Zagreb)</option>
    <option value="pgluhakovic.png">Petar Gluhaković (Lokomotiva Zagreb)</option>
    <option value="mkaramarko.png">Marko Karamarko (Slaven Belupo)</option>
    <option value="miharos.png">Marko Iharoš (Slaven Belupo)</option>
    <option value="abosec.png">Antonio Bosec (Inter Zaprešić)</option>
    <option value="gbaric.png">Gordan Barić (Inter Zaprešić)</option>
    <option value="mgalic.png">Marin Galić (Inter Zaprešić)</option>
    <option value="mgrujevic.png">Marin Grujević (Istra 1961)</option>
    <option value="mfranic.png">Martin Franić (Istra 1961)</option>
    <option value="ntkalcic.png">Nikola Tkalčić (Varaždin)</option>
    <option value="dperkovic.png">Dominik Perković (Varaždin)</option>
  </select>
  </div>

  <div style="text-align:center; font-size:40px; font-family: Cuprum; color:black; width:image width px; position:absolute; left:797px; top:640px;">
  <img id="gk1" src="playertemplate.png" style="position: absolute; top:50px;">
   <select id="selectgk1" v-on:change="countergk1(); showButton(); bodovigk1();" onchange="document.getElementById('gk1').src = this.value" style="font-size:20px; position:absolute; left:822px; top:-140px; width:284px;">
    <option value="playertemplate.png">Odaberite Vratara</option>
    <option value="dlivakovic.png">Dominik Livaković (Dinamo Zagreb)</option>
    <option value="dzagorac.png">Danijel Zagorac (Dinamo Zagreb)</option>
    <option value="jposavec.png">Josip Posavec (Hajduk Split)</option>
    <option value="mljubic.png">Marin Ljubić (Hajduk Split)</option>
    <option value="gblazevic.png">Goran Blažević (Hajduk Split)</option>
    <option value="dmatijas.png">Davor Matijaš (Hajduk Split)</option>
    <option value="aprskalo.png">Andrej Prskalo (Rijeka)</option>
    <option value="ipandur.png">Ivor Pandur (Rijeka)</option>
    <option value="dnwolokor.png">David Nwolokor (Rijeka)</option>
    <option value="iivusic.png">Ivica Ivušić (Osijek)</option>
    <option value="mmalenica.png">Marko Malenica (Osijek)</option>
    <option value="kkahlina.png">Kristijan Kahlina (Gorica)</option>
    <option value="icovic.png">Ivan Čović (Gorica)</option>
    <option value="igrbic.png">Ivo Grbić (Lokomotiva Zagreb)</option>
    <option value="khendija.png">Krunoslav Hendija (Lokomotiva Zagreb)</option>
    <option value="ifilipovic.png">Ivan Filipović (Slaven Belupo)</option>
    <option value="ajezina.png">Antonio Ježina (Slaven Belupo)</option>
    <option value="zfrelih.png">Žiga Frelih (Inter Zaprešić)</option>
    <option value="mmatkovic.png">Mladen Matković (Inter Zaprešić)</option>
    <option value="jcondric.png">Josip Čondrić (Istra 1961)</option>
    <option value="tduka.png">Tomislav Duka (Istra 1961)</option>
    <option value="lmajkic.png">Lovro Majkić (Istra 1961)</option>
    <option value="inevistic.png">Ivan Nevistić (Varaždin)</option>
    <option value="amrmic.png">Ante Mrmić (Varaždin)</option>
  </select>
  </div>

<button id="Button" onclick="
  document.getElementById('selectfw1').disabled=true;
  document.getElementById('selectfw2').disabled=true;
  document.getElementById('selectfw3').disabled=true;
  document.getElementById('selectmf1').disabled=true;
  document.getElementById('selectmf2').disabled=true;
  document.getElementById('selectmf3').disabled=true;
  document.getElementById('selectdf1').disabled=true;
  document.getElementById('selectdf2').disabled=true;
  document.getElementById('selectdf3').disabled=true;
  document.getElementById('selectdf4').disabled=true;
  document.getElementById('selectgk1').disabled=true;
   "
   v-on:click="savedb();"
   style="font-family:Cuprum; font-size:28px; position:absolute; left:1675px; top:550px;">ZAKLJUČAJ TIM</button>

  </div>
</template>

<script>
    import store from '@/store.js'
    var countfw1=0;
    var countfw2=0;
    var countfw3=0;
    var countmf1=0;
    var countmf2=0;
    var countmf3=0;
    var countdf1=0;
    var countdf2=0;
    var countdf3=0;
    var countdf4=0;
    var countgk1=0;
    var fw1w1,fw1w2,fw1w3,fw1w4,fw1w5,fw1w6,fw1w7,fw1w8,fw1w9,fw1w10,fw1w11,fw1w12,fw1w13,fw1w14,fw1w15,fw1w16,fw1w17,fw1w18,fw1w19;
    var fw2w1,fw2w2,fw2w3,fw2w4,fw2w5,fw2w6,fw2w7,fw2w8,fw2w9,fw2w10,fw2w11,fw2w12,fw2w13,fw2w14,fw2w15,fw2w16,fw2w17,fw2w18,fw2w19;
    var fw3w1,fw3w2,fw3w3,fw3w4,fw3w5,fw3w6,fw3w7,fw3w8,fw3w9,fw3w10,fw3w11,fw3w12,fw3w13,fw3w14,fw3w15,fw3w16,fw3w17,fw3w18,fw3w19;
    var mf1w1;
    var mf2w1;
    var mf3w1;
    var df1w1;
    var df2w1;
    var df3w1;
    var df4w1;
    var gk1w1;
    export default {
      data(){
          return store;
      },
      methods:{
          counterfw1(){
            if(document.getElementById('selectfw1').value!="playertemplate.png"){
              countfw1=1;
            }
          },
          counterfw2(){
            if(document.getElementById('selectfw2').value!="playertemplate.png"){
              countfw2=1;
            }
          },
          counterfw3(){
            if(document.getElementById('selectfw3').value!="playertemplate.png"){
              countfw3=1;
            }
          },
          countermf1(){
            if(document.getElementById('selectmf1').value!="playertemplate.png"){
              countmf1=1;
            }
          },
          countermf2(){
            if(document.getElementById('selectmf2').value!="playertemplate.png"){
              countmf2=1;
            }
          },
          countermf3(){
            if(document.getElementById('selectmf3').value!="playertemplate.png"){
              countmf3=1;
            }
          },
          counterdf1(){
            if(document.getElementById('selectdf1').value!="playertemplate.png"){
              countdf1=1;
            }
          },
          counterdf2(){
            if(document.getElementById('selectdf2').value!="playertemplate.png"){
              countdf2=1;
            }
          },
          counterdf3(){
            if(document.getElementById('selectdf3').value!="playertemplate.png"){
              countdf3=1;
            }
          },
          counterdf4(){
            if(document.getElementById('selectdf4').value!="playertemplate.png"){
              countdf4=1;
            }
          },
          countergk1(){
            if(document.getElementById('selectgk1').value!="playertemplate.png"){
              countgk1=1;
            }
          },
          showButton(){
            if((countfw1+countfw2+countfw3+countmf1+countmf2+countmf3+countdf1+countdf2+countdf3+countdf4+countgk1)===11){
              if((document.getElementById('selectmf1').value!=document.getElementById('selectmf2').value)&&
              (document.getElementById('selectmf1').value!=document.getElementById('selectmf3').value)&&
              (document.getElementById('selectmf2').value!=document.getElementById('selectmf3').value)&&
              document.getElementById('selectdf1').value!=document.getElementById('selectdf2').value){
              document.getElementById("Button").disabled = false;
              }
            }
          },
          bodovifw1(){
            if(document.getElementById('selectfw1').value.includes("petkovic")){
              fw1w1=3;
            }
          },
          bodovifw2(){
            if(document.getElementById('selectfw2').value.includes("orsic")){
              fw2w1=3;
            }
          },
          bodovifw3(){
            if(document.getElementById('selectfw3').value.includes("kadzior")){
              fw3w1=3;
            }
          },
          bodovimf1(){
            if(document.getElementById('selectmf1').value.includes("olmo")){
              mf1w1=3;
            }
          },
          bodovimf2(){
            if(document.getElementById('selectmf2').value.includes("ademi")){
              mf2w1=3;
            }
          },
          bodovimf3(){
            if(document.getElementById('selectmf3').value.includes("moro")){
              mf3w1=3;
            }
          },
          bodovidf1(){
            if(document.getElementById('selectdf1').value.includes("leovac")){
              df1w1=3;
            }
          },
          bodovidf2(){
            if(document.getElementById('selectdf2').value.includes("peric")){
              df2w1=3;
            }
          },
          bodovidf3(){
            if(document.getElementById('selectdf3').value.includes("theophilecatherine")){
              df3w1=3;
            }
          },
          bodovidf4(){
            if(document.getElementById('selectdf4').value.includes("stojanovic")){
              df4w1=3;
            }
          },
          bodovigk1(){
            if(document.getElementById('selectgk1').value.includes("livakovic")){
              gk1w1=3;
            }
          },
          bodoviw1(){
            console.log(gk1w1)
          },
          savedb() {
          let id = this.userEmail;
          db.collection("timovi").doc(id).set({
                                        st: document.getElementById('selectfw1').value,
                                        lw: document.getElementById('selectfw2').value,
                                        rw: document.getElementById('selectfw3').value,
                                        lcm: document.getElementById('selectmf1').value,
                                        ccm: document.getElementById('selectmf2').value,
                                        rcm: document.getElementById('selectmf3').value,
                                        lb: document.getElementById('selectdf1').value,
                                        lcb: document.getElementById('selectdf2').value,
                                        rcb: document.getElementById('selectdf3').value,
                                        rb: document.getElementById('selectdf4').value,
                                        gk: document.getElementById('selectgk1').value, })
          },
          loaddb(){
            let id = this.userEmail;
            db.collection("timovi").doc(id).get().then(doc => {
              if(doc.exists){
                            document.getElementById('selectfw1').value = doc.data().st;
                            document.getElementById('fw1').src = doc.data().st;
                            document.getElementById('selectfw2').value = doc.data().lw;
                            document.getElementById('fw2').src = doc.data().lw;
                            document.getElementById('selectfw3').value = doc.data().rw;
                            document.getElementById('fw3').src = doc.data().rw;
                            document.getElementById('selectmf1').value = doc.data().lcm;
                            document.getElementById('mf1').src = doc.data().lcm;
                            document.getElementById('selectmf2').value = doc.data().ccm;
                            document.getElementById('mf2').src = doc.data().ccm;
                            document.getElementById('selectmf3').value = doc.data().rcm;
                            document.getElementById('mf3').src = doc.data().rcm;
                            document.getElementById('selectdf1').value = doc.data().lb;
                            document.getElementById('df1').src = doc.data().lb;
                            document.getElementById('selectdf2').value = doc.data().lcb;
                            document.getElementById('df2').src = doc.data().lcb;
                            document.getElementById('selectdf3').value = doc.data().rcb;
                            document.getElementById('df3').src = doc.data().rcb;
                            document.getElementById('selectdf4').value = doc.data().rb;
                            document.getElementById('df4').src = doc.data().rb;
                            document.getElementById('selectgk1').value = doc.data().gk;
                            document.getElementById('gk1').src = doc.data().gk;
              }
            })
          }
      },
      beforeUpdate(){
        this.loaddb();
      }
    }
</script>
