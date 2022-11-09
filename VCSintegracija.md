# VCS Integracija

> :warning: **POZOR:** Email GitHub računa mora biti enak emailu uporabnika (ne administratorja) na YouTrack! V nasprotnem primeru premikanje opravil po scrum tabli z uporabo commit sporočil ne bo delovalo.

<br>

## Povezava z GitHub

Kliknite na gumb ***Nastavitve (desni zgornji kot) -> Integrations -> VSC Integrations -> New VCS Integration***:

- **Main project**: izberite vaš projekt
- **Server type**: GitHub
- **Repository url**: prilepite link do repozitorija
- **Personal access token**: klik na gumb **Generate token** in sledite navodilom na GitHub-u.  
  > :memo: **Note:**
  > - Pod **note** napišite, da je to token za YouTrack (za kasnejšo evidenco)
  > - Expiration: Vsaj 90 dni
  > - Pod *Select scopes* naj bo obkljukan **repo** in **admin:repo_hook**
  > - Klik na **Generate Token** in prekopirajte vrednost v polje v YouTrack
  > - Klik na **Save**

<br>

## Spreminjanje stanja opravil s commit sporočili

Taske ročno prestavljajte iz **Sprint backlog -> TODO -> DOING**.  

Premik iz **DOING -> DONE**, skupaj s podatkom o porabljenem času, mora biti opravljen preko commit sporočila.

Primer:  
```
git commit -m "inicializiral repozitorij #R2022-6 DONE Time 4h"
```

- **Commit sporočilo avtorja**: inicializiral repozitorij
- **Referenca opravila na YouTrack**: #R2022-6
- **Željeno stanje**: DONE *(vrednost se mora ujemati z vrednostimi nastavljenimi v projektu)*
- **Porabljen čas**: Time 4h

Po ukazu ```git push``` se bo task prestavil na stolpec **DONE**, opravilu pa se bo vpisal tudi porabljen čas.
