
# YouTrack

<p align="center"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/8/8d/YouTrack_Icon.svg/1200px-YouTrack_Icon.svg.png" alt="drawing" width="200"/></p>


## Vzpostavitev projekta

**En** član skupine naj vzpostavi YouTrack projekt v **oblaku**. Brezplačno različico najdete na tej [povezavi](https://www.jetbrains.com/youtrack/buy/#cloud). Vpišite željeni **link** (najboljše da kar ime projekta brez presledkov) do vašega projekta in **email**.  

> :warning: **POZOR:** član skupine, ki ustvari strežnik, naj za to uporabi email, ki ga ne uporablja za GitHub, saj administratorja projekta, ni mogoče dodati na opravila kot udeleženca. Če na GitHub-u uporabljate @gmail račun, kreirajte YouTrack projet s študentskim emailom in obratno.

<br>

## Nastavitve projekta - ***Dodajanje uporabnikov***

Administrator projekt ustvari, nato pa s svojim **drugim emailom** kreira uporabnika s katerim dostopa do projekta v prihodnje in povabi drugega člana skupine.  

Kliknite na ikono v desnem zgornjem kotu ***Settings (Administration) -> Access management -> Users -> New User -> Invite users***, vpišite email in kliknite na ***Invite Users***

> :warning: **POZOR:** Email račun uporabnika na GitHub-u mora biti enak emailu uporabnika (uporabnika, ne administratorja, ki je ustvaril projekt) na YouTrack!

<br>


## Nastavitve projekta - ***Polja***

Kliknite ***Project -> <Ime vašega projekta> -> Fields (meni na desni strani)*** in uredite/dodajte naslednja polja:

- **State:** Vrednosti polja ***State -> Add Value*** in dodajte (vse obstoječe vrednosti odstranite):  

  - **TODO**
  - **DOING**
  - **DONE** (obkljukajte **Resolved** in nastavite zeleno barvo)


- **Dodatna polja:** Kliknite ***Add field to project***:  

  - **Simple description** -> Show only when: Type -> Is Set to: User Story
  - Due date -> Show only when: Type -> Is Set to: Task, Type: date and time  
  - Time -> Show only when: Type -> Is Set to: Task, Type: Period

  > :memo: **Note:** Asignee: polje že obstaja, morate pa ga nastaviti tako, da se pokaže le pri Task-ih. To storite enako kot pri poljih Due date in Time.
