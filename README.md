# Mol Colors #

Administra los colores de fondo, texto y borde basado en una paleta de color.
__
*Este proyecto utiliza [mol.normalize](https://github.com/MolFramework/mol.normalize)*


( ﾟ▽ﾟ)/ Hi! [@MolFramework](https://twitter.com/MolFramework)


## Uso e instalación
Para utilizar la paleta de color en tu proyecto, puedes installarlo con [npm](https://www.npmjs.com/)
```sh
npm install https://github.com/MolFramework/mol.colors.git
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
git clone https://github.com/MolFramework/mol.colors.git
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
    ├── _colors.scss
    ├── _vars.scss
    └── colors.scss
```

#### Variables para la paleta de color
```text

```
