# tyovuoroennuste analytiikka

Tarkoituksena on rakentaa ennustemalli saapuneista puheluista contact centeriin. 

Tavoitteena asiakaspalvelun resursoinnin optimointi. 

Haasteena:

Jos AsPassa on liian vähän resursseja, tulee jonoa ja asiakastyytymättömyyttä. Taustalla SLA-vaatimukset.

Jos AsPassa on liikaa väkeä, turhia henkilöstökuluja, ei ole hyödyllistä tekemistä.

AsPaan tulevien soittojen/palautteiden määrät vaihtelevat kausiluonteisesti.

Muut markkinointitekijät mm. erilaiset kampanjat ja muut tapahtumat lisäävät päivittäistä asiakaskontaktien määrää, mitä historiadata ei huomioi. Tämä on otettava ennusteessa huomioon.

Kysynnän aikasarjaennustaminen koneoppimismenetelmällä, ohjelmointikielenä Python

Ennustetaan asiakaspalveluun tulevien soittojen ja sähköpostiviestien päivittäiset/viikottaiset/kuukausittaiset määrät, voidaan asiakaspalvelu resursoida optimaalisemmin. 

Historiatieto saatavilla puhelujen ja viestien määristä riittävällä aikasyklillä. Laadullisilla asiakashaastatteluilla voidaan tietoa saada myös muista lähteistä, muun muassa markkinointitekijöistä ja suhdannevaihteluista.

Haasteena on, että historiadata tuottaa liian subjektiivisia arvioita. Historiatiedon lisäksi haastatteluja ennakoimattomista markkinointitekijöistä.

Aikasarjaennustaminen on aikaan sidottua säännönmukaisuutta.

Aikasarja voidaan jakaa komponentteihin, joita ovat trendi, kausivaihtelu, syklinen vaihtelu sekä satunnaisvaihtelu.

Mallinnuksessa keskeistä parametrien estimointi. 

Liukuva keskiarvo yksinkertaisin malli ennustaa kehitystä.

Liukuvan keskiarvon menetelmässä tulevan ajanhetken kysynnän ennuste on keskiarvo menneiden ajanhetkien kysynnästä.

Ratkaisuna: eksponentiaalinen tasoitus (liukuva keskiarvo painotettuna tuoreimpiin ajankohtiin) = > Ennuste reagoi herkästi muutoksiin ja helposti päivitettävissä.

Yksi suosituimmista kysynnän ennustamisen malleista.

Malliin voidaan lisätä komponentteja, jotka huomioivat trendin ja kausivaihtelun.

Kysyntään vaikuttavia tekijöitä ovat kysynnän perustason lisäksi trendi-, kausi-, sykli- ja markkinointitekijät sekä ennustamaton vaihtelu.

Mallia voi käyttää myös muiden contact center -datojen ennustamiseen.

Yksinkertainen, kaksinkertainen (Holtin malli) ja kolminkertainen (Holt-Winterin malli) eksponentiaalisen tasoituksen mallit. 

Eksponentiaalinen tasoitus löytyy statsmodels.tsa-kirjastosta.

Kolminkertainen malli huomioi sekä trendin että kausivaihtelun.
