# Dag 10 · GitHub och publicering

*Modul 4, UI/UX & Frontendutveckling, Lexicon IT-Proffs*

## Vad du ska göra idag

Du skickar upp ditt arbete med `git push` och publicerar sidan på riktigt med GitHub Pages. Du får en publik adress som alla kan öppna.

## Bakgrund

Hittills har dina commits bara funnits på din dator. Ett *remote* repo på GitHub är både en säkerhetskopia och ett sätt att dela. **GitHub Pages** gör att GitHub visar dina HTML-filer som en riktig webbplats på `https://ditt-namn.github.io/repo/`.

## Så arbetar du (samma som alltid)

1. **Forka** dagens repo på GitHub (*Fork → Create fork*).
2. **Klona din fork:** *Code → HTTPS → kopiera adressen*. I terminalen (Ctrl+ö i VS Code): `git clone <adressen>`. Öppna den nya mappen i VS Code och starta *Live Server*.
3. **Gör uppgiften.** Spara och kontrollera i webbläsaren efter varje steg. Gör en commit efter varje avslutat steg: `git add .` och `git commit -m "Beskriv vad du gjorde"`.
4. **Skicka upp** när du är klar: `git push`.
5. **Lämna in i Microsoft Forms.**

Fastnar du: skriv ner exakt var och vad du försökt, och ta det först i nästa handledda pass.

## Uppgiften steg för steg

### Steg 1. Kontrollera kopplingen

I terminalen: `git remote -v`. Du ska se `origin` med adressen till din fork på GitHub. Det kommer från att du klonade den.

### Steg 2. Kontrollera historiken på GitHub

Öppna din fork på GitHub och klicka *Commits*. Dina commits sedan dag 1 ska synas. Det är samma `git push` som du kört hela tiden. Första gången kan GitHub ha bett dig logga in, och det behövs normalt inte igen.

### Steg 3. Gör en commit och push i ett svep

Ändra något litet, kör `git add .`, `git commit -m "..."` och `git push`. Verifiera på GitHub. Du har nu den vanliga arbetsloopen: ändra, add, commit, push.

### Steg 4. Slå på GitHub Pages

På GitHub, i din fork: *Settings → Pages*. Under *Build and deployment*: Source = *Deploy from a branch*, Branch = `main`, mapp `/ (root)`. Spara. Vänta 1–2 minuter.

### Steg 5. Öppna din sida

Överst på Pages-inställningen visas adressen. Öppna den. Fungerar bilderna och CSS:en? Annars: kontrollera att sökvägarna är relativa (`css/base.css`, inte `/css/base.css`).

### Steg 6. Skriv README

Redigera `README.md`: rubrik, en mening om vad sajten är, länk till live-sidan, och vilka tekniker du använt. Commit, push.

### Steg 7. Gör samma sak med mitt-projekt

Publicera ditt eget projekt på samma sätt. Det är den länken du ska visa på redovisningen dag 12.

## AI-spåret (nivå 3: Styr och ansvara)

**AI skriver README, du verifierar** (cirka 25 minuter, efter att du gjort din egen lösning)

Fri användning, full loggning. Du bär ansvaret för allt du lämnar in. AI hittar gärna på funktioner som inte finns. En README som ljuger är värre än ingen README.

Regler: egen lösning först, du ska kunna förklara varje rad, och du loggar i `docs/ai-logg.md` i `mitt-projekt`. Reglerna finns i `AI-REGLER.md` i `mitt-projekt`.

1. Be AI skriva en README med prompten nedan.
2. Gå igenom varje påstående: finns det i koden?
3. Ta bort eller rätta det som är påhittat.
4. Kontrollera alla länkar och att live-länken fungerar.
5. Logga hur många påstånden som var fel.

Prompt att utgå från:

```
Skriv en README.md för detta repo.
Beskriv bara sådant som finns i filerna.
Markera med [KONTROLLERA] allt du är
osäker på.

[klistra in filstruktur och nyckelfiler]
```

**Kontrollera med:**

- Öppna varje länk.
- Jämför varje funktion som nämns mot koden.
- Läs hela texten högt. Låter det som dig?

**I ditt projekt:** Skriv READMEn för ditt projekt med AI och verifiera varje påstående.

## Kontrollista: så vet du att du är klar

- [ ] `git push` har skickat upp alla dina commits.
- [ ] Din fork har GitHub Pages påslaget, och live-länken fungerar.
- [ ] Bilder och CSS laddas på den publicerade sidan.
- [ ] README.md beskriver projektet och innehåller live-länken.
- [ ] Du har publicerat även `mitt-projekt`.
- [ ] Du har skickat in alla tre länkarna (repo, live-sida, mitt-projekt-live).
- [ ] Du har gjort AI-uppgiften och skrivit en post i `docs/ai-logg.md`.

## Tips om du fastnar

- 404 på sidan? Vänta några minuter och kontrollera att filen heter exakt `index.html` i rotmappen.
- Bilderna saknas? Sökvägar får inte börja med `/` och filnamn är känsliga för versaler.
- Repot måste vara publikt för att Pages ska fungera på ett gratiskonto.
- Push avvisas? Kör `git pull` först och försök igen.

## Ditt projekt: Dagens steg i `mitt-projekt`

Efter övningen här jobbar du vidare i ditt eget projekt (din design från modul 3). Dagens steg står i `PROJEKTSTEG.md` i ditt repo `mitt-projekt`, under **Dag 10**. Det är där ditt riktiga arbete växer. Övningen här är träningsbanan.

## Inlämning

**Deadline: imorgon klockan 09.00.** Allt lämnas in i Microsoft Forms. Du behöver inte redovisa något muntligt.

I formuläret fyller du i:

1. Länk till din fork av det här repot.
2. Länk till ditt `mitt-projekt`.
3. Reflektion: Klistra in live-länken. Vad var det första du tänkte när du öppnade din publicerade sida?

## Vill du mer? (frivilligt)

- Lägg till en `.gitignore`.
- Lägg till en skärmbild av sidan i README.md.
