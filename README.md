# Bachelorproef toegepaste informatica

Deze repository bevat LaTeX sjablonen voor gebruik bij het opmaken van je bachelorproef toegepaste informatica zoals gevonden op [bachproef-latex-sjabloon](https://github.com/HoGentTIN/bachproef-latex-sjabloon):

- [Het onderzoeksvoorstel](./voorstel/)
- [De bachelorproef zelf](./bachproef/)
- [Een poster](./poster/)

Het voorblad van het bachelorproefsjabloon is conform aan datgene dat door de [scriptie-tool](https://scriptie.hogent.be/) wordt gegenereerd.

## Aan de slag

Voor aanbevelingen i.v.m. het onderzoeksproces en het gebruik van LaTeX voor het schrijven van een bachelorproef, kan je [deze praktische gids](https://github.com/hogenttin/bachproef-gids) nalezen. Je vindt er bv. uitleg over hoe je een onderwerp kan kiezen, hoe je een vergelijkende studie aanpakt, hoe je een literatuurstudie voert en dat op een correcte manier in LaTeX verwerkt, invoegen van afbeeldingen, enz.

## LaTeX editor, bibliografie

Qua editors voor LaTeX zijn er verschillende keuzemogelijkheden. We raden [TeXstudio](https://www.texstudio.org/) aan en [Jabref](https://www.jabref.org/) voor het bijhouden van een bibliografische databank. Enkele richtlijnen bij het configureren van deze applicaties:

### TeXstudio

Kies in het menu voor Options > Configure TeXstudio en pas volgende instellingen aan:

- Build:
    - Default compiler: "Latexmk"
    - Default Bibliography Tool: "Biber"
- Commands:
    - Latexmk: `latexmk -xelatex -shell-escape -synctex=1 -interaction=nonstopmode -file-line-error %`
- Editor:
    - Indentation mode: Indent and Unindent Automatically
    - Replace Indentation Tab by Spaces: Aanvinken
    - Replace Tab in Text by spaces: Aanvinken
    - Replace Double Quotes: English Quotes: ‘‘’’

Tips:

- Gebruik functietoets **F5** om het document te compileren en het resultaat te bekijken.
- Als na compilatie de bibliografie niet zichtbaar is, probeer die dan expliciet te compileren met **F8** en daarna opnieuw **F5**

### Jabref

Kies voor Options > Preferences en pas volgende instellingen aan:

- General:
    - Default encoding: UTF-8
    - Default library mode: biblatex
- File:
    - (optioneel) Main file directory: geef hier de directory waar je de PDFs van gevonden bronnen bijhoudt. Als je dezelfde bestandsnaam gebruikt als je BibtexKey, dan vindt JabRef de PDF en kan je die openen vanuit het overzicht.

## Bachelorproef in het Engels

Het bachelorproefsjabloon is voorzien op tekst in hetzij Nederlands, hetzij Engels. Wanneer je je bachelorproef in het Engels schrijft, moet je [lijn 52 van het hoofddocument](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/bachproef-tin.tex#L52) uit commentaar halen:

```latex
\selectlanguage{english}
```

Aandachtspunten:

- Het voorblad blijft in het Nederlands (behalve je titel), en dit is ook de bedoeling
- Je moet in dit geval ook een Nederlandse vertaling van je samenvatting voorzien. Het sjabloon houdt daar ook rekening mee:
    - De samenvatting in de hoofdtaal van het document komt [op lijn 40 van het LaTeX-bestand](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/samenvatting.tex#L40)
    - De Nederlandse vertaling ervan komt [op lijn 31](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/samenvatting.tex#L31)

## Bachelorproef in het Engels

Het bachelorproefsjabloon is voorzien op tekst in hetzij Nederlands, hetzij Engels. Wanneer je je bachelorproef in het Engels schrijft, moet je [lijn 54 van het hoofddocument](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/bachproef-tin.tex#L54) uit commentaar halen:

```latex
\selectlanguage{english}
```

Aandachtspunten:

- Het voorblad blijft in het Nederlands (behalve je titel), en dit is ook de bedoeling
- Je moet in dit geval ook een Nederlandse vertaling van je samenvatting voorzien. Het sjabloon houdt daar ook rekening mee:
    - De samenvatting in de hoofdtaal van het document komt [op lijn 40 van het LaTeX-bestand](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/samenvatting.tex#L40)
    - De Nederlandse vertaling ervan komt [op lijn 31](https://github.com/HoGentTIN/bachproef-latex-sjabloon/blob/master/bachproef/samenvatting.tex#L31)

## Bijdragen

- De vormgeving van het bachelorproefsjabloon is gebaseerd op het "[Legrand Orange Book](http://www.latextemplates.com/template/the-legrand-orange-book)" sjabloon door Mathias Legrand, met aanpassingen specifiek voor HoGent.
- De vormgeving van het sjabloon voor het onderzoeksvoorstel is gebaseerd op "Stylish Article", eveneens door Mathias Legrand.

Volgende personen hebben bijgedragen aan deze sjablonen:

- Bert Van Vreckem
- Jens Buysse
- Chantal Teerlinck
- Jeroen Maelbrancke
- Matts Devriendt
- Niels Corneille
- Patrick Van Brussel
- Simon Rondelez

