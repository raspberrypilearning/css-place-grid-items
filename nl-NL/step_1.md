Een van de beste aspecten van een rasteropmaak is dat je items heel nauwkeurig kunt plaatsen.

### Standaard plaatsing

By default, when you put elements in a container with the `display: grid;` property, each item will take up **one grid cell** ordered first left to right and then top to bottom.

![An example grid with 6 items, the top row reads 1, 2, 3. De onderste rij is 4, 5, 6.](images/default-grid-placement.png)

Eén manier waarop je de plaatsing van jouw elementen kunt bepalen, is door de volgorde van de HTML zelf te wijzigen.

### Items over rijen en kolommen verspreiden

If you want to stretch elements so they cover more than one row or column, you can use the following properties:

- `grid-row-start` & `grid-row-end`
- `grid-column-start` & `grid-column-end`

De `grid-row-start` eigenschap is de **eerste** rij waarin het element wordt weergegeven.

`grid-row-end` is the row where the element ends. The image will **not** display on this row.

Hetzelfde geldt voor kolommen met `grid-column-start` & `grid-column-end`.

Je voegt deze eigenschappen toe aan de klasse van het element dat je wilt verspreiden.

## --- code ---

language: css
filename: style.css
---------------------------------------------------

.stretch-rows {
grid-row-start: 1;
grid-row-end: 3;
}

\--- /code ---

## --- code ---

language: css
filename: style.css
---------------------------------------------------

.stretch-columns {
grid-column-start: 2;
grid-column-end: 4;
}

\--- /code ---

![Het voorbeeldraster, met het item met nummer 1 verspreid over rij 1 en 2. Rasteritem 4 is verspreid over kolommen 2 en 3 in de onderste rij.](images/placing-grid-items.png)
