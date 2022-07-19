# Medomet
Tento projekt vznikl jako výsledek vlastní potřeby motorizovat 4 rámkový medomet, protože točit celý den klikou znamená o 1 pracovní sílu na odvíčkování méně a také slušnou bolest ruky. Od počátku jsem přemýšlel jak pohon koncipovat a i když používat krokový motor může vzbuzovat pochybnosti, mám hodně důvodů proč jsme jej zvolil.

* Mám ke krokovým motorům blíže
* Žádný komutátor a uhlíky
* Levné díly
* Snadno opravitelné
* Snadno identifikovatelné místo závady
* Minimální potřeba výroby mechanických dílů
* Možnost elektronického otáčení koše po 90 stupních při výměně rámků
* Řízení rychlosti rozběhu i doběhu, potenciálně tvorba vytáčecích programů a to i pro zvratné medomety (reverzace chodu)

Samozřejmě jsou zde i nevýhody

* Hlučnější (kroky způsobují slyšitelné vibrace)
* Omezené otáčky (obykle přes 5 otáček za sekundu začne padat moment)

Pro řízení jsem použil Arduino UNO, protože jsem měl jedno invalidní s utrženým kondíkem i s kusem plošňáku a tedy nefunkčním zdrojem, takže v aplikaci kde se stejně musí vyrábět napájecí napájení pomocí Step-Down bylo snadno využitelné.  Ale asi není důvod nepoužít třeba Arduino NANO. OLED display jsem měl na SPI a opět využít jiný třeba obyčejný 2 řádkový a třeba i řízený přes I2C by také nebyl problém. Z prvotního testovacího vrabčího hnízda jsem to dotáhl na prototyp s tištěnými krabičkami, který umožnil schovat elekroniku, ale asi by to neměl být finální stav - je to takové rozbité, rozházené, chtělo by to celé uzavřt do jedné vzhledné krabice. Vími jak omezit hlučnost - motor mimo osu na silentbloky a zpřevodovat řemínkem 1:1. Bylo by to více mechanických dílů, ale medomet je zvukově hodně podobný bubnu, takže to hučení krokového motoru dost zesiluje a tohle by výrazně pmohlo. Na druhou stranu vytáčel jsem s tím celý den (jelo to prakticky permanentně) a ten zvuk se dal zvládnout. 
