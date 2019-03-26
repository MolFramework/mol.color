# Mol Colors #

Administra los colores de fondo, texto y borde basado en una paleta de color.
__
*Este proyecto utiliza [mol.normalize](https://github.com/mol-project/mol.normalize)*


## Uso e instalación
Para utilizar la paleta de color en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install https://github.com/mol-project/mol.colors.git
```
importa el archivo principal
```sh
@import '~mol.colors/scss/_colors.scss';
```
y crea un archivo que contenga las mismas variables que las que se encuentran en
el archivo de `~mol.colors/scss/_vars.scss`

ó si no tienes tiempo, importa el archivo minificado en tu hoja de estilos principal
```sh
@import '~mol.colors/dist/colors.min.css';
```


## Dev
Clona el repositorio
```sh
git clone https://github.com/mol-project/mol.colors.git
cd mol.colors/
npm install
```
Edita los archivos dentro de la carpeta de **scss**

#### Scripts
- `npm run dist` Actualiza los archivos minificados de la carpeta de distribución **dist**
- `npm run docs` Levanta un servidor local que se autorefresca con los cambios que se ejecuten en los archivos **scss** y actualiza los archivos de **docs**

#### Archivos
```text
mol.colors/
├── dist/
│   ├── colors.min.css
│   └── colors.min.css.map
├── docs/
│   ├── colors.css
│   ├── colors.css.map
│   └── index.html
└── scss/
    ├── _background.scss
    ├── _border.scss
    ├── _colors.scss
    ├── _image.scss
    ├── _line.scss
    ├── _text.scss
    ├── _vars.scss
    └── colors.scss
```

#### Variables para la paleta de color
```text
@import url('https://fonts.googleapis.com/css?family=Josefin+Sans|Open+Sans|PT+Serif');

$m-font-serif:      'PT Serif', serif;
$m-font-family:     'Open Sans', sans-serif;
$m-font-size:       16px;
$m-font-weight:     400;
$m-letter-spacing:  normal;
$m-line-height:     1.5em;

$m-code-family:     monospace;

$m-h-family:        'Josefin Sans', sans-serif;
$m-h-size:          23px;
$m-h-height:        1em;
$m-h-spacing:       normal;
$m-h-weight:        600;
$m-h-style:         normal;
$m-h-transform:     normal;

$m-background:  #fff;
$m-color:       #222029;

$m-primary:     #32bdc6;
$m-secondary:   #009DCE;
$m-accent:      #7175CB;

$m-note:        mix(#aaa, $m-primary, 90%);
$m-error:       mix(#f10, $m-primary, 80%);
$m-success:     mix(#1e1, $m-primary, 70%);
$m-warning:     mix(#fa3, $m-primary, 95%);

$m-container-border-width:  1px;
$m-container-border-style:  solid;

$m-array-background-color-variations: true;
$m-array-background-colors:
  (primary,   $m-primary),
  (secondary, $m-secondary),
  (accent,    $m-accent);

$m-array-border-color-variations: true;
$m-array-border-colors:
  (primary,   $m-primary),
  (secondary, $m-secondary),
  (accent,    $m-accent);

$m-underline-height: 4px;
$m-underline-width: 20px;
$m-array-line-colors:
  (primary,   $m-primary),
  (secondary, $m-secondary),
  (accent,    $m-accent);

$m-array-text-colors:
  (primary,   $m-primary),
  (secondary, $m-secondary),
  (accent,    $m-accent),
  (background,$m-background);

$m-array-img-blend:
  (multiply, multiply),
  (screen, screen),
  (lighten, lighten),
  (difference, difference),
  (burn, color-burn);

```

## Problemas conocidos

ヾ( ￣O￣)ツ Los estilos de linea no funcionaran en elementos que no pueden tener :after elments como cualquier input.

Σ(T□T) el blend mode para las clases de las imágenes no funciona en todos los navegadores [caniuse](https://caniuse.com/#feat=css-backgroundblendmode)
