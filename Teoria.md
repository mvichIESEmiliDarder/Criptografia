# Introducció

## Què és la criptografia?
El terme **criptografia** prové de dos vocables grecs: *criptos*,que significa ocult o amagat, i *grafos*, que signifca escriptura. Segons aquesta definició, doncs, la criptografia és l'especialitat que estudia l'escriptura oculta.

L'encriptament d'un missatge consisteix en, mitjançant tènciques i algoritmes que poden ser públics o privats i amb l'ajud de claus, amagar un missatge que només pugui coneixer el qui encripta el missatge i el qui el rep.

El desencriptament d'un missatge consisteix en dur a terme l'operació inversa, de forma que a partir d'un missatge encriptat, una clau i una algoritme o tènciques de desencriptat, podem obtenir el missatge original.

El text que forma el missatge original i que s'encripta amb un algorisme donat
s'anomena **text pla o text clar**, mentre que el missatge ja encriptat rep el
nom genèric de text xifrat o **criptograma**.

Per tant, un sistema criptogràfic es compon de:

| Concepte                   | Descripció                                                                                               |
| -------------------------- | -------------------------------------------------------------------------------------------------------- |
| Texte encriptat o missatge | Texte resultat d'aplicar un algoritme d'encriptació al missatge original                                 |
| Texte pla                  | Missatge original                                                                                        |
| Sistema criptogràfic       | Tènciques matemàtiques que empren algoritmes d'encriptació i encriptació                                 |
| Clau                       | Paraula o conjunt de caracteres alfanumèrics emprada tant per encriptar com per desencriptar el missatge |
| Emissor                    | Persona que encripta el texte pla o missatge no encriptat                                                |
| Receptor                   | Persona que rep i desencripta el texte encriptat o missatge                                              |
 
## Conseqüencies d'encriptar
El fet d'encriptar un missatge ens garanteix d'una serie de beneficis que són els motius bàsics de la criptografia:

- **Confidencialitat**: La informació només pot ser llegida per destinataris autoritzats
- **Integritat**: La informació no pot ser alterada en la seva transmissió
- **Autenticitat**: Ens garanteix que el missatge ve de l'emissor i no d'un tercer mal intencionat
- **No repudi**: L'emissor no pot negar l'autoria del missatge, ja que el destinatari en té proves del missatge

# Mètodes criptogràfics
Per a què el missatge sigui inintel·ligible per a qualsevol que no conegui l'algorisme d'encriptació, aquest s'encripta mitjançant un protocol o algorisme compartit per l'emissor i el receptor del missatge, així com la seva clau. D'aquesta manera, el receptor sempre podrà revertir el procés i fer que el missatge sigui comprensible.

A l'antiguetat, ja s'empraven mètodes criptogràfics que estudiem encara avui en dia. A la vida quotidiana, en afers d'estat, en guerres, en comerç i transaccions econòmiques, era molt útil i a voltes imperscindible,  emprar sistemes criptogràfics. Vegem-ne els més representatius:

## Xifrat Escítala
El sistema consistia en tenir dues vares del mateix gruix que s'entregaven als participants de la comunicació. Per enviar un missatge s'enrotllava una cinta de cuir de forma espiral a un dels bastons i s'escrivia el missatge longitudinalment, de manera que a cada volta de cinta aparegués una lletra de cada cop. Un cop escrit el missatge, es desenrotllava la cinta i s'enviava al receptor, que només l'havia d'enrotllar a la vara bessona per llegir el missatge original.

Podem trobar una descripció del procediment a l'obra de Plutarc, Vida de Lisandre. (font [wikipedia](https://es.wikipedia.org/wiki/Esc%C3%ADtala))

![[Skytale.png]]

## Xifratge Atbash
Històricament, fins i tot abans que els grecs utilitzessin la famosa Escítala, hi ha constància escrita d'un mètode de transposició a la Bíblia, el **xifrat Atbash**, un sistema en mirall que consisteix en substituir una lletra de l'alfabet hebreu per la seva espellada. Per exemple: es canvia la lletra *àlef* (la primera de l'alfabet) per la lletra de posició simètrica respecte al centre, en aquest cas l'última *tav*. El seu ús més conegut es dóna al llibre de Jeremies I on a fi de no nomenar l'odiada Babilònia (בבל, Babel) s'utilitza el terme, en atbash, Sesac (ששך, Sheshakh).

![[atbash.jpg]]
![[atbash1.jpg]]

Aquests dos mètodes de xifratge fan ús de la **transposició** de les lletres. En una **transposició** les lletres del text pla es barregen o desordenen seguint un determinat algorisme per obtenir un anagrama. 

## Xifrat César
El xifrat Cèsar, també conegut com a xifrat per desplaçament, codi de Cèsar o desplaçament de Cèsar. És una de les tècniques de xifrat més simples i més usades. És un tipus de xifrat per **substitució** en què una lletra al text original és reemplaçada per una altra lletra que es troba un nombre fix de posicions més endavant a l'alfabet. Per exemple, amb un desplaçament de 3, l'A seria substituïda per la D (situada 3 llocs a la dreta de l'A), la B seria reemplaçada per l'E, etc. Aquest mètode deu el seu nom a Juli Cèsar, que el feia servir per comunicar-se amb els seus generals. (font [wikipedia](https://es.wikipedia.org/wiki/Cifrado_C%C3%A9sar))

![[Caesar3.svg.png]]

## Xifrat Polibio
Un altre dels sistemes clàssics més coneguts és el **xifrat de Polybios** que data del segle II aC. i és el sistema per *substitució* de caràcters més antic que es coneix. En aquest cas se substitueix cada caràcter, cada lletra, per una parella de números o lletres. L'A passa a ser una AA, la B una AB, la C una AC… Aquests quadres podien canviar la combinació de lletres cada cop, provocant moltes variables”.

![[Polibio.png]]

Hem vist ara dos exemples xifrat per **substitució**. Aquest és un mètode de xifrat pel qual unitats de text pla són substituïts amb text xifrat seguint un sistema regular; les "unitats" poden ser una sola lletra (el cas més comú), parells de lletres, trios de lletres, barreges de l'anterior, entre d'altres. El receptor desxifra el text fent la substitució inversa. En una substitució, per contra, les unitats de text pla mantenen el seu ordre al missatge, però se substitueixen amb text xifrat seguint un algorisme específic.

Similars exemples de xifrat per substitució es poden considerar els sistemes alfabètics no convencionals (que poden actuar com a codis secrets per als profans que els desconeguin). Així tenim el Codi Morse, l'alfabet amb banderes, el Sistema Braille, els jeroglífics dels egípcis o l'alfabet dactilològic. 

També citarem noveles, on la trama discorre arran de desxifrar un codi secret, com, el llibre d'Edgar A. Poe, *L'escarabat d'or* (1843) o a la novela de Juli Verne, Viatge al centre de la terra  (1864) com a part dels esforços per desxifrar el missatge que dóna lloc al viatge,  o finalment la novela més moderna *Circo Máximo* de Santiago Posteguillo (2014), on en  el capítol 93 presenta un missatge xifrat per transposició columnar simple explicant-se, al llarg del mateix, el funcionament del desxifrat. El títol del capítol és aquest missatge xifrat (SIEAAZTEREUXMGSI).

![[goldbug.jpg]]
Imatge del llibre *l'Escarabat d'or*

![[Jules_verne_cryptogramme.png]]
Imatge del llibre *Viatge al centre de la terra*

I ens hem deixat molts d'exemples que a la història s'ha fet servir la criptografia,  els jeroglífics de fa 4000 anys a la ciutat Menet-Khufu que contaven la vida del seu senyor Khnumhoteb II; a la Índia al segle IV a.C el ministre Kautilya va escriure al seu rei Chandragupta la necessitat de desplegar espies per tot el pais i xifrar totes les seves comunicacions; Heródote, descriu a la seva obra *Històries* els conflictes entre Grècia i Persia al segle V a.C. i com va ser la criptografia la que va salvar a Grècia de ser ocupada per Jerjes, el rei dels Perses; els àrabs a l'any 750 ja empraven, entre els funcionaris, una forma rutinaria de criptografia per escriure manuals administratius (*Adab al-Kuttab*) o per per comunicar-se amb els seus governants; inclús els àrabs varen tractar també com rompre els sitemes criptogràfics, com l'erudit Abu Yusuf al-Kindi que al segle IX va escriure entre d'altres, el llibre *Sobre el desxiframent de missatges criptogràfics*.

![[erudit.jpg]]

En resum, sobre els mètodes criptogràfics podem dir que tenim dos tipus:
| Mètodes criptogràfics | Descripció                                                                                              |
| ------------------- | --------------------------------------------------------------------------------------------------------- |
| Transposició        | Les lletres del text pla es barregen o desordenen seguint un determinat algorisme per obtenir un anagrama |
| Substitució         | Les unitats de text pla són substituides amb text xifrat seguint un sistema regular                                                                                                          |

Finalment direm que *mentre que les tècniques de transposició barregen el text clar mitjançant un algoritme donat fins a obtenir un anagrama inintel·ligible, els mètodes de substitució mantenen l'ordre dels caràcters, però se substitueixen amb unitats de text xifrat*.


# Algoritmes criptogràfics
