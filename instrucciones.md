# Instrucciones y funciones para proyecto en Metabank


*** Los links para vincular el programa en boostrap y scss ***
```html 
<link rel="stylesheet" href="assets/css/style.css" />
    <link rel="stylesheet" href="assets/css/fontawesome.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Roboto+Condensed:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet"> 
```


## Elementos del front end


**css:** 

- Fuentes:
```css
font-family: 'Roboto Condensed', sans-serif;
```

- Colores:
```css

    --color1:#0E1331;
    --color2:#4A517D;
    --color3:#3A50C9;
    --color4:#2C304A;
    --color5:#24327D; 

```

El boostrap se encuentra en una carpeta _node_modules_ para que se pueda abrir de manera offline sin cdn: 
se usaron los siguientes paquetes npm: ```sass por npm, bootstrap, fontawesome y autoprefixer```



- Al usar npm se **compila** escribiendo en la terminal de esta manera

```
npm run compile:sass
```

### Estructura de archivos:
Para más eficiencia, la estructura de archivos es

METABANK
-
- FRONTEND(AQUÍ SE PROBARON LOS HTML)
- IMAGENES(AQUÍ ESTÁ EL LOGO)
- IMG(IMAGENES QUE SE NECESITAN PARA LOS ASSETS)
- NODE_MODUES(AQUÍ SE ALOJA EL BOOSTRAP Y EL COMPILADOR DE SCSS)
- SCSS(AQUÍ DENTRO SE ENCUENTRAN LOS COMPONENTES Y SECCIONES, LOS CUÁLES VAN A IR CAMBIANDO PARA HACER LA PÁGINA MÁS ESTÉTICA CON EL PASO DEL TIEMPO)
  - Components
    - archivos.scss como animaciones, barras, mixins, buttons y typography
  - Sections
    - bancos.footer,form, into-section,loguin,navbar,registro 
  - _custom(Para modificar el boostrap)
  - fontawesome.scss(para modificar la tipografia)
- TODOS LOS HTMLS DEL PROYECTO *.HTML
<!-- - Pruebas unitarias
- conexión con el back -->

### Elementos que se repiten


Borde inferior
-
 <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320"><path fill="#ffffff" fill-opacity="1" d="M0,160L48,176C96,192,192,224,288,208C384,192,480,128,576,133.3C672,139,768,213,864,202.7C960,192,1056,96,1152,74.7C1248,53,1344,107,1392,133.3L1440,160L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path></svg>

----

El navbar
-
 ```html
  <nav class="navbar navbar-expand-lg navbar-dark menu shadow fixed-top">
        <div class="container"><a class="navbar-brand" href="#"><img src="/imagenes/log.ico/android-icon-48x48.png" alt="Metabank Logo"></a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
      
        <div class="collapse navbar-collapse justify-content-end" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item active">
              <a class="nav-link" href="/index.html">Inicio <span class="sr-only"></span></a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="registro.html">Registro</a>
            </li>
            <li class="nav-item"><a href="bancos.html" class="nav-link">bancos</a></li>
              <!--Estaría bueno un toggle por aquí pero me sale todo blanco-->
  
              <!-- <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">Bancolombia</a>
                <a class="dropdown-item" href="#">Davivienda</a>
                <a href="" class="dropdown-item">Nequi</a>
                <a href="" class="dropdown-item">Banco caja Social</a>
                <div class="dropdown-divider"></div>
                <a class="dropdown-item" href="#">¿No está tu banco?
                  Agregalo aquí
                </a>
              </div> -->
            </li>
            <li class="nav-item">
              <a class="nav-link disabled" href="#">ayuda</a>
            </li>
          </ul>
          <button type="button" class="rounded-pill btn-rounded">+57 321 6060 741 <span><i class="fas fa-phone-alt"></i></span></button>
         
        </div>
      </div>
    </nav>

```

el logo:
---
![Logo](imagenes/log.ico/android-icon-144x144.png)