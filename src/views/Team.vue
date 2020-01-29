<template>
  <div class="jumbotron jumbotron-fluid" id="jumboteam" style="background-image: url(teren.jpg);">
    <h1 class="display-2" id="naslovteam"><b>{{ myteam }} </b>
    </h1>

  <div id="divfw1">
    <img id="fw1" src="playertemplate.png">
    <select id="selectfw1" v-on:change="counterfw1(); showButton(); bodovifw1();" onchange="document.getElementById('fw1').src = this.value;">
      <option value="playertemplate.png">Odaberite Napadača</option>
      <option value="bpetkovic.png">Bruno Petković (Dinamo Zagreb)</option>
      <option value="mgavranovic.png">Mario Gavranović (Dinamo Zagreb)</option>
      <option value="skulenovic.png">Sandro Kulenović (Dinamo Zagreb)</option>
      <option value="kandric.png">Komnen Andrić (Dinamo Zagreb)</option>
      <option value="mcuze.png">Mario Ćuže (Dinamo Zagreb)</option>
      <option value="rbaturina.png">Roko Baturina (Dinamo Zagreb)</option>
      <option value="lsipos.png">Leon Šipoš (Dinamo Zagreb)</option>
      <option value="mjakolis.png">Marin Jakoliš (Hajduk Split)</option>
      <option value="idelic.png">Ivan Delić (Hajduk Split)</option>
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
      <option value="drakic.png">Đorđe Rakić (Lokomotiva Zagreb)</option>
      <option value="lmaruzin.png">Loren Maružin (Lokomotiva Zagreb)</option>
      <option value="mdelic.png">Mateas Delić (Slaven Belupo)</option>
      <option value="mmladen.png">Mihael Mladen (Slaven Belupo)</option>
      <option value="msego.png">Michele Šego (Slaven Belupo)</option>
      <option value="fetoundi.png">Franck Etoundi (Slaven Belupo)</option>
      <option value="mateus.png">Mateus (Slaven Belupo)</option>
      <option value="ikrstanovic.png">Ivan Krstanović (Slaven Belupo)</option>
      <option value="akaluderovic.png">Andrija Kaluđerović (Inter Zaprešić)</option>
      <option value="imamut.png">Ivan Mamut (Inter Zaprešić)</option>
      <option value="mvasilj.png">Mario Vasilj (Inter Zaprešić)</option>
      <option value="wtchuameni.png">William Tchuameni (Inter Zaprešić)</option>
      <option value="bbilobrk.png">Borna Bilobrk (Inter Zaprešić)</option>
      <option value="mbencic.png">Mihael Benčić (Inter Zaprešić)</option>
      <option value="klaukzemis.png">Karolis Laukžemis (Istra 1961)</option>
      <option value="rperickomsic.png">Robert Perić-Komšić (Istra 1961)</option>
      <option value="afuentes.png">Adrian Fuentes (Istra 1961)</option>
      <option value="vlisakovich.png">Vitali Lisakovich (Varaždin)</option>
      <option value="lbenko.png">Leon Benko (Varaždin)</option>
      <option value="dglavina.png">Dominik Glavina (Varaždin)</option>
      <option value="pkesse.png">Patrick Kesse (Varaždin)</option>
    </select>
  </div>

  <div id="divfw2">
    <img id="fw2" src="playertemplate.png">
    <select id="selectfw2" v-on:change="counterfw2(); showButton(); bodovifw2();" onchange="document.getElementById('fw2').src = this.value">
      <option value="playertemplate.png">Odaberite Lijevo Krilo</option>
      <option value="morsic.png">Mislav Oršić (Dinamo Zagreb)</option>
      <option value="iatiemwen.png">Iyayi Atiemwen (Dinamo Zagreb)</option>
      <option value="amarin.png">Antonio Marin (Dinamo Zagreb)</option>
      <option value="jairo.png">Jairo da Silva (Hajduk Split)</option>
      <option value="idolcek.png">Ivan Dolček (Hajduk Split)</option>
      <option value="esahiti.png">Emir Sahiti (Hajduk Split)</option>
      <option value="agorgon.png">Alexander Gorgon (Rijeka)</option>
      <option value="mvuk.png">Matej Vuk (Rijeka)</option>
      <option value="pbockaj.png">Petar Bočkaj (Osijek)</option>
      <option value="mndockyt.png">Merveil Ndockyt (Osijek)</option>
      <option value="mpilj.png">Marin Pilj (Osijek)</option>
      <option value="klovric.png">Kristijan Lovrić (Gorica)</option>
      <option value="msroler.png">Martin Šroler (Gorica)</option>
      <option value="dspikic.png">Dario Špikić (Gorica)</option>
      <option value="muzuni.png">Myrto Uzuni (Lokomotiva Zagreb)</option>
      <option value="jmajic.png">Josip Majić (Lokomotiva Zagreb)</option>
      <option value="dlovren.png">Davor Lovren (Slaven Belupo)</option>
      <option value="sserderov.png">Serder Serderov (Inter Zaprešić)</option>
      <option value="ozamouri.png">Oussama Zamouri (Inter Zaprešić)</option>
      <option value="dbusnja.png">Denis Bušnja (Istra 1961)</option>
      <option value="jmaganjic.png">Josip Maganjić (Istra 1961)</option>
      <option value="ddrozdek.png">Domagoj Drožđek (Varaždin)</option>
      <option value="lvuk.png">Leonard Vuk (Varaždin)</option>
      <option value="kfucak.png">Kristian Fućak (Varaždin)</option>
      <option value="vpetkovic.png">Vinko Petković (Varaždin)</option>
    </select>
  </div>

  <div id="divfw3">
    <img id="fw3" src="playertemplate.png">
    <select id="selectfw3" v-on:change="counterfw3(); showButton(); bodovifw3();" onchange="document.getElementById('fw3').src = this.value">
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
      <option value="nhavelka.png">Niko Havelka (Slaven Belupo)</option>
      <option value="jmitrovic.png">Josip Mitrović (Inter Zaprešić)</option>
      <option value="sgrzan.png">Šime Gržan (Istra 1961)</option>
      <option value="mmunivrana.png">Mario Munivrana (Istra 1961)</option>
      <option value="asane.png">Arona Sane (Istra 1961)</option>
      <option value="mmehdikani.png">Mehdi Mehdikani (Varaždin)</option>
      <option value="tturcin.png">Tomislav Turčin (Varaždin)</option>
      <option value="mkolaric.png">Matija Kolarić (Varaždin)</option>
    </select>
  </div>

  <div id="divmf1">
    <img id="mf1" src="playertemplate.png">
    <select id="selectmf1" v-on:change="countermf1(); showButton(); bodovimf1();" onchange="document.getElementById('mf1').src = this.value">
      <option value="playertemplate.png">Odaberite Veznjaka</option>
      <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
      <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
      <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
      <option value="rmiskovic.png">Robert Mišković (Dinamo Zagreb)</option>
      <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
      <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
      <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
      <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
      <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
      <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
      <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
      <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
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
      <option value="asvetic.png">Antun Svetić (Rijeka)</option>
      <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
      <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
      <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
      <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
      <option value="mzaper.png">Mihael Žaper (Osijek)</option>
      <option value="jljubic.png">Juraj Ljubić (Osijek)</option>
      <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
      <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
      <option value="jsuk.png">Joey Suk (Gorica)</option>
      <option value="icepo.png">Ivano Čepo (Gorica)</option>
      <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
      <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
      <option value="mmaloca.png">Martin Maloča (Gorica)</option>
      <option value="pgolubickas.png">Paulius Golubickas (Gorica)</option>
      <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
      <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
      <option value="fvojkovic.png">Frane Vojković (Lokomotiva Zagreb)</option>
      <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
      <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
      <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
      <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
      <option value="ecokaj.png">Enis Čokaj (Lokomotiva Zagreb)</option>
      <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
      <option value="tbrezina.png">Toni Brezina (Lokomotiva Zagreb)</option>
      <option value="acarapina.png">Andrijano Čarapina (Lokomotiva Zagreb)</option>
      <option value="bkaroglan.png">Bruno Karoglan (Lokomotiva Zagreb)</option>
      <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
      <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
      <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
      <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
      <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
      <option value="rkamber.png">Robin Kamber (Slaven Belupo)</option>
      <option value="tsrbljinovic.png">Tomislav Srbljinović (Slaven Belupo)</option>
      <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
      <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
      <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
      <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
      <option value="tmazalovic.png">Tomislav Mazalović (Inter Zaprešić)</option>
      <option value="smarasovic.png">Sacha Marasović (Inter Zaprešić)</option>
      <option value="aspoljaric.png">Ante Špoljarić (Inter Zaprešić)</option>
      <option value="robeng.png">Regan Obeng (Istra 1961)</option>
      <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
      <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
      <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
      <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
      <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
      <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
      <option value="tburic.png">Toni Burić (Istra 1961)</option>
      <option value="opaez.png">Octavio Paez (Istra 1961)</option>
      <option value="dsadiku.png">Drilon Sadiku (Istra 1961)</option>
      <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
      <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
      <option value="ktezak.png">Karlo Težak (Varaždin)</option>
      <option value="syokoyama.png">Shohei Yokoyama (Varaždin)</option>
      <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
      <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
      <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
      <option value="iroca.png">Ivan Roca (Varaždin)</option>
    </select>
  </div>

  <div id="divmf2">
    <img id="mf2" src="playertemplate.png">
    <select id="selectmf2" v-on:change="countermf2(); showButton(); bodovimf2();" onchange="document.getElementById('mf2').src = this.value">
      <option value="playertemplate.png">Odaberite Veznjaka</option>
      <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
      <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
      <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
      <option value="rmiskovic.png">Robert Mišković (Dinamo Zagreb)</option>
      <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
      <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
      <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
      <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
      <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
      <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
      <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
      <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
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
      <option value="asvetic.png">Antun Svetić (Rijeka)</option>
      <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
      <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
      <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
      <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
      <option value="mzaper.png">Mihael Žaper (Osijek)</option>
      <option value="jljubic.png">Juraj Ljubić (Osijek)</option>
      <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
      <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
      <option value="jsuk.png">Joey Suk (Gorica)</option>
      <option value="icepo.png">Ivano Čepo (Gorica)</option>
      <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
      <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
      <option value="mmaloca.png">Martin Maloča (Gorica)</option>
      <option value="pgolubickas.png">Paulius Golubickas (Gorica)</option>
      <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
      <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
      <option value="fvojkovic.png">Frane Vojković (Lokomotiva Zagreb)</option>
      <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
      <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
      <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
      <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
      <option value="ecokaj.png">Enis Čokaj (Lokomotiva Zagreb)</option>
      <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
      <option value="tbrezina.png">Toni Brezina (Lokomotiva Zagreb)</option>
      <option value="acarapina.png">Andrijano Čarapina (Lokomotiva Zagreb)</option>
      <option value="bkaroglan.png">Bruno Karoglan (Lokomotiva Zagreb)</option>
      <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
      <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
      <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
      <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
      <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
      <option value="rkamber.png">Robin Kamber (Slaven Belupo)</option>
      <option value="tsrbljinovic.png">Tomislav Srbljinović (Slaven Belupo)</option>
      <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
      <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
      <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
      <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
      <option value="tmazalovic.png">Tomislav Mazalović (Inter Zaprešić)</option>
      <option value="smarasovic.png">Sacha Marasović (Inter Zaprešić)</option>
      <option value="aspoljaric.png">Ante Špoljarić (Inter Zaprešić)</option>
      <option value="robeng.png">Regan Obeng (Istra 1961)</option>
      <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
      <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
      <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
      <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
      <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
      <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
      <option value="tburic.png">Toni Burić (Istra 1961)</option>
      <option value="opaez.png">Octavio Paez (Istra 1961)</option>
      <option value="dsadiku.png">Drilon Sadiku (Istra 1961)</option>
      <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
      <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
      <option value="ktezak.png">Karlo Težak (Varaždin)</option>
      <option value="syokoyama.png">Shohei Yokoyama (Varaždin)</option>
      <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
      <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
      <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
      <option value="iroca.png">Ivan Roca (Varaždin)</option>
    </select>
  </div>

  <div id="divmf3">
    <img id="mf3" src="playertemplate.png">
    <select id="selectmf3" v-on:change="countermf3(); showButton(); bodovimf3();" onchange="document.getElementById('mf3').src = this.value">
      <option value="playertemplate.png">Odaberite Veznjaka</option>
      <option value="agojak.png">Amer Gojak (Dinamo Zagreb)</option>
      <option value="livanusec.png">Luka Ivanušec (Dinamo Zagreb)</option>
      <option value="lmajer.png">Lovro Majer (Dinamo Zagreb)</option>
      <option value="rmiskovic.png">Robert Mišković (Dinamo Zagreb)</option>
      <option value="aademi.png">Arijan Ademi (Dinamo Zagreb)</option>
      <option value="nmoro.png">Nikola Moro (Dinamo Zagreb)</option>
      <option value="mdira.png">Marko Đira (Dinamo Zagreb)</option>
      <option value="bjradi.png">Bassel Jradi (Hajduk Split)</option>
      <option value="tteklic.png">Tonio Teklić (Hajduk Split)</option>
      <option value="jblagaic.png">Jakov Blagaić (Hajduk Split)</option>
      <option value="mcaktas.png">Mijo Caktaš (Hajduk Split)</option>
      <option value="hbarry.png">Hamza Barry (Hajduk Split)</option>
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
      <option value="asvetic.png">Antun Svetić (Rijeka)</option>
      <option value="lkleinheisler.png">Laszlo Kleinheisler (Osijek)</option>
      <option value="dlepa.png">Dmytro Lepa (Osijek)</option>
      <option value="kkamenar.png">Karlo Kamenar (Osijek)</option>
      <option value="vjugovic.png">Vedran Jugović (Osijek)</option>
      <option value="mzaper.png">Mihael Žaper (Osijek)</option>
      <option value="jljubic.png">Juraj Ljubić (Osijek)</option>
      <option value="jhamad.png">Jiloan Hamad (Gorica)</option>
      <option value="mmaslowski.png">Michal Maslowski (Gorica)</option>
      <option value="jsuk.png">Joey Suk (Gorica)</option>
      <option value="icepo.png">Ivano Čepo (Gorica)</option>
      <option value="dcanadija.png">Dario Čanađija (Gorica)</option>
      <option value="hbabec.png">Hrvoje Babec (Gorica)</option>
      <option value="mmaloca.png">Martin Maloča (Gorica)</option>
      <option value="pgolubickas.png">Paulius Golubickas (Gorica)</option>
      <option value="mtolic.png">Marko Tolić (Lokomotiva Zagreb)</option>
      <option value="sammir.png">Sammir (Lokomotiva Zagreb)</option>
      <option value="fvojkovic.png">Frane Vojković (Lokomotiva Zagreb)</option>
      <option value="sgorican.png">Silvio Goričan (Lokomotiva Zagreb)</option>
      <option value="dhalilovic.png">Dino Halilović (Lokomotiva Zagreb)</option>
      <option value="passane.png">Pape Assane (Lokomotiva Zagreb)</option>
      <option value="kjakic.png">Kristijan Jakić (Lokomotiva Zagreb)</option>
      <option value="ecokaj.png">Enis Čokaj (Lokomotiva Zagreb)</option>
      <option value="opetrak.png">Oliver Petrak (Lokomotiva Zagreb)</option>
      <option value="tbrezina.png">Toni Brezina (Lokomotiva Zagreb)</option>
      <option value="acarapina.png">Andrijano Čarapina (Lokomotiva Zagreb)</option>
      <option value="bkaroglan.png">Bruno Karoglan (Lokomotiva Zagreb)</option>
      <option value="klulic.png">Karlo Lulić (Slaven Belupo)</option>
      <option value="nglavcic.png">Nemanja Glavčić (Slaven Belupo)</option>
      <option value="sbacelicgrgic.png">Stipe Bačelić-Grgić (Slaven Belupo)</option>
      <option value="dpuclin.png">David Puclin (Slaven Belupo)</option>
      <option value="gparacki.png">Goran Paracki (Slaven Belupo)</option>
      <option value="rkamber.png">Robin Kamber (Slaven Belupo)</option>
      <option value="tsrbljinovic.png">Tomislav Srbljinović (Slaven Belupo)</option>
      <option value="abrkovic.png">Arijan Brković (Slaven Belupo)</option>
      <option value="btsonev.png">Borislav Tsonev (Inter Zaprešić)</option>
      <option value="ipostonjski.png">Igor Postonjski (Inter Zaprešić)</option>
      <option value="fmlinar.png">Frano Mlinar (Inter Zaprešić)</option>
      <option value="tmazalovic.png">Tomislav Mazalović (Inter Zaprešić)</option>
      <option value="smarasovic.png">Sacha Marasović (Inter Zaprešić)</option>
      <option value="aspoljaric.png">Ante Špoljarić (Inter Zaprešić)</option>
      <option value="robeng.png">Regan Obeng (Istra 1961)</option>
      <option value="imocinic.png">Ivan Močinić (Istra 1961)</option>
      <option value="mfintic.png">Matija Fintić (Istra 1961)</option>
      <option value="egalilea.png">Einar Galilea (Istra 1961)</option>
      <option value="sblagojevic.png">Slavko Blagojević (Istra 1961)</option>
      <option value="aivancic.png">Antonio Ivančić (Istra 1961)</option>
      <option value="sloncar2.png">Stefan Lončar (Istra 1961)</option>
      <option value="tburic.png">Toni Burić (Istra 1961)</option>
      <option value="opaez.png">Octavio Paez (Istra 1961)</option>
      <option value="dsadiku.png">Drilon Sadiku (Istra 1961)</option>
      <option value="dglavica.png">Dejan Glavica (Varaždin)</option>
      <option value="iposavec.png">Ivan Posavec (Varaždin)</option>
      <option value="ktezak.png">Karlo Težak (Varaždin)</option>
      <option value="syokoyama.png">Shohei Yokoyama (Varaždin)</option>
      <option value="jgueradjou.png">Jessie Guera Djou (Varaždin)</option>
      <option value="ndurasek.png">Neven Đurasek (Varaždin)</option>
      <option value="jbajandooh.png">Jamal Bajandooh (Varaždin)</option>
      <option value="iroca.png">Ivan Roca (Varaždin)</option>
    </select>
  </div>

  <div id="divdf1">
    <img id="df1" src="playertemplate.png">
    <select id="selectdf1" v-on:change="counterdf1(); showButton(); bodovidf1();" onchange="document.getElementById('df1').src = this.value">
      <option value="playertemplate.png">Odaberite Lijevog Beka</option>
      <option value="fmoubandje.png">Francois Moubandje (Dinamo Zagreb)</option>
      <option value="mleovac.png">Marin Leovac (Dinamo Zagreb)</option>
      <option value="dcolina.png">David Čolina (Hajduk Split)</option>
      <option value="pmamic.png">Petar Mamić (Rijeka)</option>
      <option value="dstefulj.png">Daniel Štefulj (Rijeka)</option>
      <option value="mkabiru.png">Muhammed Kabiru (Rijeka)</option>
      <option value="talys.png">Talys (Osijek)</option>
      <option value="lmarin.png">Luka Marin (Osijek)</option>
      <option value="mcabraja.png">Marijan Čabraja (Gorica)</option>
      <option value="smarkovic.png">Stipo Marković (Lokomotiva Zagreb)</option>
      <option value="bvliet.png">Bradley Vliet (Lokomotiva Zagreb)</option>
      <option value="srozman.png">Siniša Rožman (Lokomotiva Zagreb)</option>
      <option value="imilicevic.png">Ivan Miličević (Lokomotiva Zagreb)</option>
      <option value="icelikovic.png">Ivan Čeliković (Lokomotiva Zagreb)</option>
      <option value="bgoda.png">Bruno Goda (Slaven Belupo)</option>
      <option value="mradivojevic.png">Miloš Radivojević (Slaven Belupo)</option>
      <option value="mmartinaga.png">Marko Martinaga (Slaven Belupo)</option>
      <option value="svego.png">Stjepan Vego (Inter Zaprešić)</option>
      <option value="mpavic.png">Markus Pavić (Istra 1961)</option>
      <option value="sgonzalez.png">Sergio Gonzalez (Istra 1961)</option>
      <option value="dglavina2.png">Denis Glavina (Varaždin)</option>
      <option value="mspicic.png">Matija Špičić (Varaždin)</option>
      <option value="ksambolec.png">Karlo Sambolec (Varaždin)</option>
    </select>
  </div>

  <div id="divdf2">
    <img id="df2" src="playertemplate.png">
    <select id="selectdf2" v-on:change="counterdf2(); showButton(); bodovidf2();" onchange="document.getElementById('df2').src = this.value">
      <option value="playertemplate.png">Odaberite Stopera</option>
      <option value="dperic.png">Dino Perić (Dinamo Zagreb)</option>
      <option value="ktheophilecatherine.png">Kevin Theophile-Catherine (Dinamo Zagreb)</option>
      <option value="edilaver.png">Emir Dilaver (Dinamo Zagreb)</option>
      <option value="jgvardiol.png">Joško Gvardiol (Dinamo Zagreb)</option>
      <option value="vsoldo.png">Vinko Soldo (Dinamo Zagreb)</option>
      <option value="jsutalo.png">Josip Šutalo (Dinamo Zagreb)</option>
      <option value="bfranjic.png">Bartol Franjić (Dinamo Zagreb)</option>
      <option value="ssimic.png">Stefan Simić (Hajduk Split)</option>
      <option value="aismajli.png">Ardian Ismajli (Hajduk Split)</option>
      <option value="nmujakic.png">Nihad Mujakić (Hajduk Split)</option>
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
      <option value="ajovicic.png">Aleksandar Jovičić (Gorica)</option>
      <option value="kkrizmanic.png">Krešimir Krizmanić (Gorica)</option>
      <option value="msteenvoorden.png">Matthew Steenvoorden (Gorica)</option>
      <option value="mjcelic.png">Maks Juraj Čelić (Gorica)</option>
      <option value="dkolinger.png">Denis Kolinger (Lokomotiva Zagreb)</option>
      <option value="jmersinaj.png">Jon Mersinaj (Lokomotiva Zagreb)</option>
      <option value="mleskovic.png">Marko Lešković (Lokomotiva Zagreb)</option>
      <option value="dkovacic.png">Dominik Kovačić (Lokomotiva Zagreb)</option>
      <option value="djokovic.png">Dušan Joković (Lokomotiva Zagreb)</option>
      <option value="msuto.png">Mate Šuto (Lokomotiva Zagreb)</option>
      <option value="npejovic.png">Nikola Pejović (Lokomotiva Zagreb)</option>
      <option value="ilovric.png">Ivan Lovrić (Lokomotiva Zagreb)</option>
      <option value="lsmoljo.png">Luka Smoljo (Lokomotiva Zagreb)</option>
      <option value="ffilipovic.png">Frano Filipović (Lokomotiva Zagreb)</option>
      <option value="franklin.png">Franklin (Lokomotiva Zagreb)</option>
      <option value="bmikulic.png">Božo Mikulić (Slaven Belupo)</option>
      <option value="vmedimorec.png">Vinko Međimorec (Slaven Belupo)</option>
      <option value="mzirdum.png">Matko Zirdum (Slaven Belupo)</option>
      <option value="tbozic.png">Tomislav Božić (Slaven Belupo)</option>
      <option value="fhlevnjak.png">Filip Hlevnjak (Slaven Belupo)</option>
      <option value="nsoldo.png">Nikola Soldo (Inter Zaprešić)</option>
      <option value="dvanbruggen.png">Damian van Bruggen (Inter Zaprešić)</option>
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
      <option value="inovoselec.png">Ivan Novoselec (Varaždin)</option>
    </select>
  </div>

  <div id="divdf3">
    <img id="df3" src="playertemplate.png">
    <select id="selectdf3" v-on:change="counterdf3(); showButton(); bodovidf3();" onchange="document.getElementById('df3').src = this.value">
      <option value="playertemplate.png">Odaberite Stopera</option>
      <option value="dperic.png">Dino Perić (Dinamo Zagreb)</option>
      <option value="ktheophilecatherine.png">Kevin Theophile-Catherine (Dinamo Zagreb)</option>
      <option value="edilaver.png">Emir Dilaver (Dinamo Zagreb)</option>
      <option value="jgvardiol.png">Joško Gvardiol (Dinamo Zagreb)</option>
      <option value="vsoldo.png">Vinko Soldo (Dinamo Zagreb)</option>
      <option value="jsutalo.png">Josip Šutalo (Dinamo Zagreb)</option>
      <option value="bfranjic.png">Bartol Franjić (Dinamo Zagreb)</option>
      <option value="ssimic.png">Stefan Simić (Hajduk Split)</option>
      <option value="aismajli.png">Ardian Ismajli (Hajduk Split)</option>
      <option value="nmujakic.png">Nihad Mujakić (Hajduk Split)</option>
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
      <option value="ajovicic.png">Aleksandar Jovičić (Gorica)</option>
      <option value="kkrizmanic.png">Krešimir Krizmanić (Gorica)</option>
      <option value="msteenvoorden.png">Matthew Steenvoorden (Gorica)</option>
      <option value="mjcelic.png">Maks Juraj Čelić (Gorica)</option>
      <option value="dkolinger.png">Denis Kolinger (Lokomotiva Zagreb)</option>
      <option value="jmersinaj.png">Jon Mersinaj (Lokomotiva Zagreb)</option>
      <option value="mleskovic.png">Marko Lešković (Lokomotiva Zagreb)</option>
      <option value="dkovacic.png">Dominik Kovačić (Lokomotiva Zagreb)</option>
      <option value="djokovic.png">Dušan Joković (Lokomotiva Zagreb)</option>
      <option value="msuto.png">Mate Šuto (Lokomotiva Zagreb)</option>
      <option value="npejovic.png">Nikola Pejović (Lokomotiva Zagreb)</option>
      <option value="lovric.png">Ivan Lovrić (Lokomotiva Zagreb)</option>
      <option value="lsmoljo.png">Luka Smoljo (Lokomotiva Zagreb)</option>
      <option value="ffilipovic.png">Frano Filipović (Lokomotiva Zagreb)</option>
      <option value="franklin.png">Franklin (Lokomotiva Zagreb)</option>
      <option value="bmikulic.png">Božo Mikulić (Slaven Belupo)</option>
      <option value="vmedimorec.png">Vinko Međimorec (Slaven Belupo)</option>
      <option value="mzirdum.png">Matko Zirdum (Slaven Belupo)</option>
      <option value="tbozic.png">Tomislav Božić (Slaven Belupo)</option>
      <option value="fhlevnjak.png">Filip Hlevnjak (Slaven Belupo)</option>
      <option value="nsoldo.png">Nikola Soldo (Inter Zaprešić)</option>
      <option value="dvanbruggen.png">Damian van Bruggen (Inter Zaprešić)</option>
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
      <option value="inovoselec.png">Ivan Novoselec (Varaždin)</option>
    </select>
  </div>

  <div id="divdf4">
    <img id="df4" src="playertemplate.png">
    <select id="selectdf4" v-on:change="counterdf4(); showButton(); bodovidf4();" onchange="document.getElementById('df4').src = this.value">
      <option value="playertemplate.png">Odaberite Desnog Beka</option>
      <option value="pstojanovic.png">Petar Stojanović (Dinamo Zagreb)</option>
      <option value="smoharrami.png">Sadegh Moharrami (Dinamo Zagreb)</option>
      <option value="thrvoj.png">Tin Hrvoj (Dinamo Zagreb)</option>
      <option value="jjuranovic.png">Josip Juranović (Hajduk Split)</option>
      <option value="jbasic.png">Josip Bašić (Hajduk Split)</option>
      <option value="itomecak.png">Ivan Tomečak (Rijeka)</option>
      <option value="mraspopovic.png">Momčilo Raspopović (Rijeka)</option>
      <option value="mpavelic.png">Mario Pavelić (Rijeka)</option>
      <option value="isilva.png">Igor Silva (Osijek)</option>
      <option value="agrgic.png">Alen Grgić (Osijek)</option>
      <option value="tsorsa.png">Tomislav Šorša (Osijek)</option>
      <option value="ttodoroski.png">Todor Todoroski (Osijek)</option>
      <option value="mmuhammed.png">Musa Muhammed (Gorica)</option>
      <option value="pperisa.png">Patrik Periša (Gorica)</option>
      <option value="fkaracic.png">Fran Karačić (Lokomotiva Zagreb)</option>
      <option value="pgluhakovic.png">Petar Gluhaković (Lokomotiva Zagreb)</option>
      <option value="mjuric.png">Marko Jurić (Lokomotiva Zagreb)</option>
      <option value="mkaramarko.png">Marko Karamarko (Slaven Belupo)</option>
      <option value="miharos.png">Marko Iharoš (Slaven Belupo)</option>
      <option value="mrom.png">Matija Rom (Inter Zaprešić)</option>
      <option value="abosec.png">Antonio Bosec (Inter Zaprešić)</option>
      <option value="gbaric.png">Gordan Barić (Inter Zaprešić)</option>
      <option value="mgrujevic.png">Marin Grujević (Istra 1961)</option>
      <option value="mfranic.png">Martin Franić (Istra 1961)</option>
      <option value="ntkalcic.png">Nikola Tkalčić (Varaždin)</option>
      <option value="dperkovic.png">Dominik Perković (Varaždin)</option>
      <option value="ftomaskovic.png">Filip Tomašković (Varaždin)</option>
    </select>
  </div>

  <div id="divgk1">
    <img id="gk1" src="playertemplate.png">
    <select id="selectgk1" v-on:change="countergk1(); showButton(); bodovigk1();" onchange="document.getElementById('gk1').src = this.value">
      <option value="playertemplate.png">Odaberite Vratara</option>
      <option value="dlivakovic.png">Dominik Livaković (Dinamo Zagreb)</option>
      <option value="dzagorac.png">Danijel Zagorac (Dinamo Zagreb)</option>
      <option value="jposavec.png">Josip Posavec (Hajduk Split)</option>
      <option value="mljubic.png">Marin Ljubić (Hajduk Split)</option>
      <option value="gblazevic.png">Goran Blažević (Hajduk Split)</option>
      <option value="aprskalo.png">Andrej Prskalo (Rijeka)</option>
      <option value="ipandur.png">Ivor Pandur (Rijeka)</option>
      <option value="dnwolokor.png">David Nwolokor (Rijeka)</option>
      <option value="iivusic.png">Ivica Ivušić (Osijek)</option>
      <option value="mmalenica.png">Marko Malenica (Osijek)</option>
      <option value="kkahlina.png">Kristijan Kahlina (Gorica)</option>
      <option value="icovic.png">Ivan Čović (Gorica)</option>
      <option value="lisek.png">Leon Išek (Gorica)</option>
      <option value="igrbic.png">Ivo Grbić (Lokomotiva Zagreb)</option>
      <option value="khendija.png">Krunoslav Hendija (Lokomotiva Zagreb)</option>
      <option value="mkramer.png">Matko Kramer (Lokomotiva Zagreb)</option>
      <option value="ifilipovic.png">Ivan Filipović (Slaven Belupo)</option>
      <option value="ajezina.png">Antonio Ježina (Slaven Belupo)</option>
      <option value="dsugic.png">David Šugić (Slaven Belupo)</option>
      <option value="ohadzikic.png">Osman Hadžikić (Inter Zaprešić)</option>
      <option value="zfrelih.png">Žiga Frelih (Inter Zaprešić)</option>
      <option value="mmatkovic.png">Mladen Matković (Inter Zaprešić)</option>
      <option value="ikelava.png">Ivan Kelava (Inter Zaprešić)</option>
      <option value="cberkovic.png">Carlo Berković (Inter Zaprešić)</option>
      <option value="jcondric.png">Josip Čondrić (Istra 1961)</option>
      <option value="tduka.png">Tomislav Duka (Istra 1961)</option>
      <option value="lmajkic.png">Lovro Majkić (Istra 1961)</option>
      <option value="inevistic.png">Ivan Nevistić (Varaždin)</option>
      <option value="amrmic.png">Ante Mrmić (Varaždin)</option>
    </select>
  </div>

<button
  id="Button" disabled
  v-on:click="savestats(); savedb();">
    ZAKLJUČAJ TIM
</button>

<button
  v-on:click="savestats(); refresh();"
  id="tipkaupdate">
    AŽURIRAJ PODATKE
</button>

<table id="stattable">
  <tr>
    <th></th>
    <th></th>
    <th id="stathdr">KLUB</th>
    <th id="stathdr">ODIGRANI SUSRETI</th>
    <th id="stathdr">POBJEDE</th>
    <th id="stathdr">NERIJEŠENE</th>
    <th id="stathdr">PORAZI</th>
    <th id="stathdr">BODOVI</th>
  </tr>
  <tr>
    <th></th>
    <th></th>
    <th id="stathdr">{{ myteam }}</th>
    <th id="stathdr">{{ played }}</th>
    <th id="stathdr">{{ wins }}</th>
    <th id="stathdr">{{ draws }}</th>
    <th id="stathdr">{{ losses }}</th>
    <th id="stathdr">{{ points }}</th>
  </tr>
  
</table>

  </div>
</template>

<style>
  #jumboteam{
    padding:0.5em;
    background-repeat:no-repeat;
    background-size: 1710px 1080px;
    height:900px;
    background-position: left
  }
  #naslovteam{
    font-family:Cuprum;
    text-align:center;
    margin-right:100px;
    color: black;
    font-size:90px;
  }
  #divfw1{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:793px;
  }
  #selectfw1{
    font-size:20px;
    position:absolute;
    left:826px;
    width:284px;
  }
  #divfw2{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:500px;
  }
  #selectfw2{
    font-size:20px;
    position:absolute;
    left:1119px;
    top:27px;
    width:284px;
  }
  #divfw3{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:1085px;
  }
  #selectfw3{
    font-size:20px;
    position:absolute;
    left:534px;
    top:54px;
    width:284px;
  }
  #divmf1{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:520px;
    top:370px;
  }
  #selectmf1{
    font-size:20px;
    position:absolute;
    left:1099px;
    bottom:32px;
    width:284px;
  }
  #divmf2{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:795px;
    top:380px;
  }
  #selectmf2{
    font-size:20px;
    position:absolute;
    left:824px;
    bottom:15px;
    width:284px;
  }
  #divmf3{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:1075px;
    top:370px;
  }
  #selectmf3{
    font-size:20px;
    position:absolute;
    left:544px;
    top:-5px;
    width:284px;
  }
  #divdf1{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:350px;
    top:535px;
  }
  #selectdf1{
    font-size:20px;
    position:absolute;
    left:1269px;
    top:-143px;
    width:284px;
  }
  #divdf2{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:630px;
    top:540px;
  }
  #selectdf2{
    font-size:20px;
    position:absolute;
    left:989px;
    top:-121px;
    width:284px;
  }
  #divdf3{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:948px;
    top:540px;
  }
  #selectdf3{
    font-size:20px;
    position:absolute;
    left:671px;
    top:-94px;
    width:284px;
  }
  #divdf4{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:1240px;
    top:540px;
  }
  #selectdf4{
    font-size:20px;
    position:absolute;
    left:379px;
    top:-67px;
    width:284px;
  }
  #divgk1{
    text-align:center;
    font-size:40px;
    font-family:Cuprum;
    color:black;
    width:image width px;
    position:absolute;
    left:797px;
    top:640px;
  }
  #selectgk1{
    font-size:20px;
    position:absolute;
    left:822px;
    top:-140px;
    width:284px;
  }
  #fw1{
    position:absolute;
  }
  #fw2{
    position:absolute;
    top:50px;
  }
  #fw3{
    position:absolute;
    top:50px;
  }
  #mf1{
    position:absolute;
    top:50px;
  }
  #mf2{
    position:absolute;
    top:50px;
  }
  #mf3{
    position:absolute;
    top:50px;
  }
  #df1{
    position:absolute;
    top:50px;
  }
  #df2{
    position:absolute;
    top:50px;
  }
  #df3{
    position:absolute;
    top:50px;
  }
  #df4{
    position:absolute;
    top:50px;
  }
  #gk1{
    position:absolute;
    top:50px;
  }
  #Button{
    font-family:Cuprum;
    font-size:28px;
    position:absolute;
    left:1675px;
    top:550px;
  }
  #tipkaupdate{
    font-family:Cuprum;
    font-size:28px;
    position:absolute;
    left:1675px;
    top:620px;
  }
  #stattable{
    width:56%;
    font-family:Cuprum;
    font-size:28px;
    margin-left:320px;
    color:black;
    margin-top:650px;
  }
  #stathdr{
    font-size:30px;
    text-align:center;
    padding-right:100px;
  }
</style>

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
    var mf1w1,mf1w2,mf1w3,mf1w4,mf1w5,mf1w6,mf1w7,mf1w8,mf1w9,mf1w10,mf1w11,mf1w12,mf1w13,mf1w14,mf1w15,mf1w16,mf1w17,mf1w18,mf1w19;
    var mf2w1,mf2w2,mf2w3,mf2w4,mf2w5,mf2w6,mf2w7,mf2w8,mf2w9,mf2w10,mf2w11,mf2w12,mf2w13,mf2w14,mf2w15,mf2w16,mf2w17,mf2w18,mf2w19;
    var mf3w1,mf3w2,mf3w3,mf3w4,mf3w5,mf3w6,mf3w7,mf3w8,mf3w9,mf3w10,mf3w11,mf3w12,mf3w13,mf3w14,mf3w15,mf3w16,mf3w17,mf3w18,mf3w19;
    var df1w1,df1w2,df1w3,df1w4,df1w5,df1w6,df1w7,df1w8,df1w9,df1w10,df1w11,df1w12,df1w13,df1w14,df1w15,df1w16,df1w17,df1w18,df1w19;
    var df2w1,df2w2,df2w3,df2w4,df2w5,df2w6,df2w7,df2w8,df2w9,df2w10,df2w11,df2w12,df2w13,df2w14,df2w15,df2w16,df2w17,df2w18,df2w19;
    var df3w1,df3w2,df3w3,df3w4,df3w5,df3w6,df3w7,df3w8,df3w9,df3w10,df3w11,df3w12,df3w13,df3w14,df3w15,df3w16,df3w17,df3w18,df3w19;
    var df4w1,df4w2,df4w3,df4w4,df4w5,df4w6,df4w7,df4w8,df4w9,df4w10,df4w11,df4w12,df4w13,df4w14,df4w15,df4w16,df4w17,df4w18,df4w19;
    var gk1w1,gk1w2,gk1w3,gk1w4,gk1w5,gk1w6,gk1w7,gk1w8,gk1w9,gk1w10,gk1w11,gk1w12,gk1w13,gk1w14,gk1w15,gk1w16,gk1w17,gk1w18,gk1w19;
    var pobjede=0;
    var nerijesene=0;
    var porazi=0;
    var odigrani=0;
    var bodovi=0;
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
            if((document.getElementById('selectfw1').value=="bpetkovic.png")||
              (document.getElementById('selectfw1').value=="mgavranovic.png")||
              (document.getElementById('selectfw1').value=="skulenovic.png")||
              (document.getElementById('selectfw1').value=="kandric.png")||
              (document.getElementById('selectfw1').value=="mcuze.png")||
              (document.getElementById('selectfw1').value=="rbaturina.png")||
              (document.getElementById('selectfw1').value=="lsipos.png")){
              fw1w1=3;
              fw1w2=3;
              fw1w3=3;
              fw1w4=1;
              fw1w5=3;
              fw1w6=3;
              fw1w7=0;
              fw1w8=3;
              fw1w9=0;
              fw1w10=3;
              fw1w11=3;
              fw1w12=3;
              fw1w13=3;
              fw1w14=3;
              fw1w15=3;
              fw1w16=1;
              fw1w17=3;
              fw1w18=3;
              fw1w19=3;
            }
            else if((document.getElementById('selectfw1').value=="mjakolis.png")||
              (document.getElementById('selectfw1').value=="idelic.png")||
              (document.getElementById('selectfw1').value=="lkrekovic.png")){
              fw1w1=3;
              fw1w2=3;
              fw1w3=3;
              fw1w4=0;
              fw1w5=3;
              fw1w6=0;
              fw1w7=3;
              fw1w8=1;
              fw1w9=3;
              fw1w10=1;
              fw1w11=3;
              fw1w12=1;
              fw1w13=3;
              fw1w14=0;
              fw1w15=3;
              fw1w16=1;
              fw1w17=0;
              fw1w18=1;
              fw1w19=3;
            }
            else if((document.getElementById('selectfw1').value=="amcolak.png")||
              (document.getElementById('selectfw1').value=="jpuljic.png")||
              (document.getElementById('selectfw1').value=="mbabic.png")||
              (document.getElementById('selectfw1').value=="mmatulja.png")){
              fw1w1=3;
              fw1w2=3;
              fw1w3=3;
              fw1w4=0;
              fw1w5=1;
              fw1w6=0;
              fw1w7=1;
              fw1w8=1;
              fw1w9=3;
              fw1w10=3;
              fw1w11=1;
              fw1w12=3;
              fw1w13=0;
              fw1w14=0;
              fw1w15=0;
              fw1w16=3;
              fw1w17=3;
              fw1w18=3;
              fw1w19=3;
            }
            else if((document.getElementById('selectfw1').value=="mmaric.png")||
              (document.getElementById('selectfw1').value=="amance.png")||
              (document.getElementById('selectfw1').value=="jmbakogu.png")||
              (document.getElementById('selectfw1').value=="jspoljaric.png")||
              (document.getElementById('selectfw1').value=="ddrenabeljo.png")){
              fw1w1=3;
              fw1w2=0;
              fw1w3=3;
              fw1w4=1;
              fw1w5=1;
              fw1w6=3;
              fw1w7=1;
              fw1w8=1;
              fw1w9=0;
              fw1w10=3;
              fw1w11=3;
              fw1w12=1;
              fw1w13=0;
              fw1w14=3;
              fw1w15=0;
              fw1w16=3;
              fw1w17=1;
              fw1w18=3;
              fw1w19=3;
            }
            else if((document.getElementById('selectfw1').value=="cndiaye.png")||
              (document.getElementById('selectfw1').value=="lzwolinski.png")){
              fw1w1=1;
              fw1w2=3;
              fw1w3=0;
              fw1w4=3;
              fw1w5=0;
              fw1w6=1;
              fw1w7=3;
              fw1w8=1;
              fw1w9=0;
              fw1w10=3;
              fw1w11=0;
              fw1w12=0;
              fw1w13=3;
              fw1w14=3;
              fw1w15=1;
              fw1w16=3;
              fw1w17=0;
              fw1w18=3;
              fw1w19=1;
            }
            else if((document.getElementById('selectfw1').value=="mbudimir.png")||
              (document.getElementById('selectfw1').value=="ituci.png")||
              (document.getElementById('selectfw1').value=="drakic.png")||
              (document.getElementById('selectfw1').value=="lmaruzin.png")){
              fw1w1=0;
              fw1w2=0;
              fw1w3=0;
              fw1w4=3;
              fw1w5=1;
              fw1w6=3;
              fw1w7=3;
              fw1w8=1;
              fw1w9=3;
              fw1w10=0;
              fw1w11=1;
              fw1w12=1;
              fw1w13=3;
              fw1w14=3;
              fw1w15=3;
              fw1w16=0;
              fw1w17=3;
              fw1w18=0;
              fw1w19=0;
            }
            else if((document.getElementById('selectfw1').value=="mdelic.png")||
              (document.getElementById('selectfw1').value=="mmladen.png")||
              (document.getElementById('selectfw1').value=="msego.png")||
              (document.getElementById('selectfw1').value=="fetoundi.png")||
              (document.getElementById('selectfw1').value=="mateus.png")||
              (document.getElementById('selectfw1').value=="ikrstanovic.png")){
              fw1w1=0;
              fw1w2=0;
              fw1w3=0;
              fw1w4=3;
              fw1w5=3;
              fw1w6=1;
              fw1w7=0;
              fw1w8=0;
              fw1w9=3;
              fw1w10=0;
              fw1w11=0;
              fw1w12=0;
              fw1w13=0;
              fw1w14=1;
              fw1w15=1;
              fw1w16=3;
              fw1w17=3;
              fw1w18=0;
              fw1w19=0;
            }
            else if((document.getElementById('selectfw1').value=="akaluderovic.png")||
              (document.getElementById('selectfw1').value=="imamut.png")||
              (document.getElementById('selectfw1').value=="mvasilj.png")||
              (document.getElementById('selectfw1').value=="wtchuameni.png")||
              (document.getElementById('selectfw1').value=="bbilobrk.png")||
              (document.getElementById('selectfw1').value=="mbencic.png")){
              fw1w1=1;
              fw1w2=0;
              fw1w3=0;
              fw1w4=1;
              fw1w5=0;
              fw1w6=0;
              fw1w7=1;
              fw1w8=3;
              fw1w9=0;
              fw1w10=0;
              fw1w11=1;
              fw1w12=1;
              fw1w13=3;
              fw1w14=0;
              fw1w15=0;
              fw1w16=0;
              fw1w17=0;
              fw1w18=1;
              fw1w19=1;
            }
            else if((document.getElementById('selectfw1').value=="klaukzemis.png")||
              (document.getElementById('selectfw1').value=="rperickomsic.png")||
              (document.getElementById('selectfw1').value=="afuentes.png")){
              fw1w1=0;
              fw1w2=3;
              fw1w3=3;
              fw1w4=0;
              fw1w5=0;
              fw1w6=1;
              fw1w7=1;
              fw1w8=0;
              fw1w9=0;
              fw1w10=1;
              fw1w11=1;
              fw1w12=0;
              fw1w13=0;
              fw1w14=1;
              fw1w15=1;
              fw1w16=0;
              fw1w17=0;
              fw1w18=0;
              fw1w19=0;
            }
            else if((document.getElementById('selectfw1').value=="vlisakovich.png")||
              (document.getElementById('selectfw1').value=="lbenko.png")||
              (document.getElementById('selectfw1').value=="dglavina.png")||
              (document.getElementById('selectfw1').value=="pkesse.png")){
              fw1w1=0;
              fw1w2=0;
              fw1w3=0;
              fw1w4=1;
              fw1w5=1;
              fw1w6=1;
              fw1w7=0;
              fw1w8=1;
              fw1w9=3;
              fw1w10=0;
              fw1w11=0;
              fw1w12=3;
              fw1w13=0;
              fw1w14=0;
              fw1w15=1;
              fw1w16=0;
              fw1w17=1;
              fw1w18=0;
              fw1w19=0;
            }
          },
          bodovifw2(){
            if((document.getElementById('selectfw2').value=="morsic.png")||
              (document.getElementById('selectfw2').value=="iatiemwen.png")||
              (document.getElementById('selectfw2').value=="amarin.png")){
              fw2w1=3;
              fw2w2=3;
              fw2w3=3;
              fw2w4=1;
              fw2w5=3;
              fw2w6=3;
              fw2w7=0;
              fw2w8=3;
              fw2w9=0;
              fw2w10=3;
              fw2w11=3;
              fw2w12=3;
              fw2w13=3;
              fw2w14=3;
              fw2w15=3;
              fw2w16=1;
              fw2w17=3;
              fw2w18=3;
              fw2w19=3;
            }
            else if((document.getElementById('selectfw2').value=="jairo.png")||
              (document.getElementById('selectfw2').value=="idolcek.png")||
              (document.getElementById('selectfw2').value=="esahiti.png")){
              fw2w1=3;
              fw2w2=3;
              fw2w3=3;
              fw2w4=0;
              fw2w5=3;
              fw2w6=0;
              fw2w7=3;
              fw2w8=1;
              fw2w9=3;
              fw2w10=1;
              fw2w11=3;
              fw2w12=1;
              fw2w13=3;
              fw2w14=0;
              fw2w15=3;
              fw2w16=1;
              fw2w17=0;
              fw2w18=1;
              fw2w19=3;
            }
            else if((document.getElementById('selectfw2').value=="agorgon.png")||
              (document.getElementById('selectfw2').value=="mvuk.png")){
              fw2w1=3;
              fw2w2=3;
              fw2w3=3;
              fw2w4=0;
              fw2w5=1;
              fw2w6=0;
              fw2w7=1;
              fw2w8=1;
              fw2w9=3;
              fw2w10=3;
              fw2w11=1;
              fw2w12=3;
              fw2w13=0;
              fw2w14=0;
              fw2w15=0;
              fw2w16=3;
              fw2w17=3;
              fw2w18=3;
              fw2w19=3;
            }
            else if((document.getElementById('selectfw2').value=="pbockaj.png")||
              (document.getElementById('selectfw2').value=="mndockyt.png")||
              (document.getElementById('selectfw2').value=="mpilj.png")){
              fw2w1=3;
              fw2w2=0;
              fw2w3=3;
              fw2w4=1;
              fw2w5=1;
              fw2w6=3;
              fw2w7=1;
              fw2w8=1;
              fw2w9=0;
              fw2w10=3;
              fw2w11=3;
              fw2w12=1;
              fw2w13=0;
              fw2w14=3;
              fw2w15=0;
              fw2w16=3;
              fw2w17=1;
              fw2w18=3;
              fw2w19=3;
            }
            else if((document.getElementById('selectfw2').value=="klovric.png")||
              (document.getElementById('selectfw2').value=="msroler.png")||
              (document.getElementById('selectfw2').value=="dspikic.png")){
              fw2w1=1;
              fw2w2=3;
              fw2w3=0;
              fw2w4=3;
              fw2w5=0;
              fw2w6=1;
              fw2w7=3;
              fw2w8=1;
              fw2w9=0;
              fw2w10=3;
              fw2w11=0;
              fw2w12=0;
              fw2w13=3;
              fw2w14=3;
              fw2w15=1;
              fw2w16=3;
              fw2w17=0;
              fw2w18=3;
              fw2w19=1;
            }
            else if((document.getElementById('selectfw2').value=="muzuni.png")||
              (document.getElementById('selectfw2').value=="jmajic.png")){
              fw2w1=0;
              fw2w2=0;
              fw2w3=0;
              fw2w4=3;
              fw2w5=1;
              fw2w6=3;
              fw2w7=3;
              fw2w8=1;
              fw2w9=3;
              fw2w10=0;
              fw2w11=1;
              fw2w12=1;
              fw2w13=3;
              fw2w14=3;
              fw2w15=3;
              fw2w16=0;
              fw2w17=3;
              fw2w18=0;
              fw2w19=0;
            }
            else if(document.getElementById('selectfw2').value=="dlovren.png"){
              fw2w1=0;
              fw2w2=0;
              fw2w3=0;
              fw2w4=3;
              fw2w5=3;
              fw2w6=1;
              fw2w7=0;
              fw2w8=0;
              fw2w9=3;
              fw2w10=0;
              fw2w11=0;
              fw2w12=0;
              fw2w13=0;
              fw2w14=1;
              fw2w15=1;
              fw2w16=3;
              fw2w17=3;
              fw2w18=0;
              fw2w19=0;
            }
            else if((document.getElementById('selectfw2').value=="sserderov.png")||
              (document.getElementById('selectfw2').value=="ozamouri.png")){
              fw2w1=1;
              fw2w2=0;
              fw2w3=0;
              fw2w4=1;
              fw2w5=0;
              fw2w6=0;
              fw2w7=1;
              fw2w8=3;
              fw2w9=0;
              fw2w10=0;
              fw2w11=1;
              fw2w12=1;
              fw2w13=3;
              fw2w14=0;
              fw2w15=0;
              fw2w16=0;
              fw2w17=0;
              fw2w18=1;
              fw2w19=1;
            }
            else if((document.getElementById('selectfw2').value=="dbusnja.png")||
              (document.getElementById('selectfw2').value=="jmaganjic.png")){
              fw2w1=0;
              fw2w2=3;
              fw2w3=3;
              fw2w4=0;
              fw2w5=0;
              fw2w6=1;
              fw2w7=1;
              fw2w8=0;
              fw2w9=0;
              fw2w10=1;
              fw2w11=1;
              fw2w12=0;
              fw2w13=0;
              fw2w14=1;
              fw2w15=1;
              fw2w16=0;
              fw2w17=0;
              fw2w18=0;
              fw2w19=0;
            }
            else if((document.getElementById('selectfw2').value=="ddrozdek.png")||
              (document.getElementById('selectfw2').value=="lvuk.png")||
              (document.getElementById('selectfw2').value=="kfucak.png")||
              (document.getElementById('selectfw2').value=="vpetkovic.png")){
              fw2w1=0;
              fw2w2=0;
              fw2w3=0;
              fw2w4=1;
              fw2w5=1;
              fw2w6=1;
              fw2w7=0;
              fw2w8=1;
              fw2w9=3;
              fw2w10=0;
              fw2w11=0;
              fw2w12=3;
              fw2w13=0;
              fw2w14=0;
              fw2w15=1;
              fw2w16=0;
              fw2w17=1;
              fw2w18=0;
              fw2w19=0;
            }
          },
          bodovifw3(){
            if((document.getElementById('selectfw3').value=="dkadzior.png")||
              (document.getElementById('selectfw3').value=="ihajrovic.png")){
              fw3w1=3;
              fw3w2=3;
              fw3w3=3;
              fw3w4=1;
              fw3w5=3;
              fw3w6=3;
              fw3w7=0;
              fw3w8=3;
              fw3w9=0;
              fw3w10=3;
              fw3w11=3;
              fw3w12=3;
              fw3w13=3;
              fw3w14=3;
              fw3w15=3;
              fw3w16=1;
              fw3w17=3;
              fw3w18=3;
              fw3w19=3;
            }
            else if((document.getElementById('selectfw3').value=="seduok.png")||
              (document.getElementById('selectfw3').value=="ftahiraj.png")){
              fw3w1=3;
              fw3w2=3;
              fw3w3=3;
              fw3w4=0;
              fw3w5=3;
              fw3w6=0;
              fw3w7=3;
              fw3w8=1;
              fw3w9=3;
              fw3w10=1;
              fw3w11=3;
              fw3w12=1;
              fw3w13=3;
              fw3w14=0;
              fw3w15=3;
              fw3w16=1;
              fw3w17=0;
              fw3w18=1;
              fw3w19=3;
            }
            else if((document.getElementById('selectfw3').value=="macosty.png")||
              (document.getElementById('selectfw3').value=="rmuric.png")){
              fw3w1=3;
              fw3w2=3;
              fw3w3=3;
              fw3w4=0;
              fw3w5=1;
              fw3w6=0;
              fw3w7=1;
              fw3w8=1;
              fw3w9=3;
              fw3w10=3;
              fw3w11=1;
              fw3w12=3;
              fw3w13=0;
              fw3w14=0;
              fw3w15=0;
              fw3w16=3;
              fw3w17=3;
              fw3w18=3;
              fw3w19=3;
            }
            else if(document.getElementById('selectfw3').value=="egrezda.png"){
              fw3w1=3;
              fw3w2=0;
              fw3w3=3;
              fw3w4=1;
              fw3w5=1;
              fw3w6=3;
              fw3w7=1;
              fw3w8=1;
              fw3w9=0;
              fw3w10=3;
              fw3w11=3;
              fw3w12=1;
              fw3w13=0;
              fw3w14=3;
              fw3w15=0;
              fw3w16=3;
              fw3w17=1;
              fw3w18=3;
              fw3w19=3;
            }
            else if((document.getElementById('selectfw3').value=="jmathieu.png")||
              (document.getElementById('selectfw3').value=="mdvornekovic.png")){
              fw3w1=1;
              fw3w2=3;
              fw3w3=0;
              fw3w4=3;
              fw3w5=0;
              fw3w6=1;
              fw3w7=3;
              fw3w8=1;
              fw3w9=0;
              fw3w10=3;
              fw3w11=0;
              fw3w12=0;
              fw3w13=3;
              fw3w14=3;
              fw3w15=1;
              fw3w16=3;
              fw3w17=0;
              fw3w18=3;
              fw3w19=1;
            }
            else if((document.getElementById('selectfw3').value=="lkastrati.png")||
              (document.getElementById('selectfw3').value=="edeocleciano.png")){
              fw3w1=0;
              fw3w2=0;
              fw3w3=0;
              fw3w4=3;
              fw3w5=1;
              fw3w6=3;
              fw3w7=3;
              fw3w8=1;
              fw3w9=3;
              fw3w10=0;
              fw3w11=1;
              fw3w12=1;
              fw3w13=3;
              fw3w14=3;
              fw3w15=3;
              fw3w16=0;
              fw3w17=3;
              fw3w18=0;
              fw3w19=0;
            }
            else if((document.getElementById('selectfw3').value=="bbogojevic.png")||
              (document.getElementById('selectfw3').value=="falidema.png")||
              (document.getElementById('selectfw3').value=="nhavelka.png")){
              fw3w1=0;
              fw3w2=0;
              fw3w3=0;
              fw3w4=3;
              fw3w5=3;
              fw3w6=1;
              fw3w7=0;
              fw3w8=0;
              fw3w9=3;
              fw3w10=0;
              fw3w11=0;
              fw3w12=0;
              fw3w13=0;
              fw3w14=1;
              fw3w15=1;
              fw3w16=3;
              fw3w17=3;
              fw3w18=0;
              fw3w19=0;
            }
            else if(document.getElementById('selectfw3').value=="jmitrovic.png"){
              fw3w1=1;
              fw3w2=0;
              fw3w3=0;
              fw3w4=1;
              fw3w5=0;
              fw3w6=0;
              fw3w7=1;
              fw3w8=3;
              fw3w9=0;
              fw3w10=0;
              fw3w11=1;
              fw3w12=1;
              fw3w13=3;
              fw3w14=0;
              fw3w15=0;
              fw3w16=0;
              fw3w17=0;
              fw3w18=1;
              fw3w19=1;
            }
            else if((document.getElementById('selectfw3').value=="sgrzan.png")||
              (document.getElementById('selectfw3').value=="mmunivrana.png")||
              (document.getElementById('selectfw3').value=="asane.png")){
              fw3w1=0;
              fw3w2=3;
              fw3w3=3;
              fw3w4=0;
              fw3w5=0;
              fw3w6=1;
              fw3w7=1;
              fw3w8=0;
              fw3w9=0;
              fw3w10=1;
              fw3w11=1;
              fw3w12=0;
              fw3w13=0;
              fw3w14=1;
              fw3w15=1;
              fw3w16=0;
              fw3w17=0;
              fw3w18=0;
              fw3w19=0;
            }
            else if((document.getElementById('selectfw3').value=="mmehdikani.png")||
              (document.getElementById('selectfw3').value=="tturcin.png")||
              (document.getElementById('selectfw3').value=="mkolaric.png")){
              fw3w1=0;
              fw3w2=0;
              fw3w3=0;
              fw3w4=1;
              fw3w5=1;
              fw3w6=1;
              fw3w7=0;
              fw3w8=1;
              fw3w9=3;
              fw3w10=0;
              fw3w11=0;
              fw3w12=3;
              fw3w13=0;
              fw3w14=0;
              fw3w15=1;
              fw3w16=0;
              fw3w17=1;
              fw3w18=0;
              fw3w19=0;
            }
          },
          bodovimf1(){
            if((document.getElementById('selectmf1').value=="agojak.png")||
              (document.getElementById('selectmf1').value=="livanusec.png")||
              (document.getElementById('selectmf1').value=="lmajer.png")||
              (document.getElementById('selectmf1').value=="rmiskovic.png")||
              (document.getElementById('selectmf1').value=="aademi.png")||
              (document.getElementById('selectmf1').value=="nmoro.png")||
              (document.getElementById('selectmf1').value=="mdira.png")){
              mf1w1=3;
              mf1w2=3;
              mf1w3=3;
              mf1w4=1;
              mf1w5=3;
              mf1w6=3;
              mf1w7=0;
              mf1w8=3;
              mf1w9=0;
              mf1w10=3;
              mf1w11=3;
              mf1w12=3;
              mf1w13=3;
              mf1w14=3;
              mf1w15=3;
              mf1w16=1;
              mf1w17=3;
              mf1w18=3;
              mf1w19=3;
            }
            else if((document.getElementById('selectmf1').value=="bjradi.png")||
              (document.getElementById('selectmf1').value=="tteklic.png")||
              (document.getElementById('selectmf1').value=="jblagaic.png")||
              (document.getElementById('selectmf1').value=="mcaktas.png")||
              (document.getElementById('selectmf1').value=="hbarry.png")||
              (document.getElementById('selectmf1').value=="dnejasmic.png")||
              (document.getElementById('selectmf1').value=="sjuric.png")||
              (document.getElementById('selectmf1').value=="akalik.png")){
              mf1w1=3;
              mf1w2=3;
              mf1w3=3;
              mf1w4=0;
              mf1w5=3;
              mf1w6=0;
              mf1w7=3;
              mf1w8=1;
              mf1w9=3;
              mf1w10=1;
              mf1w11=3;
              mf1w12=1;
              mf1w13=3;
              mf1w14=0;
              mf1w15=3;
              mf1w16=1;
              mf1w17=0;
              mf1w18=1;
              mf1w19=3;
            }
            else if((document.getElementById('selectmf1').value=="fandrijasevic.png")||
              (document.getElementById('selectmf1').value=="thalilovic.png")||
              (document.getElementById('selectmf1').value=="diglesias.png")||
              (document.getElementById('selectmf1').value=="dpavicic.png")||
              (document.getElementById('selectmf1').value=="sloncar.png")||
              (document.getElementById('selectmf1').value=="ilepinjica.png")||
              (document.getElementById('selectmf1').value=="lcapan.png")||
              (document.getElementById('selectmf1').value=="asvetic.png")){
              mf1w1=3;
              mf1w2=3;
              mf1w3=3;
              mf1w4=0;
              mf1w5=1;
              mf1w6=0;
              mf1w7=1;
              mf1w8=1;
              mf1w9=3;
              mf1w10=3;
              mf1w11=1;
              mf1w12=3;
              mf1w13=0;
              mf1w14=0;
              mf1w15=0;
              mf1w16=3;
              mf1w17=3;
              mf1w18=3;
              mf1w19=3;
            }
            else if((document.getElementById('selectmf1').value=="lkleinheisler.png")||
              (document.getElementById('selectmf1').value=="dlepa.png")||
              (document.getElementById('selectmf1').value=="kkamenar.png")||
              (document.getElementById('selectmf1').value=="vjugovic.png")||
              (document.getElementById('selectmf1').value=="mzaper.png")||
              (document.getElementById('selectmf1').value=="mljubic.png")){
              mf1w1=3;
              mf1w2=0;
              mf1w3=3;
              mf1w4=1;
              mf1w5=1;
              mf1w6=3;
              mf1w7=1;
              mf1w8=1;
              mf1w9=0;
              mf1w10=3;
              mf1w11=3;
              mf1w12=1;
              mf1w13=0;
              mf1w14=3;
              mf1w15=0;
              mf1w16=3;
              mf1w17=1;
              mf1w18=3;
              mf1w19=3;
            }
            else if((document.getElementById('selectmf1').value=="jhamad.png")||
              (document.getElementById('selectmf1').value=="mmaslowski.png")||
              (document.getElementById('selectmf1').value=="jsuk.png")||
              (document.getElementById('selectmf1').value=="icepo.png")||
              (document.getElementById('selectmf1').value=="dcanadija.png")||
              (document.getElementById('selectmf1').value=="hbabec.png")||
              (document.getElementById('selectmf1').value=="mmaloca.png")||
              (document.getElementById('selectmf1').value=="pgolubickas.png")){
              mf1w1=1;
              mf1w2=3;
              mf1w3=0;
              mf1w4=3;
              mf1w5=0;
              mf1w6=1;
              mf1w7=3;
              mf1w8=1;
              mf1w9=0;
              mf1w10=3;
              mf1w11=0;
              mf1w12=0;
              mf1w13=3;
              mf1w14=3;
              mf1w15=1;
              mf1w16=3;
              mf1w17=0;
              mf1w18=3;
              mf1w19=1;
            }
            else if((document.getElementById('selectmf1').value=="mtolic.png")||
              (document.getElementById('selectmf1').value=="sammir.png")||
              (document.getElementById('selectmf1').value=="fvojkovic.png")||
              (document.getElementById('selectmf1').value=="sgorican.png")||
              (document.getElementById('selectmf1').value=="dhalilovic.png")||
              (document.getElementById('selectmf1').value=="passane.png")||
              (document.getElementById('selectmf1').value=="kjakic.png")||
              (document.getElementById('selectmf1').value=="ecokaj.png")||
              (document.getElementById('selectmf1').value=="opetrak.png")||
              (document.getElementById('selectmf1').value=="tbrezina.png")||
              (document.getElementById('selectmf1').value=="acarapina.png")||
              (document.getElementById('selectmf1').value=="bkaroglan.png")){
              mf1w1=0;
              mf1w2=0;
              mf1w3=0;
              mf1w4=3;
              mf1w5=1;
              mf1w6=3;
              mf1w7=3;
              mf1w8=1;
              mf1w9=3;
              mf1w10=0;
              mf1w11=1;
              mf1w12=1;
              mf1w13=3;
              mf1w14=3;
              mf1w15=3;
              mf1w16=0;
              mf1w17=3;
              mf1w18=0;
              mf1w19=0;
            }
            else if((document.getElementById('selectmf1').value=="klulic.png")||
              (document.getElementById('selectmf1').value=="nglavcic.png")||
              (document.getElementById('selectmf1').value=="sbacelicgrgic.png")||
              (document.getElementById('selectmf1').value=="dpuclin.png")||
              (document.getElementById('selectmf1').value=="gparacki.png")||
              (document.getElementById('selectmf1').value=="rkamber.png")||
              (document.getElementById('selectmf1').value=="tsrbljinovic.png")||
              (document.getElementById('selectmf1').value=="abrkovic.png")){
              mf1w1=0;
              mf1w2=0;
              mf1w3=0;
              mf1w4=3;
              mf1w5=3;
              mf1w6=1;
              mf1w7=0;
              mf1w8=0;
              mf1w9=3;
              mf1w10=0;
              mf1w11=0;
              mf1w12=0;
              mf1w13=0;
              mf1w14=1;
              mf1w15=1;
              mf1w16=3;
              mf1w17=3;
              mf1w18=0;
              mf1w19=0;
            }
            else if((document.getElementById('selectmf1').value=="btsonev.png")||
              (document.getElementById('selectmf1').value=="ipostonjski.png")||
              (document.getElementById('selectmf1').value=="fmlinar.png")||
              (document.getElementById('selectmf1').value=="tmazalovic.png")||
              (document.getElementById('selectmf1').value=="smarasovic.png")||
              (document.getElementById('selectmf1').value=="aspoljaric.png")){
              mf1w1=1;
              mf1w2=0;
              mf1w3=0;
              mf1w4=1;
              mf1w5=0;
              mf1w6=0;
              mf1w7=1;
              mf1w8=3;
              mf1w9=0;
              mf1w10=0;
              mf1w11=1;
              mf1w12=1;
              mf1w13=3;
              mf1w14=0;
              mf1w15=0;
              mf1w16=0;
              mf1w17=0;
              mf1w18=1;
              mf1w19=1;
            }
            else if((document.getElementById('selectmf1').value=="robeng.png")||
              (document.getElementById('selectmf1').value=="imocinic.png")||
              (document.getElementById('selectmf1').value=="egalilea.png")||
              (document.getElementById('selectmf1').value=="sblagojevic.png")||
              (document.getElementById('selectmf1').value=="aivancic.png")||
              (document.getElementById('selectmf1').value=="sloncar2.png")||
              (document.getElementById('selectmf1').value=="tburic.png")||
              (document.getElementById('selectmf1').value=="opaez.png")||
              (document.getElementById('selectmf1').value=="dsadiku.png")){
              mf1w1=0;
              mf1w2=3;
              mf1w3=3;
              mf1w4=0;
              mf1w5=0;
              mf1w6=1;
              mf1w7=1;
              mf1w8=0;
              mf1w9=0;
              mf1w10=1;
              mf1w11=1;
              mf1w12=0;
              mf1w13=0;
              mf1w14=1;
              mf1w15=1;
              mf1w16=0;
              mf1w17=0;
              mf1w18=0;
              mf1w19=0;
            }
            else if((document.getElementById('selectmf1').value=="dglavica.png")||
              (document.getElementById('selectmf1').value=="iposavec.png")||
              (document.getElementById('selectmf1').value=="ktezak.png")||
              (document.getElementById('selectmf1').value=="syokoyama.png")||
              (document.getElementById('selectmf1').value=="jgueradjou.png")||
              (document.getElementById('selectmf1').value=="ndurasek.png")||
              (document.getElementById('selectmf1').value=="jbajandooh.png")||
              (document.getElementById('selectmf1').value=="iroca.png")){
              mf1w1=0;
              mf1w2=0;
              mf1w3=0;
              mf1w4=1;
              mf1w5=1;
              mf1w6=1;
              mf1w7=0;
              mf1w8=1;
              mf1w9=3;
              mf1w10=0;
              mf1w11=0;
              mf1w12=3;
              mf1w13=0;
              mf1w14=0;
              mf1w15=1;
              mf1w16=0;
              mf1w17=1;
              mf1w18=0;
              mf1w19=0;
            }
          },
          bodovimf2(){
            if((document.getElementById('selectmf2').value=="dolmo.png")||
              (document.getElementById('selectmf2').value=="agojak.png")||
              (document.getElementById('selectmf2').value=="livanusec.png")||
              (document.getElementById('selectmf2').value=="lmajer.png")||
              (document.getElementById('selectmf2').value=="rmiskovic.png")||
              (document.getElementById('selectmf2').value=="aademi.png")||
              (document.getElementById('selectmf2').value=="nmoro.png")||
              (document.getElementById('selectmf2').value=="mdira.png")){
              mf2w1=3;
              mf2w2=3;
              mf2w3=3;
              mf2w4=1;
              mf2w5=3;
              mf2w6=3;
              mf2w7=0;
              mf2w8=3;
              mf2w9=0;
              mf2w10=3;
              mf2w11=3;
              mf2w12=3;
              mf2w13=3;
              mf2w14=3;
              mf2w15=3;
              mf2w16=1;
              mf2w17=3;
              mf2w18=3;
              mf2w19=3;
            }
            else if((document.getElementById('selectmf2').value=="bjradi.png")||
              (document.getElementById('selectmf2').value=="tteklic.png")||
              (document.getElementById('selectmf2').value=="jblagaic.png")||
              (document.getElementById('selectmf2').value=="mcaktas.png")||
              (document.getElementById('selectmf2').value=="hbarry.png")||
              (document.getElementById('selectmf2').value=="dnejasmic.png")||
              (document.getElementById('selectmf2').value=="sjuric.png")||
              (document.getElementById('selectmf2').value=="akalik.png")){
              mf2w1=3;
              mf2w2=3;
              mf2w3=3;
              mf2w4=0;
              mf2w5=3;
              mf2w6=0;
              mf2w7=3;
              mf2w8=1;
              mf2w9=3;
              mf2w10=1;
              mf2w11=3;
              mf2w12=1;
              mf2w13=3;
              mf2w14=0;
              mf2w15=3;
              mf2w16=1;
              mf2w17=0;
              mf2w18=1;
              mf2w19=3;
            }
            else if((document.getElementById('selectmf2').value=="fandrijasevic.png")||
              (document.getElementById('selectmf2').value=="thalilovic.png")||
              (document.getElementById('selectmf2').value=="diglesias.png")||
              (document.getElementById('selectmf2').value=="dpavicic.png")||
              (document.getElementById('selectmf2').value=="sloncar.png")||
              (document.getElementById('selectmf2').value=="ilepinjica.png")||
              (document.getElementById('selectmf2').value=="lcapan.png")||
              (document.getElementById('selectmf2').value=="asvetic.png")){
              mf2w1=3;
              mf2w2=3;
              mf2w3=3;
              mf2w4=0;
              mf2w5=1;
              mf2w6=0;
              mf2w7=1;
              mf2w8=1;
              mf2w9=3;
              mf2w10=3;
              mf2w11=1;
              mf2w12=3;
              mf2w13=0;
              mf2w14=0;
              mf2w15=0;
              mf2w16=3;
              mf2w17=3;
              mf2w18=3;
              mf2w19=3;
            }
            else if((document.getElementById('selectmf2').value=="lkleinheisler.png")||
              (document.getElementById('selectmf2').value=="dlepa.png")||
              (document.getElementById('selectmf2').value=="kkamenar.png")||
              (document.getElementById('selectmf2').value=="vjugovic.png")||
              (document.getElementById('selectmf2').value=="mzaper.png")||
              (document.getElementById('selectmf2').value=="mljubic.png")){
              mf2w1=3;
              mf2w2=0;
              mf2w3=3;
              mf2w4=1;
              mf2w5=1;
              mf2w6=3;
              mf2w7=1;
              mf2w8=1;
              mf2w9=0;
              mf2w10=3;
              mf2w11=3;
              mf2w12=1;
              mf2w13=0;
              mf2w14=3;
              mf2w15=0;
              mf2w16=3;
              mf2w17=1;
              mf2w18=3;
              mf2w19=3;
            }
            else if((document.getElementById('selectmf2').value=="jhamad.png")||
              (document.getElementById('selectmf2').value=="mmaslowski.png")||
              (document.getElementById('selectmf2').value=="jsuk.png")||
              (document.getElementById('selectmf2').value=="icepo.png")||
              (document.getElementById('selectmf2').value=="dcanadija.png")||
              (document.getElementById('selectmf2').value=="hbabec.png")||
              (document.getElementById('selectmf2').value=="mmaloca.png")||
              (document.getElementById('selectmf2').value=="pgolubickas.png")){
              mf2w1=1;
              mf2w2=3;
              mf2w3=0;
              mf2w4=3;
              mf2w5=0;
              mf2w6=1;
              mf2w7=3;
              mf2w8=1;
              mf2w9=0;
              mf2w10=3;
              mf2w11=0;
              mf2w12=0;
              mf2w13=3;
              mf2w14=3;
              mf2w15=1;
              mf2w16=3;
              mf2w17=0;
              mf2w18=3;
              mf2w19=1;
            }
            else if((document.getElementById('selectmf2').value=="mtolic.png")||
              (document.getElementById('selectmf2').value=="sammir.png")||
              (document.getElementById('selectmf2').value=="fvojkovic.png")||
              (document.getElementById('selectmf2').value=="sgorican.png")||
              (document.getElementById('selectmf2').value=="dhalilovic.png")||
              (document.getElementById('selectmf2').value=="passane.png")||
              (document.getElementById('selectmf2').value=="kjakic.png")||
              (document.getElementById('selectmf2').value=="ecokaj.png")||
              (document.getElementById('selectmf2').value=="opetrak.png")||
              (document.getElementById('selectmf2').value=="tbrezina.png")||
              (document.getElementById('selectmf2').value=="acarapina.png")||
              (document.getElementById('selectmf2').value=="bkaroglan.png")){
              mf2w1=0;
              mf2w2=0;
              mf2w3=0;
              mf2w4=3;
              mf2w5=1;
              mf2w6=3;
              mf2w7=3;
              mf2w8=1;
              mf2w9=3;
              mf2w10=0;
              mf2w11=1;
              mf2w12=1;
              mf2w13=3;
              mf2w14=3;
              mf2w15=3;
              mf2w16=0;
              mf2w17=3;
              mf2w18=0;
              mf2w19=0;
            }
            else if((document.getElementById('selectmf2').value=="klulic.png")||
              (document.getElementById('selectmf2').value=="nglavcic.png")||
              (document.getElementById('selectmf2').value=="sbacelicgrgic.png")||
              (document.getElementById('selectmf2').value=="dpuclin.png")||
              (document.getElementById('selectmf2').value=="gparacki.png")||
              (document.getElementById('selectmf2').value=="rkamber.png")||
              (document.getElementById('selectmf2').value=="tsrbljinovic.png")||
              (document.getElementById('selectmf2').value=="abrkovic.png")){
              mf2w1=0;
              mf2w2=0;
              mf2w3=0;
              mf2w4=3;
              mf2w5=3;
              mf2w6=1;
              mf2w7=0;
              mf2w8=0;
              mf2w9=3;
              mf2w10=0;
              mf2w11=0;
              mf2w12=0;
              mf2w13=0;
              mf2w14=1;
              mf2w15=1;
              mf2w16=3;
              mf2w17=3;
              mf2w18=0;
              mf2w19=0;
            }
            else if((document.getElementById('selectmf2').value=="btsonev.png")||
              (document.getElementById('selectmf2').value=="ipostonjski.png")||
              (document.getElementById('selectmf2').value=="fmlinar.png")||
              (document.getElementById('selectmf2').value=="tmazalovic.png")||
              (document.getElementById('selectmf2').value=="smarasovic.png")||
              (document.getElementById('selectmf2').value=="aspoljaric.png")){
              mf2w1=1;
              mf2w2=0;
              mf2w3=0;
              mf2w4=1;
              mf2w5=0;
              mf2w6=0;
              mf2w7=1;
              mf2w8=3;
              mf2w9=0;
              mf2w10=0;
              mf2w11=1;
              mf2w12=1;
              mf2w13=3;
              mf2w14=0;
              mf2w15=0;
              mf2w16=0;
              mf2w17=0;
              mf2w18=1;
              mf2w19=1;
            }
            else if((document.getElementById('selectmf2').value=="robeng.png")||
              (document.getElementById('selectmf2').value=="imocinic.png")||
              (document.getElementById('selectmf2').value=="egalilea.png")||
              (document.getElementById('selectmf2').value=="sblagojevic.png")||
              (document.getElementById('selectmf2').value=="aivancic.png")||
              (document.getElementById('selectmf2').value=="sloncar2.png")||
              (document.getElementById('selectmf2').value=="tburic.png")||
              (document.getElementById('selectmf2').value=="opaez.png")||
              (document.getElementById('selectmf2').value=="dsadiku.png")){
              mf2w1=0;
              mf2w2=3;
              mf2w3=3;
              mf2w4=0;
              mf2w5=0;
              mf2w6=1;
              mf2w7=1;
              mf2w8=0;
              mf2w9=0;
              mf2w10=1;
              mf2w11=1;
              mf2w12=0;
              mf2w13=0;
              mf2w14=1;
              mf2w15=1;
              mf2w16=0;
              mf2w17=0;
              mf2w18=0;
              mf2w19=0;
            }
            else if((document.getElementById('selectmf2').value=="dglavica.png")||
              (document.getElementById('selectmf2').value=="iposavec.png")||
              (document.getElementById('selectmf2').value=="ktezak.png")||
              (document.getElementById('selectmf2').value=="syokoyama.png")||
              (document.getElementById('selectmf2').value=="jgueradjou.png")||
              (document.getElementById('selectmf2').value=="ndurasek.png")||
              (document.getElementById('selectmf2').value=="jbajandooh.png")||
              (document.getElementById('selectmf2').value=="iroca.png")){
              mf2w1=0;
              mf2w2=0;
              mf2w3=0;
              mf2w4=1;
              mf2w5=1;
              mf2w6=1;
              mf2w7=0;
              mf2w8=1;
              mf2w9=3;
              mf2w10=0;
              mf2w11=0;
              mf2w12=3;
              mf2w13=0;
              mf2w14=0;
              mf2w15=1;
              mf2w16=0;
              mf2w17=1;
              mf2w18=0;
              mf2w19=0;
            }
          },
          bodovimf3(){
            if((document.getElementById('selectmf3').value=="dolmo.png")||
              (document.getElementById('selectmf3').value=="agojak.png")||
              (document.getElementById('selectmf3').value=="livanusec.png")||
              (document.getElementById('selectmf3').value=="lmajer.png")||
              (document.getElementById('selectmf3').value=="rmiskovic.png")||
              (document.getElementById('selectmf3').value=="aademi.png")||
              (document.getElementById('selectmf3').value=="nmoro.png")||
              (document.getElementById('selectmf3').value=="mdira.png")){
              mf3w1=3;
              mf3w2=3;
              mf3w3=3;
              mf3w4=1;
              mf3w5=3;
              mf3w6=3;
              mf3w7=0;
              mf3w8=3;
              mf3w9=0;
              mf3w10=3;
              mf3w11=3;
              mf3w12=3;
              mf3w13=3;
              mf3w14=3;
              mf3w15=3;
              mf3w16=1;
              mf3w17=3;
              mf3w18=3;
              mf3w19=3;
            }
            else if((document.getElementById('selectmf3').value=="bjradi.png")||
              (document.getElementById('selectmf3').value=="tteklic.png")||
              (document.getElementById('selectmf3').value=="jblagaic.png")||
              (document.getElementById('selectmf3').value=="mcaktas.png")||
              (document.getElementById('selectmf3').value=="hbarry.png")||
              (document.getElementById('selectmf3').value=="dnejasmic.png")||
              (document.getElementById('selectmf3').value=="sjuric.png")||
              (document.getElementById('selectmf3').value=="akalik.png")){
              mf3w1=3;
              mf3w2=3;
              mf3w3=3;
              mf3w4=0;
              mf3w5=3;
              mf3w6=0;
              mf3w7=3;
              mf3w8=1;
              mf3w9=3;
              mf3w10=1;
              mf3w11=3;
              mf3w12=1;
              mf3w13=3;
              mf3w14=0;
              mf3w15=3;
              mf3w16=1;
              mf3w17=0;
              mf3w18=1;
              mf3w19=3;
            }
            else if((document.getElementById('selectmf3').value=="fandrijasevic.png")||
              (document.getElementById('selectmf3').value=="thalilovic.png")||
              (document.getElementById('selectmf3').value=="diglesias.png")||
              (document.getElementById('selectmf3').value=="dpavicic.png")||
              (document.getElementById('selectmf3').value=="sloncar.png")||
              (document.getElementById('selectmf3').value=="ilepinjica.png")||
              (document.getElementById('selectmf3').value=="lcapan.png")||
              (document.getElementById('selectmf3').value=="asvetic.png")){
              mf3w1=3;
              mf3w2=3;
              mf3w3=3;
              mf3w4=0;
              mf3w5=1;
              mf3w6=0;
              mf3w7=1;
              mf3w8=1;
              mf3w9=3;
              mf3w10=3;
              mf3w11=1;
              mf3w12=3;
              mf3w13=0;
              mf3w14=0;
              mf3w15=0;
              mf3w16=3;
              mf3w17=3;
              mf3w18=3;
              mf3w19=3;
            }
            else if((document.getElementById('selectmf3').value=="lkleinheisler.png")||
              (document.getElementById('selectmf3').value=="dlepa.png")||
              (document.getElementById('selectmf3').value=="kkamenar.png")||
              (document.getElementById('selectmf3').value=="vjugovic.png")||
              (document.getElementById('selectmf3').value=="mzaper.png")||
              (document.getElementById('selectmf3').value=="mljubic.png")){
              mf3w1=3;
              mf3w2=0;
              mf3w3=3;
              mf3w4=1;
              mf3w5=1;
              mf3w6=3;
              mf3w7=1;
              mf3w8=1;
              mf3w9=0;
              mf3w10=3;
              mf3w11=3;
              mf3w12=1;
              mf3w13=0;
              mf3w14=3;
              mf3w15=0;
              mf3w16=3;
              mf3w17=1;
              mf3w18=3;
              mf3w19=3;
            }
            else if((document.getElementById('selectmf3').value=="jhamad.png")||
              (document.getElementById('selectmf3').value=="mmaslowski.png")||
              (document.getElementById('selectmf3').value=="jsuk.png")||
              (document.getElementById('selectmf3').value=="icepo.png")||
              (document.getElementById('selectmf3').value=="dcanadija.png")||
              (document.getElementById('selectmf3').value=="hbabec.png")||
              (document.getElementById('selectmf3').value=="mmaloca.png")||
              (document.getElementById('selectmf3').value=="pgolubickas.png")){
              mf3w1=1;
              mf3w2=3;
              mf3w3=0;
              mf3w4=3;
              mf3w5=0;
              mf3w6=1;
              mf3w7=3;
              mf3w8=1;
              mf3w9=0;
              mf3w10=3;
              mf3w11=0;
              mf3w12=0;
              mf3w13=3;
              mf3w14=3;
              mf3w15=1;
              mf3w16=3;
              mf3w17=0;
              mf3w18=3;
              mf3w19=1;
            }
            else if((document.getElementById('selectmf3').value=="mtolic.png")||
              (document.getElementById('selectmf3').value=="sammir.png")||
              (document.getElementById('selectmf3').value=="fvojkovic.png")||
              (document.getElementById('selectmf3').value=="sgorican.png")||
              (document.getElementById('selectmf3').value=="dhalilovic.png")||
              (document.getElementById('selectmf3').value=="passane.png")||
              (document.getElementById('selectmf3').value=="kjakic.png")||
              (document.getElementById('selectmf3').value=="ecokaj.png")||
              (document.getElementById('selectmf3').value=="opetrak.png")||
              (document.getElementById('selectmf3').value=="tbrezina.png")||
              (document.getElementById('selectmf3').value=="acarapina.png")||
              (document.getElementById('selectmf3').value=="bkaroglan.png")){
              mf3w1=0;
              mf3w2=0;
              mf3w3=0;
              mf3w4=3;
              mf3w5=1;
              mf3w6=3;
              mf3w7=3;
              mf3w8=1;
              mf3w9=3;
              mf3w10=0;
              mf3w11=1;
              mf3w12=1;
              mf3w13=3;
              mf3w14=3;
              mf3w15=3;
              mf3w16=0;
              mf3w17=3;
              mf3w18=0;
              mf3w19=0;
            }
            else if((document.getElementById('selectmf3').value=="klulic.png")||
              (document.getElementById('selectmf3').value=="nglavcic.png")||
              (document.getElementById('selectmf3').value=="sbacelicgrgic.png")||
              (document.getElementById('selectmf3').value=="dpuclin.png")||
              (document.getElementById('selectmf3').value=="gparacki.png")||
              (document.getElementById('selectmf3').value=="rkamber.png")||
              (document.getElementById('selectmf3').value=="tsrbljinovic.png")||
              (document.getElementById('selectmf3').value=="abrkovic.png")){
              mf3w1=0;
              mf3w2=0;
              mf3w3=0;
              mf3w4=3;
              mf3w5=3;
              mf3w6=1;
              mf3w7=0;
              mf3w8=0;
              mf3w9=3;
              mf3w10=0;
              mf3w11=0;
              mf3w12=0;
              mf3w13=0;
              mf3w14=1;
              mf3w15=1;
              mf3w16=3;
              mf3w17=3;
              mf3w18=0;
              mf3w19=0;
            }
            else if((document.getElementById('selectmf3').value=="btsonev.png")||
              (document.getElementById('selectmf3').value=="ipostonjski.png")||
              (document.getElementById('selectmf3').value=="fmlinar.png")||
              (document.getElementById('selectmf3').value=="tmazalovic.png")||
              (document.getElementById('selectmf3').value=="smarasovic.png")||
              (document.getElementById('selectmf3').value=="aspoljaric.png")){
              mf3w1=1;
              mf3w2=0;
              mf3w3=0;
              mf3w4=1;
              mf3w5=0;
              mf3w6=0;
              mf3w7=1;
              mf3w8=3;
              mf3w9=0;
              mf3w10=0;
              mf3w11=1;
              mf3w12=1;
              mf3w13=3;
              mf3w14=0;
              mf3w15=0;
              mf3w16=0;
              mf3w17=0;
              mf3w18=1;
              mf3w19=1;
            }
            else if((document.getElementById('selectmf3').value=="robeng.png")||
              (document.getElementById('selectmf3').value=="imocinic.png")||
              (document.getElementById('selectmf3').value=="egalilea.png")||
              (document.getElementById('selectmf3').value=="sblagojevic.png")||
              (document.getElementById('selectmf3').value=="aivancic.png")||
              (document.getElementById('selectmf3').value=="sloncar2.png")||
              (document.getElementById('selectmf3').value=="tburic.png")||
              (document.getElementById('selectmf3').value=="opaez.png")||
              (document.getElementById('selectmf3').value=="dsadiku.png")){
              mf3w1=0;
              mf3w2=3;
              mf3w3=3;
              mf3w4=0;
              mf3w5=0;
              mf3w6=1;
              mf3w7=1;
              mf3w8=0;
              mf3w9=0;
              mf3w10=1;
              mf3w11=1;
              mf3w12=0;
              mf3w13=0;
              mf3w14=1;
              mf3w15=1;
              mf3w16=0;
              mf3w17=0;
              mf3w18=0;
              mf3w19=0;
            }
            else if((document.getElementById('selectmf3').value=="dglavica.png")||
              (document.getElementById('selectmf3').value=="iposavec.png")||
              (document.getElementById('selectmf3').value=="ktezak.png")||
              (document.getElementById('selectmf3').value=="syokoyama.png")||
              (document.getElementById('selectmf3').value=="jgueradjou.png")||
              (document.getElementById('selectmf3').value=="ndurasek.png")||
              (document.getElementById('selectmf3').value=="jbajandooh.png")||
              (document.getElementById('selectmf3').value=="iroca.png")){
              mf3w1=0;
              mf3w2=0;
              mf3w3=0;
              mf3w4=1;
              mf3w5=1;
              mf3w6=1;
              mf3w7=0;
              mf3w8=1;
              mf3w9=3;
              mf3w10=0;
              mf3w11=0;
              mf3w12=3;
              mf3w13=0;
              mf3w14=0;
              mf3w15=1;
              mf3w16=0;
              mf3w17=1;
              mf3w18=0;
              mf3w19=0;
            }
          },
          bodovidf1(){
            if((document.getElementById('selectdf1').value=="mleovac.png")||
              (document.getElementById('selectdf1').value=="fmoubandje.png")){
              df1w1=3;
              df1w2=3;
              df1w3=3;
              df1w4=1;
              df1w5=3;
              df1w6=3;
              df1w7=0;
              df1w8=3;
              df1w9=0;
              df1w10=3;
              df1w11=3;
              df1w12=3;
              df1w13=3;
              df1w14=3;
              df1w15=3;
              df1w16=1;
              df1w17=3;
              df1w18=3;
              df1w19=3;
            }
            else if(document.getElementById('selectdf1').value=="dcolina.png"){
              df1w1=3;
              df1w2=3;
              df1w3=3;
              df1w4=0;
              df1w5=3;
              df1w6=0;
              df1w7=3;
              df1w8=1;
              df1w9=3;
              df1w10=1;
              df1w11=3;
              df1w12=1;
              df1w13=3;
              df1w14=0;
              df1w15=3;
              df1w16=1;
              df1w17=0;
              df1w18=1;
              df1w19=3;
            }
            else if((document.getElementById('selectdf1').value=="pmamic.png")||
              (document.getElementById('selectdf1').value=="dstefulj.png")||
              (document.getElementById('selectdf1').value=="mkabiru.png")){
              df1w1=3;
              df1w2=3;
              df1w3=3;
              df1w4=0;
              df1w5=1;
              df1w6=0;
              df1w7=1;
              df1w8=1;
              df1w9=3;
              df1w10=3;
              df1w11=1;
              df1w12=3;
              df1w13=0;
              df1w14=0;
              df1w15=0;
              df1w16=3;
              df1w17=3;
              df1w18=3;
              df1w19=3;
            }
            else if((document.getElementById('selectdf1').value=="talys.png")||
              (document.getElementById('selectdf1').value=="lmarin.png")){
              df1w1=3;
              df1w2=0;
              df1w3=3;
              df1w4=1;
              df1w5=1;
              df1w6=3;
              df1w7=1;
              df1w8=1;
              df1w9=0;
              df1w10=3;
              df1w11=3;
              df1w12=1;
              df1w13=0;
              df1w14=3;
              df1w15=0;
              df1w16=3;
              df1w17=1;
              df1w18=3;
              df1w19=3;
            }
            else if(document.getElementById('selectdf1').value=="mcabraja.png"){
              df1w1=1;
              df1w2=3;
              df1w3=0;
              df1w4=3;
              df1w5=0;
              df1w6=1;
              df1w7=3;
              df1w8=1;
              df1w9=0;
              df1w10=3;
              df1w11=0;
              df1w12=0;
              df1w13=3;
              df1w14=3;
              df1w15=1;
              df1w16=3;
              df1w17=0;
              df1w18=3;
              df1w19=1;
            }
            else if((document.getElementById('selectdf1').value=="smarkovic.png")||
              (document.getElementById('selectdf1').value=="bvliet.png")||
              (document.getElementById('selectdf1').value=="srozman.png")||
              (document.getElementById('selectdf1').value=="imilicevic.png")||
              (document.getElementById('selectdf1').value=="icelikovic.png")){
              df1w1=0;
              df1w2=0;
              df1w3=0;
              df1w4=3;
              df1w5=1;
              df1w6=3;
              df1w7=3;
              df1w8=1;
              df1w9=3;
              df1w10=0;
              df1w11=1;
              df1w12=1;
              df1w13=3;
              df1w14=3;
              df1w15=3;
              df1w16=0;
              df1w17=3;
              df1w18=0;
              df1w19=0;
            }
            else if((document.getElementById('selectdf1').value=="bgoda.png")||
              (document.getElementById('selectdf1').value=="mradivojevic.png")||
              (document.getElementById('selectdf1').value=="mmartinaga.png")){
              df1w1=0;
              df1w2=0;
              df1w3=0;
              df1w4=3;
              df1w5=3;
              df1w6=1;
              df1w7=0;
              df1w8=0;
              df1w9=3;
              df1w10=0;
              df1w11=0;
              df1w12=0;
              df1w13=0;
              df1w14=1;
              df1w15=1;
              df1w16=3;
              df1w17=3;
              df1w18=0;
              df1w19=0;
            }
            else if(document.getElementById('selectdf1').value=="svego.png"){
              df1w1=1;
              df1w2=0;
              df1w3=0;
              df1w4=1;
              df1w5=0;
              df1w6=0;
              df1w7=1;
              df1w8=3;
              df1w9=0;
              df1w10=0;
              df1w11=1;
              df1w12=1;
              df1w13=3;
              df1w14=0;
              df1w15=0;
              df1w16=0;
              df1w17=0;
              df1w18=1;
              df1w19=1;
            }
            else if((document.getElementById('selectdf1').value=="mpavic.png")||
              (document.getElementById('selectdf1').value=="sgonzalez.png")){
              df1w1=0;
              df1w2=3;
              df1w3=3;
              df1w4=0;
              df1w5=0;
              df1w6=1;
              df1w7=1;
              df1w8=0;
              df1w9=0;
              df1w10=1;
              df1w11=1;
              df1w12=0;
              df1w13=0;
              df1w14=1;
              df1w15=1;
              df1w16=0;
              df1w17=0;
              df1w18=0;
              df1w19=0;
            }
            else if((document.getElementById('selectdf1').value=="dglavina2.png")||
              (document.getElementById('selectdf1').value=="mspicic.png")||
              (document.getElementById('selectdf1').value=="ksambolec.png")){
              df1w1=0;
              df1w2=0;
              df1w3=0;
              df1w4=1;
              df1w5=1;
              df1w6=1;
              df1w7=0;
              df1w8=1;
              df1w9=3;
              df1w10=0;
              df1w11=0;
              df1w12=3;
              df1w13=0;
              df1w14=0;
              df1w15=1;
              df1w16=0;
              df1w17=1;
              df1w18=0;
              df1w19=0;
            }
          },
          bodovidf2(){
            if((document.getElementById('selectdf2').value=="dperic.png")||
              (document.getElementById('selectdf2').value=="ktheophilecatherine.png")||
              (document.getElementById('selectdf2').value=="edilaver.png")||
              (document.getElementById('selectdf2').value=="jgvardiol.png")||
              (document.getElementById('selectdf2').value=="vsoldo.png")||
              (document.getElementById('selectdf2').value=="jsutalo.png")||
              (document.getElementById('selectdf2').value=="bfranjic.png")){
              df2w1=3;
              df2w2=3;
              df2w3=3;
              df2w4=1;
              df2w5=3;
              df2w6=3;
              df2w7=0;
              df2w8=3;
              df2w9=0;
              df2w10=3;
              df2w11=3;
              df2w12=3;
              df2w13=3;
              df2w14=3;
              df2w15=3;
              df2w16=1;
              df2w17=3;
              df2w18=3;
              df2w19=3;
            }
            else if((document.getElementById('selectdf2').value=="ssimic.png")||
              (document.getElementById('selectdf2').value=="aismajli.png")||
              (document.getElementById('selectdf2').value=="nmujakic.png")||
              (document.getElementById('selectdf2').value=="mvuskovic.png")||
              (document.getElementById('selectdf2').value=="svucur.png")||
              (document.getElementById('selectdf2').value=="sradic.png")||
              (document.getElementById('selectdf2').value=="ldellova.png")){
              df2w1=3;
              df2w2=3;
              df2w3=3;
              df2w4=0;
              df2w5=3;
              df2w6=0;
              df2w7=3;
              df2w8=1;
              df2w9=3;
              df2w10=1;
              df2w11=3;
              df2w12=1;
              df2w13=3;
              df2w14=0;
              df2w15=3;
              df2w16=1;
              df2w17=0;
              df2w18=1;
              df2w19=3;
            }
            else if((document.getElementById('selectdf2').value=="hsmolcic.png")||
              (document.getElementById('selectdf2').value=="ngalovic.png")||
              (document.getElementById('selectdf2').value=="jescoval.png")||
              (document.getElementById('selectdf2').value=="lsimic.png")||
              (document.getElementById('selectdf2').value=="dvelkovski.png")||
              (document.getElementById('selectdf2').value=="jcelikovic.png")||
              (document.getElementById('selectdf2').value=="lmikulica.png")){
              df2w1=3;
              df2w2=3;
              df2w3=3;
              df2w4=0;
              df2w5=1;
              df2w6=0;
              df2w7=1;
              df2w8=1;
              df2w9=3;
              df2w10=3;
              df2w11=1;
              df2w12=3;
              df2w13=0;
              df2w14=0;
              df2w15=0;
              df2w16=3;
              df2w17=3;
              df2w18=3;
              df2w19=3;
            }
            else if((document.getElementById('selectdf2').value=="mskoric.png")||
              (document.getElementById('selectdf2').value=="amajstorovic.png")||
              (document.getElementById('selectdf2').value=="bsutalo.png")||
              (document.getElementById('selectdf2').value=="guti.png")||
              (document.getElementById('selectdf2').value=="dloncar.png")){
              df2w1=3;
              df2w2=0;
              df2w3=3;
              df2w4=1;
              df2w5=1;
              df2w6=3;
              df2w7=1;
              df2w8=1;
              df2w9=0;
              df2w10=3;
              df2w11=3;
              df2w12=1;
              df2w13=0;
              df2w14=3;
              df2w15=0;
              df2w16=3;
              df2w17=1;
              df2w18=3;
              df2w19=3;
            }
            else if((document.getElementById('selectdf2').value=="ajovicic.png")||
              (document.getElementById('selectdf2').value=="kkrizmanic.png")||
              (document.getElementById('selectdf2').value=="msteenvoorden.png")||
              (document.getElementById('selectdf2').value=="mjcelic.png")){
              df2w1=1;
              df2w2=3;
              df2w3=0;
              df2w4=3;
              df2w5=0;
              df2w6=1;
              df2w7=3;
              df2w8=1;
              df2w9=0;
              df2w10=3;
              df2w11=0;
              df2w12=0;
              df2w13=3;
              df2w14=3;
              df2w15=1;
              df2w16=3;
              df2w17=0;
              df2w18=3;
              df2w19=1;
            }
            else if((document.getElementById('selectdf2').value=="dkolinger.png")||
              (document.getElementById('selectdf2').value=="jmersinaj.png")||
              (document.getElementById('selectdf2').value=="mleskovic.png")||
              (document.getElementById('selectdf2').value=="dkovacic.png")||
              (document.getElementById('selectdf2').value=="djokovic.png")||
              (document.getElementById('selectdf2').value=="msuto.png")||
              (document.getElementById('selectdf2').value=="npejovic.png")||
              (document.getElementById('selectdf2').value=="ilovric.png")||
              (document.getElementById('selectdf2').value=="lsmoljo.png")||
              (document.getElementById('selectdf2').value=="ffilipovic.png")||
              (document.getElementById('selectdf2').value=="franklin.png")){
              df2w1=0;
              df2w2=0;
              df2w3=0;
              df2w4=3;
              df2w5=1;
              df2w6=3;
              df2w7=3;
              df2w8=1;
              df2w9=3;
              df2w10=0;
              df2w11=1;
              df2w12=1;
              df2w13=3;
              df2w14=3;
              df2w15=3;
              df2w16=0;
              df2w17=3;
              df2w18=0;
              df2w19=0;
            }
            else if((document.getElementById('selectdf2').value=="bmikulic.png")||
              (document.getElementById('selectdf2').value=="vmedimorec.png")||
              (document.getElementById('selectdf2').value=="mzirdum.png")||
              (document.getElementById('selectdf2').value=="tbozic.png")||
              (document.getElementById('selectdf2').value=="fhlevnjak.png")){
              df2w1=0;
              df2w2=0;
              df2w3=0;
              df2w4=3;
              df2w5=3;
              df2w6=1;
              df2w7=0;
              df2w8=0;
              df2w9=3;
              df2w10=0;
              df2w11=0;
              df2w12=0;
              df2w13=0;
              df2w14=1;
              df2w15=1;
              df2w16=3;
              df2w17=3;
              df2w18=0;
              df2w19=0;
            }
            else if((document.getElementById('selectdf2').value=="nsoldo.png")||
              (document.getElementById('selectdf2').value=="dvanbruggen.png")||
              (document.getElementById('selectdf2').value=="dgrgic.png")||
              (document.getElementById('selectdf2').value=="msavic.png")||
              (document.getElementById('selectdf2').value=="itatomirovic.png")||
              (document.getElementById('selectdf2').value=="inekic.png")||
              (document.getElementById('selectdf2').value=="igrozdek.png")){
              df2w1=1;
              df2w2=0;
              df2w3=0;
              df2w4=1;
              df2w5=0;
              df2w6=0;
              df2w7=1;
              df2w8=3;
              df2w9=0;
              df2w10=0;
              df2w11=1;
              df2w12=1;
              df2w13=3;
              df2w14=0;
              df2w15=0;
              df2w16=0;
              df2w17=0;
              df2w18=1;
              df2w19=1;
            }
            else if((document.getElementById('selectdf2').value=="pbosancic.png")||
              (document.getElementById('selectdf2').value=="jtomasevic.png")||
              (document.getElementById('selectdf2').value=="arufati.png")||
              (document.getElementById('selectdf2').value=="rpaez.png")){
              df2w1=0;
              df2w2=3;
              df2w3=3;
              df2w4=0;
              df2w5=0;
              df2w6=1;
              df2w7=1;
              df2w8=0;
              df2w9=0;
              df2w10=1;
              df2w11=1;
              df2w12=0;
              df2w13=0;
              df2w14=1;
              df2w15=1;
              df2w16=0;
              df2w17=0;
              df2w18=0;
              df2w19=0;
            }
            else if((document.getElementById('selectdf2').value=="fprce.png")||
              (document.getElementById('selectdf2').value=="mstolnik.png")||
              (document.getElementById('selectdf2').value=="msenic.png")||
              (document.getElementById('selectdf2').value=="inovoselec.png")){
              df2w1=0;
              df2w2=0;
              df2w3=0;
              df2w4=1;
              df2w5=1;
              df2w6=1;
              df2w7=0;
              df2w8=1;
              df2w9=3;
              df2w10=0;
              df2w11=0;
              df2w12=3;
              df2w13=0;
              df2w14=0;
              df2w15=1;
              df2w16=0;
              df2w17=1;
              df2w18=0;
              df2w19=0;
            }
          },
          bodovidf3(){
            if((document.getElementById('selectdf3').value=="dperic.png")||
              (document.getElementById('selectdf3').value=="ktheophilecatherine.png")||
              (document.getElementById('selectdf3').value=="edilaver.png")||
              (document.getElementById('selectdf3').value=="jgvardiol.png")||
              (document.getElementById('selectdf3').value=="vsoldo.png")||
              (document.getElementById('selectdf3').value=="jsutalo.png")||
              (document.getElementById('selectdf3').value=="bfranjic.png")){
              df3w1=3;
              df3w2=3
              df3w3=3;
              df3w4=1;
              df3w5=3;
              df3w6=3;
              df3w7=0;
              df3w8=3;
              df3w9=0;
              df3w10=3;
              df3w11=3;
              df3w12=3;
              df3w13=3;
              df3w14=3;
              df3w15=3;
              df3w16=1;
              df3w17=3;
              df3w18=3;
              df3w19=3;
            }
            else if((document.getElementById('selectdf3').value=="ssimic.png")||
              (document.getElementById('selectdf3').value=="aismajli.png")||
              (document.getElementById('selectdf3').value=="nmujakic.png")||
              (document.getElementById('selectdf3').value=="mvuskovic.png")||
              (document.getElementById('selectdf3').value=="svucur.png")||
              (document.getElementById('selectdf3').value=="sradic.png")||
              (document.getElementById('selectdf3').value=="ldellova.png")){
              df3w1=3;
              df3w2=3;
              df3w3=3;
              df3w4=0;
              df3w5=3;
              df3w6=0;
              df3w7=3;
              df3w8=1;
              df3w9=3;
              df3w10=1;
              df3w11=3;
              df3w12=1;
              df3w13=3;
              df3w14=0;
              df3w15=3;
              df3w16=1;
              df3w17=0;
              df3w18=1;
              df3w19=3;
            }
            else if((document.getElementById('selectdf3').value=="hsmolcic.png")||
              (document.getElementById('selectdf3').value=="ngalovic.png")||
              (document.getElementById('selectdf3').value=="jescoval.png")||
              (document.getElementById('selectdf3').value=="lsimic.png")||
              (document.getElementById('selectdf3').value=="dvelkovski.png")||
              (document.getElementById('selectdf3').value=="jcelikovic.png")||
              (document.getElementById('selectdf3').value=="lmikulica.png")){
              df3w1=3;
              df3w2=3;
              df3w3=3;
              df3w4=0;
              df3w5=1;
              df3w6=0;
              df3w7=1;
              df3w8=1;
              df3w9=3;
              df3w10=3;
              df3w11=1;
              df3w12=3;
              df3w13=0;
              df3w14=0;
              df3w15=0;
              df3w16=3;
              df3w17=3;
              df3w18=3;
              df3w19=3;
            }
            else if((document.getElementById('selectdf3').value=="mskoric.png")||
              (document.getElementById('selectdf3').value=="amajstorovic.png")||
              (document.getElementById('selectdf3').value=="bsutalo.png")||
              (document.getElementById('selectdf3').value=="guti.png")||
              (document.getElementById('selectdf3').value=="dloncar.png")){
              df3w1=3;
              df3w2=0;
              df3w3=3;
              df3w4=1;
              df3w5=1;
              df3w6=3;
              df3w7=1;
              df3w8=1;
              df3w9=0;
              df3w10=3;
              df3w11=3;
              df3w12=1;
              df3w13=0;
              df3w14=3;
              df3w15=0;
              df3w16=3;
              df3w17=1;
              df3w18=3;
              df3w19=3;
            }
            else if((document.getElementById('selectdf3').value=="ajovicic.png")||
              (document.getElementById('selectdf3').value=="kkrizmanic.png")||
              (document.getElementById('selectdf3').value=="msteenvoorden.png")||
              (document.getElementById('selectdf3').value=="mjcelic.png")){
              df3w1=1;
              df3w2=3;
              df3w3=0;
              df3w4=3;
              df3w5=0;
              df3w6=1;
              df3w7=3;
              df3w8=1;
              df3w9=0;
              df3w10=3;
              df3w11=0;
              df3w12=0;
              df3w13=3;
              df3w14=3;
              df3w15=1;
              df3w16=3;
              df3w17=0;
              df3w18=3;
              df3w19=1;
            }
            else if((document.getElementById('selectdf3').value=="dkolinger.png")||
              (document.getElementById('selectdf3').value=="jmersinaj.png")||
              (document.getElementById('selectdf3').value=="mleskovic.png")||
              (document.getElementById('selectdf3').value=="dkovacic.png")||
              (document.getElementById('selectdf3').value=="djokovic.png")||
              (document.getElementById('selectdf3').value=="msuto.png")||
              (document.getElementById('selectdf3').value=="npejovic.png")||
              (document.getElementById('selectdf3').value=="ilovric.png")||
              (document.getElementById('selectdf3').value=="lsmoljo.png")||
              (document.getElementById('selectdf3').value=="ffilipovic.png")||
              (document.getElementById('selectdf3').value=="franklin.png")){
              df3w1=0;
              df3w2=0;
              df3w3=0;
              df3w4=3;
              df3w5=1;
              df3w6=3;
              df3w7=3;
              df3w8=1;
              df3w9=3;
              df3w10=0;
              df3w11=1;
              df3w12=1;
              df3w13=3;
              df3w14=3;
              df3w15=3;
              df3w16=0;
              df3w17=3;
              df3w18=0;
              df3w19=0;
            }
            else if((document.getElementById('selectdf3').value=="bmikulic.png")||
              (document.getElementById('selectdf3').value=="vmedimorec.png")||
              (document.getElementById('selectdf3').value=="mzirdum.png")||
              (document.getElementById('selectdf3').value=="tbozic.png")||
              (document.getElementById('selectdf3').value=="fhlevnjak.png")){
              df3w1=0;
              df3w2=0;
              df3w3=0;
              df3w4=3;
              df3w5=3;
              df3w6=1;
              df3w7=0;
              df3w8=0;
              df3w9=3;
              df3w10=0;
              df3w11=0;
              df3w12=0;
              df3w13=0;
              df3w14=1;
              df3w15=1;
              df3w16=3;
              df3w17=3;
              df3w18=0;
              df3w19=0;
            }
            else if((document.getElementById('selectdf3').value=="nsoldo.png")||
              (document.getElementById('selectdf3').value=="dvanbruggen.png")||
              (document.getElementById('selectdf3').value=="dgrgic.png")||
              (document.getElementById('selectdf3').value=="msavic.png")||
              (document.getElementById('selectdf3').value=="itatomirovic.png")||
              (document.getElementById('selectdf3').value=="inekic.png")||
              (document.getElementById('selectdf3').value=="igrozdek.png")){
              df3w1=1;
              df3w2=0;
              df3w3=0;
              df3w4=1;
              df3w5=0;
              df3w6=0;
              df3w7=1;
              df3w8=3;
              df3w9=0;
              df3w10=0;
              df3w11=1;
              df3w12=1;
              df3w13=3;
              df3w14=0;
              df3w15=0;
              df3w16=0;
              df3w17=0;
              df3w18=1;
              df3w19=1;
            }
            else if((document.getElementById('selectdf3').value=="pbosancic.png")||
              (document.getElementById('selectdf3').value=="jtomasevic.png")||
              (document.getElementById('selectdf3').value=="arufati.png")||
              (document.getElementById('selectdf3').value=="rpaez.png")){
              df3w1=0;
              df3w2=3;
              df3w3=3;
              df3w4=0;
              df3w5=0;
              df3w6=1;
              df3w7=1;
              df3w8=0;
              df3w9=0;
              df3w10=1;
              df3w11=1;
              df3w12=0;
              df3w13=0;
              df3w14=1;
              df3w15=1;
              df3w16=0;
              df3w17=0;
              df3w18=0;
              df3w19=0;
            }
            else if((document.getElementById('selectdf3').value=="fprce.png")||
              (document.getElementById('selectdf3').value=="mstolnik.png")||
              (document.getElementById('selectdf3').value=="msenic.png")||
              (document.getElementById('selectdf3').value=="inovoselec.png")){
              df3w1=0;
              df3w2=0;
              df3w3=0;
              df3w4=1;
              df3w5=1;
              df3w6=1;
              df3w7=0;
              df3w8=1;
              df3w9=3;
              df3w10=0;
              df3w11=0;
              df3w12=3;
              df3w13=0;
              df3w14=0;
              df3w15=1;
              df3w16=0;
              df3w17=1;
              df3w18=0;
              df3w19=0;
            }
          },
          bodovidf4(){
            if((document.getElementById('selectdf4').value=="pstojanovic.png")||
              (document.getElementById('selectdf4').value=="smoharrami.png")||
              (document.getElementById('selectdf4').value=="thrvoj.png")){
              df4w1=3;
              df4w2=3;
              df4w3=3;
              df4w4=1;
              df4w5=3;
              df4w6=3;
              df4w7=0;
              df4w8=3;
              df4w9=0;
              df4w10=3;
              df4w11=3;
              df4w12=3;
              df4w13=3;
              df4w14=3;
              df4w15=3;
              df4w16=1;
              df4w17=3;
              df4w18=3;
              df4w19=3;
            }
            else if((document.getElementById('selectdf4').value=="jjuranovic.png")||
              (document.getElementById('selectdf4').value=="jbasic.png")){
              df4w1=3;
              df4w2=3;
              df4w3=3;
              df4w4=0;
              df4w5=3;
              df4w6=0;
              df4w7=3;
              df4w8=1;
              df4w9=3;
              df4w10=1;
              df4w11=3;
              df4w12=1;
              df4w13=3;
              df4w14=0;
              df4w15=3;
              df4w16=1;
              df4w17=0;
              df4w18=1;
              df4w19=3;
            }
            else if((document.getElementById('selectdf4').value=="itomecak.png")||
              (document.getElementById('selectdf4').value=="mraspopovic.png")||
              (document.getElementById('selectdf4').value=="mpavelic.png")){
              df4w1=3;
              df4w2=3;
              df4w3=3;
              df4w4=0;
              df4w5=1;
              df4w6=0;
              df4w7=1;
              df4w8=1;
              df4w9=3;
              df4w10=3;
              df4w11=1;
              df4w12=3;
              df4w13=0;
              df4w14=0;
              df4w15=0;
              df4w16=3;
              df4w17=3;
              df4w18=3;
              df4w19=3;
            }
            else if((document.getElementById('selectdf4').value=="isilva.png")||
              (document.getElementById('selectdf4').value=="agrgic.png")||
              (document.getElementById('selectdf4').value=="tsorsa.png")||
              (document.getElementById('selectdf4').value=="ttodoroski.png")){
              df4w1=3;
              df4w2=0;
              df4w3=3;
              df4w4=1;
              df4w5=1;
              df4w6=3;
              df4w7=1;
              df4w8=1;
              df4w9=0;
              df4w10=3;
              df4w11=3;
              df4w12=1;
              df4w13=0;
              df4w14=3;
              df4w15=0;
              df4w16=3;
              df4w17=1;
              df4w18=3;
              df4w19=3;
            }
            else if((document.getElementById('selectdf4').value=="mmuhammed.png")||
              (document.getElementById('selectdf4').value=="pperisa.png")){
              df4w1=1;
              df4w2=3;
              df4w3=0;
              df4w4=3;
              df4w5=0;
              df4w6=1;
              df4w7=3;
              df4w8=1;
              df4w9=0;
              df4w10=3;
              df4w11=0;
              df4w12=0;
              df4w13=3;
              df4w14=3;
              df4w15=1;
              df4w16=3;
              df4w17=0;
              df4w18=3;
              df4w19=1;
            }
            else if((document.getElementById('selectdf4').value=="fkaracic.png")||
              (document.getElementById('selectdf4').value=="pgluhakovic.png")||
              (document.getElementById('selectdf4').value=="mjuric.png")){
              df4w1=0;
              df4w2=0;
              df4w3=0;
              df4w4=3;
              df4w5=1;
              df4w6=3;
              df4w7=3;
              df4w8=1;
              df4w9=3;
              df4w10=0;
              df4w11=1;
              df4w12=1;
              df4w13=3;
              df4w14=3;
              df4w15=3;
              df4w16=0;
              df4w17=3;
              df4w18=0;
              df4w19=0;
            }
            else if((document.getElementById('selectdf4').value=="mkaramarko.png")||
              (document.getElementById('selectdf4').value=="miharos.png")){
              df4w1=0;
              df4w2=0;
              df4w3=0;
              df4w4=3;
              df4w5=3;
              df4w6=1;
              df4w7=0;
              df4w8=0;
              df4w9=3;
              df4w10=0;
              df4w11=0;
              df4w12=0;
              df4w13=0;
              df4w14=1;
              df4w15=1;
              df4w16=3;
              df4w17=3;
              df4w18=0;
              df4w19=0;
            }
            else if((document.getElementById('selectdf4').value=="mrom.png")||
              (document.getElementById('selectdf4').value=="abosec.png")||
              (document.getElementById('selectdf4').value=="gbaric.png")){
              df4w1=1;
              df4w2=0;
              df4w3=0;
              df4w4=1;
              df4w5=0;
              df4w6=0;
              df4w7=1;
              df4w8=3;
              df4w9=0;
              df4w10=0;
              df4w11=1;
              df4w12=1;
              df4w13=3;
              df4w14=0;
              df4w15=0;
              df4w16=0;
              df4w17=0;
              df4w18=1;
              df4w19=1;
            }
            else if((document.getElementById('selectdf4').value=="mgrujevic.png")||
              (document.getElementById('selectdf4').value=="mfranic.png")){
              df4w1=0;
              df4w2=3;
              df4w3=3;
              df4w4=0;
              df4w5=0;
              df4w6=1;
              df4w7=1;
              df4w8=0;
              df4w9=0;
              df4w10=1;
              df4w11=1;
              df4w12=0;
              df4w13=0;
              df4w14=1;
              df4w15=1;
              df4w16=0;
              df4w17=0;
              df4w18=0;
              df4w19=0;
            }
            else if((document.getElementById('selectdf4').value=="ntkalcic.png")||
              (document.getElementById('selectdf4').value=="dperkovic.png")||
              (document.getElementById('selectdf4').value=="ftomaskovic.png")){
              df4w1=0;
              df4w2=0;
              df4w3=0;
              df4w4=1;
              df4w5=1;
              df4w6=1;
              df4w7=0;
              df4w8=1;
              df4w9=3;
              df4w10=0;
              df4w11=0;
              df4w12=3;
              df4w13=0;
              df4w14=0;
              df4w15=1;
              df4w16=0;
              df4w17=1;
              df4w18=0;
              df4w19=0;
            }
          },
          bodovigk1(){
            if((document.getElementById('selectgk1').value=="dlivakovic.png")||
            (document.getElementById('selectgk1').value=="dzagorac.png")){
              gk1w1=3;
              gk1w2=3;
              gk1w3=3;
              gk1w4=1;
              gk1w5=3;
              gk1w6=3;
              gk1w7=0;
              gk1w8=3;
              gk1w9=0;
              gk1w10=3;
              gk1w11=3;
              gk1w12=3;
              gk1w13=3;
              gk1w14=3;
              gk1w15=3;
              gk1w16=1;
              gk1w17=3;
              gk1w18=3;
              gk1w19=3;
            }
            else if((document.getElementById('selectgk1').value=="jposavec.png")||
              (document.getElementById('selectgk1').value=="mljubic.png")||
              (document.getElementById('selectgk1').value=="gblazevic.png")){
              gk1w1=3;
              gk1w2=3;
              gk1w3=3;
              gk1w4=0;
              gk1w5=3;
              gk1w6=0;
              gk1w7=3;
              gk1w8=1;
              gk1w9=3;
              gk1w10=1;
              gk1w11=3;
              gk1w12=1;
              gk1w13=3;
              gk1w14=0;
              gk1w15=3;
              gk1w16=1;
              gk1w17=0;
              gk1w18=1;
              gk1w19=3;
            }
            else if((document.getElementById('selectgk1').value=="iprskalo.png")||
              (document.getElementById('selectgk1').value=="ipandur.png")||
              (document.getElementById('selectgk1').value=="dnwolokor.png")){
              gk1w1=3;
              gk1w2=3;
              gk1w3=3;
              gk1w4=0;
              gk1w5=1;
              gk1w6=0;
              gk1w7=1;
              gk1w8=1;
              gk1w9=3;
              gk1w10=3;
              gk1w11=1;
              gk1w12=3;
              gk1w13=0;
              gk1w14=0;
              gk1w15=0;
              gk1w16=3;
              gk1w17=3;
              gk1w18=3;
              gk1w19=3;
            }
            else if((document.getElementById('selectgk1').value=="iivusic.png")||
              (document.getElementById('selectgk1').value=="mmalenica.png")){
              gk1w1=3;
              gk1w2=0;
              gk1w3=3;
              gk1w4=1;
              gk1w5=1;
              gk1w6=3;
              gk1w7=1;
              gk1w8=1;
              gk1w9=0;
              gk1w10=3;
              gk1w11=3;
              gk1w12=1;
              gk1w13=0;
              gk1w14=3;
              gk1w15=0;
              gk1w16=3;
              gk1w17=1;
              gk1w18=3;
              gk1w19=3;
            }
            else if((document.getElementById('selectgk1').value=="kkahlina.png")||
              (document.getElementById('selectgk1').value=="icovic.png")||
              (document.getElementById('selectgk1').value=="lisek.png")){
              gk1w1=1;
              gk1w2=3;
              gk1w3=0;
              gk1w4=3;
              gk1w5=0;
              gk1w6=1;
              gk1w7=3;
              gk1w8=1;
              gk1w9=0;
              gk1w10=3;
              gk1w11=0;
              gk1w12=0;
              gk1w13=3;
              gk1w14=3;
              gk1w15=1;
              gk1w16=3;
              gk1w17=0;
              gk1w18=3;
              gk1w19=1;
            }
            else if((document.getElementById('selectgk1').value=="igrbic.png")||
              (document.getElementById('selectgk1').value=="khendija.png")||
              (document.getElementById('selectgk1').value=="mkramer.png")){
              gk1w1=0;
              gk1w2=0;
              gk1w3=0;
              gk1w4=3;
              gk1w5=1;
              gk1w6=3;
              gk1w7=3;
              gk1w8=1;
              gk1w9=3;
              gk1w10=0;
              gk1w11=1;
              gk1w12=1;
              gk1w13=3;
              gk1w14=3;
              gk1w15=3;
              gk1w16=0;
              gk1w17=3;
              gk1w18=0;
              gk1w19=0;
            }
            else if((document.getElementById('selectgk1').value=="ifilipovic.png")||
              (document.getElementById('selectgk1').value=="ajezina.png")||
              (document.getElementById('selectgk1').value=="dsugic.png")){
              gk1w1=0;
              gk1w2=0;
              gk1w3=0;
              gk1w4=3;
              gk1w5=3;
              gk1w6=1;
              gk1w7=0;
              gk1w8=0;
              gk1w9=3;
              gk1w10=0;
              gk1w11=0;
              gk1w12=0;
              gk1w13=0;
              gk1w14=1;
              gk1w15=1;
              gk1w16=3;
              gk1w17=3;
              gk1w18=0;
              gk1w19=0;
            }
            else if((document.getElementById('selectgk1').value=="ohadzikic.png")||
              (document.getElementById('selectgk1').value=="zfrelih.png")||
              (document.getElementById('selectgk1').value=="mmatkovic.png")||
              (document.getElementById('selectgk1').value=="ikelava.png")||
              (document.getElementById('selectgk1').value=="cberkovic.png")){
              gk1w1=1;
              gk1w2=0;
              gk1w3=0;
              gk1w4=1;
              gk1w5=0;
              gk1w6=0;
              gk1w7=1;
              gk1w8=3;
              gk1w9=0;
              gk1w10=0;
              gk1w11=1;
              gk1w12=1;
              gk1w13=3;
              gk1w14=0;
              gk1w15=0;
              gk1w16=0;
              gk1w17=0;
              gk1w18=1;
              gk1w19=1;
            }
            else if((document.getElementById('selectgk1').value=="jcondric.png")||
              (document.getElementById('selectgk1').value=="tduka.png")||
              (document.getElementById('selectgk1').value=="lmajkic.png")){
              gk1w1=0;
              gk1w2=3;
              gk1w3=3;
              gk1w4=0;
              gk1w5=0;
              gk1w6=1;
              gk1w7=1;
              gk1w8=0;
              gk1w9=0;
              gk1w10=1;
              gk1w11=1;
              gk1w12=0;
              gk1w13=0;
              gk1w14=1;
              gk1w15=1;
              gk1w16=0;
              gk1w17=0;
              gk1w18=0;
              gk1w19=0;
            }
            else if((document.getElementById('selectgk1').value=="inevistic.png")||
              (document.getElementById('selectgk1').value=="amrmic.png")){
              gk1w1=0;
              gk1w2=0;
              gk1w3=0;
              gk1w4=1;
              gk1w5=1;
              gk1w6=1;
              gk1w7=0;
              gk1w8=1;
              gk1w9=3;
              gk1w10=0;
              gk1w11=0;
              gk1w12=3;
              gk1w13=0;
              gk1w14=0;
              gk1w15=1;
              gk1w16=0;
              gk1w17=1;
              gk1w18=0;
              gk1w19=0;
            }
          },
          bodoviw1(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)>=0)&&(((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)<=1)){
              porazi++;
            }
            else if((((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)>1)&&(((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)>2)&&(((fw1w1+fw2w1+fw3w1+mf1w1+mf2w1+mf3w1+df1w1+df2w1+df3w1+df4w1+gk1w1)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw2(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)>=0)&&(((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)<=1)){
              porazi++;
            }
            else if((((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)>1)&&(((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)>2)&&(((fw1w2+fw2w2+fw3w2+mf1w2+mf2w2+mf3w2+df1w2+df2w2+df3w2+df4w2+gk1w2)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw3(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)>=0)&&(((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)<=1)){
              porazi++;
            }
            else if((((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)>1)&&(((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)>2)&&(((fw1w3+fw2w3+fw3w3+mf1w3+mf2w3+mf3w3+df1w3+df2w3+df3w3+df4w3+gk1w3)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw4(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)>=0)&&(((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)<=1)){
              porazi++;
            }
            else if((((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)>1)&&(((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)>2)&&(((fw1w4+fw2w4+fw3w4+mf1w4+mf2w4+mf3w4+df1w4+df2w4+df3w4+df4w4+gk1w4)/11)<=3)){
              pobjede++;
            }            
          },
          bodoviw5(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)>=0)&&(((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)<=1)){
              porazi++;
            }
            else if((((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)>1)&&(((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)>2)&&(((fw1w5+fw2w5+fw3w5+mf1w5+mf2w5+mf3w5+df1w5+df2w5+df3w5+df4w5+gk1w5)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw6(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)>=0)&&(((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)<=1)){
              porazi++;
            }
            else if((((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)>1)&&(((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)>2)&&(((fw1w6+fw2w6+fw3w6+mf1w6+mf2w6+mf3w6+df1w6+df2w6+df3w6+df4w6+gk1w6)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw7(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)>=0)&&(((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)<=1)){
              porazi++;
            }
            else if((((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)>1)&&(((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)>2)&&(((fw1w7+fw2w7+fw3w7+mf1w7+mf2w7+mf3w7+df1w7+df2w7+df3w7+df4w7+gk1w7)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw8(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)>=0)&&(((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)<=1)){
              porazi++;
            }
            else if((((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)>1)&&(((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)>2)&&(((fw1w8+fw2w8+fw3w8+mf1w8+mf2w8+mf3w8+df1w8+df2w8+df3w8+df4w8+gk1w8)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw9(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)>=0)&&(((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)<=1)){
              porazi++;
            }
            else if((((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)>1)&&(((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)>2)&&(((fw1w9+fw2w9+fw3w9+mf1w9+mf2w9+mf3w9+df1w9+df2w9+df3w9+df4w9+gk1w9)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw10(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)>=0)&&(((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)<=1)){
              porazi++;
            }
            else if((((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)>1)&&(((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)>2)&&(((fw1w10+fw2w10+fw3w10+mf1w10+mf2w10+mf3w10+df1w10+df2w10+df3w10+df4w10+gk1w10)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw11(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)>=0)&&(((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)<=1)){
              porazi++;
            }
            else if((((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)>1)&&(((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)>2)&&(((fw1w11+fw2w11+fw3w11+mf1w11+mf2w11+mf3w11+df1w11+df2w11+df3w11+df4w11+gk1w11)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw12(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)>=0)&&(((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)<=1)){
              porazi++;
            }
            else if((((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)>1)&&(((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)>2)&&(((fw1w12+fw2w12+fw3w12+mf1w12+mf2w12+mf3w12+df1w12+df2w12+df3w12+df4w12+gk1w12)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw13(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)>=0)&&(((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)<=1)){
              porazi++;
            }
            else if((((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)>1)&&(((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)>2)&&(((fw1w13+fw2w13+fw3w13+mf1w13+mf2w13+mf3w13+df1w13+df2w13+df3w13+df4w13+gk1w13)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw14(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)>=0)&&(((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)<=1)){
              porazi++;
            }
            else if((((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)>1)&&(((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)>2)&&(((fw1w14+fw2w14+fw3w14+mf1w14+mf2w14+mf3w14+df1w14+df2w14+df3w14+df4w14+gk1w14)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw15(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)>=0)&&(((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)<=1)){
              porazi++;
            }
            else if((((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)>1)&&(((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)>2)&&(((fw1w15+fw2w15+fw3w15+mf1w15+mf2w15+mf3w15+df1w15+df2w15+df3w15+df4w15+gk1w15)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw16(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)>=0)&&(((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)<=1)){
              porazi++;
            }
            else if((((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)>1)&&(((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)>2)&&(((fw1w16+fw2w16+fw3w16+mf1w16+mf2w16+mf3w16+df1w16+df2w16+df3w16+df4w16+gk1w16)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw17(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)>=0)&&(((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)<=1)){
              porazi++;
            }
            else if((((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)>1)&&(((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)>2)&&(((fw1w17+fw2w17+fw3w17+mf1w17+mf2w17+mf3w17+df1w17+df2w17+df3w17+df4w17+gk1w17)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw18(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)>=0)&&(((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)<=1)){
              porazi++;
            }
            else if((((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)>1)&&(((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)>2)&&(((fw1w18+fw2w18+fw3w18+mf1w18+mf2w18+mf3w18+df1w18+df2w18+df3w18+df4w18+gk1w18)/11)<=3)){
              pobjede++;
            }
          },
          bodoviw19(){
            this.bodovifw1();
            this.bodovifw2();
            this.bodovifw3();
            this.bodovimf1();
            this.bodovimf2();
            this.bodovimf3();
            this.bodovidf1();
            this.bodovidf2();
            this.bodovidf3();
            this.bodovidf4();
            this.bodovigk1();
            if((((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)>=0)&&(((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)<=1)){
              porazi++;
            }
            else if((((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)>1)&&(((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)<=2)){
              nerijesene++;
            }
            else if((((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)>2)&&(((fw1w19+fw2w19+fw3w19+mf1w19+mf2w19+mf3w19+df1w19+df2w19+df3w19+df4w19+gk1w19)/11)<=3)){
              pobjede++;
            }
          },
          odigranisusreti(){
            this.bodoviw1();
            this.bodoviw2();
            this.bodoviw3();
            this.bodoviw4();
            this.bodoviw5();
            this.bodoviw6();
            this.bodoviw7();
            this.bodoviw8();
            this.bodoviw9();
            this.bodoviw10();
            this.bodoviw11();
            this.bodoviw12();
            this.bodoviw13();
            this.bodoviw14();
            this.bodoviw15();
            this.bodoviw16();
            this.bodoviw17();
            this.bodoviw18();
            this.bodoviw19();
            odigrani=porazi+nerijesene+pobjede;
          },
          ukupnibodovi(){
            bodovi=0;
            odigrani=0;
            porazi=0;
            nerijesene=0;
            pobjede=0;
            this.odigranisusreti();
            bodovi=3*pobjede+nerijesene;
          },
          savestats(){
            this.ukupnibodovi();
            let id = this.userEmail;
            db.collection("bodovi").doc(id).set({
                                        wins: pobjede,
                                        draws: nerijesene,
                                        losses: porazi,
                                        played: odigrani,
                                        points: bodovi
            })
          },
          loadstats(){
            let id = this.userEmail;
            db.collection("bodovi").doc(id).get().then(doc =>{
              if(doc.exists){
                this.wins=doc.data().wins;
                this.draws=doc.data().draws;
                this.losses=doc.data().losses;
                this.played=doc.data().played;
                this.points=doc.data().points;
              }
            });
          },
          refresh(){
            setTimeout(() => window.location.reload(), 500);
          },
          savedb(){
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
                                        gk: document.getElementById('selectgk1').value, 
            })
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
        this.loadstats();
      },
      mounted(){
        this.loaddb();
        this.loadstats();
      }
    }
</script>
