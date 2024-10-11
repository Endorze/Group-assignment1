Skapa branch från MAIN.

Steg till att skapa branch från main och pusha upp på git.

Steg 1: git checkout main (om du redan är i en annan branch)

Steg 2: git checkout -b (branch namn, som till exempel "branch-aboutus-page")

Steg 3: git add .

Steg 4: git commit -m "Ditt beskrivande meddelande här"

Steg 5: git push origin "samma namn som nyskapade branch"

_______________________________________________________________________________

Steg till att merga när man är klar:

Steg 1: git add .

Steg 2: git commit -m "Beskrivning av vad du har gjort"

Steg 3: git checkout main

Steg 4: git pull (ETT MÅSTE DU FÅR INTE GLÖMMA DET KAN FUCKA UPP ALLT)
Notera att steg 6 och 7 inte behövs om steg 4 skriver ut "Already up to date" i konsolen.

Steg 5: git checkout - (Glöm ej minustecknet på slutet. Tar dig tillbaka till din branch, den du var i när du skrev steg 4)

Steg 6: git pull origin main

Steg 7: Fixa eventuella merge-konflikter, sedan git add . och git commit -m "Merge main"

Steg 8: git push

______________________________________________________________________________

Vad ska göras på sidorna?

index.html [

Header
Hero
Grid-layout med bild och text.
Footer

]

Aboutus.html [

Header
Grid-layout
Contact us
Footer

]

Branching.html [

Header
okänt
Footer

]

Changes.html [
    
    Header
    okänt
    Footer

]

Project.html [

    Header
    okänt
    Footer

]

Vad är master.css och vad får jag göra i den?

Master.css använder vi för globala variabler, att en variabel är global innebär att du kan använda den överallt i koden, till och med utanför master.css filen.
Såhär kan det se ut innuti master.css

:root {
    --headerColor: red;
}

Om du då befinner dig i exempelvis changes.css så kan du applicera detta till din header class.
.header {
    background-color: var(--headerColor);
}