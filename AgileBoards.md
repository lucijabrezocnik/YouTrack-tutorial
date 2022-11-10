# Agile boards

Za potrebe vodenja razvoja boste pripravili dve tabli:
- [Project Management Board](#Project-Management-Board) in
- [Project Development Board](#Project-Development-Board).

<br>

## Project Management Board

### Backlog

Nastavite backlog tako, da bo prikazoval vsa nedodeljena opravila. To storite tako, da odprete *Backlog* (klik na gumb Backlog na levi strani nad Scrum tablo) in kliknite na gumb z ikono svinčnika. Poskrbite da je v polju *Query* vpisano naslednje:  

```
project: <ime projekta> has: -{Board <ime projekta> project Management} #Unresolved #{User Story}  
```

### Scrum tabla

Če na Scrum tabli ne vidite vseh stolpcev (TODO, DOING, DONE), kliknite gumb ***Board settings -> Columns and Swimlanes -> Add column*** in izberite ustrezne vrednosti. Poskrbite, da stolpce določa polje *State* (to je tudi privzeta nastavitev).

<br>

## Project Development Board

Backlog in Scrum tablo nastavite podobno kot pri [Project Management Board](#Project-Management-Board), le da tukaj v *Query-u* za Backlog ***#{User story}*** spremenite v ***#Task*** ter ***Management*** v ***Development***.

Končni Query mora izgledati tako:  

```
project: <ime projekta> has: -{Board <ime projekta> Project Development} #Unresolved #Task
```
