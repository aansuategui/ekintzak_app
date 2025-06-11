# 📋 EKE-en antolatzailea

Web-aplikazio honek Maiztegiko ikasleen **eskola kanpoko ekintzak** antolatzeko prozesua automatizatzen laguntzen du.

---

## 🎯 Helburua

Familiek erantzundako Google Form-aren emaitzetatik abiatuta, aplikazio honek **ekintza bakoitzeko ikasle-zerrendak** sortzen ditu, **ikasturtearen arabera** antolatuta. Emaitza zuzenean ikus daiteke eta **Word fitxategi batean deskargatu** daiteke.

---

## 🛠️ Nola erabili

1. Google Form-a bete ondoren, joan zaitez **Google Forms**-eko **"Erantzunak"** atalean.
2. Bertan, **Excel fitxategi gisa deskargatu** formularioaren emaitzak eta gorde zure ordenagailuan.
3. **Excel fitxategia ireki eta "CSV UTF-8 (Comma delimited) (*.csv)" formatuan gorde**.
4. Sartu webgunera: 👉 [https://eke-maiztegi.streamlit.app/](https://eke-maiztegi.streamlit.app/)
5. Kargatu `.csv` fitxategia **"Igo formularioaren CSV fitxategia"** botoiarekin.
6. Ikasle-zerrendak pantailan agertuko dira, **ekintzen eta ikasturtearen arabera** antolatuta.
7. Behean botoi bat agertuko da: **"⬇️ Deskargatu DOCX fitxategia"**. Horri esker, zerrenda deskargatu daiteke Word dokumentu gisa.

---

## 📄 Onartutako CSV fitxategiaren formatua

Aplikazioa **Google Forms** bidez jasotako emaitza-fitxategietarako pentsatuta dago, eta honako egitura izan behar du:

| Zutabea | Deskribapena |
|--------|--------------|
| `UMEAREN IZEN ABIZENAK / Nombre y apellidos del alumno` | Ikaslearen izen-abizenak (automatikoki normalizatzen dira) |
| `2025/26 IKASTURTEKO IKAS-MAILA` | Ikaslearen maila (`HH3`, `HH4`, `LH2`, etab.) |
| `Aukeratu nahi dituzun ekintzak` (eta `.1`, `.2`, `.3`) | Aukeratutako ekintzak, zutabe ezberdinetan banatuta |
| Beste zutabe batzuk | (posta elektronikoa, telefonoa, oharrak...) ez dira kontuan hartzen zerrenda sortzerakoan |

> **Oharra**: ikasleek hainbat ekintza hautatzen badituzte zutabe batean, `,` bidez banatuta agertuko dira.

