# Vaja1-ADC-single-conversion-STM32F0-Buzina-Kuder-Nograsek

2.	Postopek inicializacije periferije.
a)	Zaženite STM32CubeIDE in ustvarite nov STM32 projekt (pod zavihkom information Center). V zavihku Board selector s pomočjo filtrov Vendor, Type in MCU/MPU Series Izberite ustrezno razvojno ploščo (v našem priemru STM32F0Discovery), kliknite Next, projekt poimenujte vaja1_ADC_pretvorba in kliknite  Finish (na možnosti opcije za prenastavitev periferije izberite Yes, izbrana naj bo tudi opcija perspektive za STM32CubeMX).
b)	V Pinout pogledu si oglejte prerazporeditev PIN-ov mikroprocesorja za vhodne in izhodne enote. Zelena LED je priključena na _PC9___ pin, MODRA pa na __PC8___ pin. Kaj je pa priključeno na pin PA0? ________modra tipka____________________.
c)	Glede na vašo razvojno ploščico in razširitveno vezje z tipkami ter potenciometri, izberite ustrezni analogni vhod. Kateri pin je to? __PC0____ . Poglejte vezavo na ploščici!
d)	V Analog razdelku levo od sheme mikroprocesorja ugotovite, koliko ADC pretvornikov ima vaša razvojna ploščica? _______19_______
e)	 Izbrani ADC pretvornik ima oznako s trikotnikom. Kaj to pomeni? __To pomeni da je nek pin bil zaseden
Kaj morate storiti, da razrešite to omejitev? Opišite in jo odpravite.
Odpraviti moramo pin ki je zaseden v našem primeru je to PA0 
__________________________________________________________
Pin moramo nastaviti tako da bo prost in prestaviti na drug pin tako bomo izbrisali klicaj in sprostili pin.
__________________________________________________________
__________________________________________________________
__________________________________________________________
f)	Razširite (kliknite) razdelek ADC. Koliko je vseh vhodnih kanalov (seštejte oznake INxx) ?
__16____________
g)	Glede na potenciometer na vaši ploščici izberite-obkljukajte ustrezni kanal/pin (Single-ended način!) Na zaslonu se vam mora usterzno pobarvati izbrani pin v zeleno barvo. Kaj se izpiše poleg pina? __ADC1_IN3___
h)	V kolikor še niso, aktivirajte obe LED diodi na ustreznih (dig.) izhodih/pinih, zeleno in modro (glej vaja0a).
i)	Pod Configuration  ADC enote gumb v Parameter settings izberite ločljivost pretvorbe na 8-bitno, torej je območje vrednosti od 0 ÷ 255. Preglejte, kakšne so še ostale možne ločljivosti pretvorbe in območja vrednosti?
a)	10bit, od 0 do 1023,
b)	12bit, od 0 do 4095,
c)	14bit, od 0 do 16383.
