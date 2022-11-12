# C.CSS-J.Torre-03-CSS-Grid-Basicos
- Se puede ver el resultado en el siguiente [enlace](https://santetes.github.io/C.CSS-J.Torre-03-CSS-Grid-Basicos/)

```css
/* 1 */
.grid-1{
    display: grid;
}

/* 2 */
.grid-2{
    display: grid;
    grid-template-columns: 300px 300px 300px;
}
.grid-2 .box:nth-child(2){
    grid-column: 1/2;
}

/* 3 */
.grid-3{
    display: grid;
    grid-template-rows: repeat(6, 300px);
}
.grid-3 .box:nth-child(2){
    grid-row: 1 / 2;
}

/* 4 */
.grid-4{
    display: grid;
    grid-template-rows: repeat(3, 300px);
    grid-template-columns: repeat(3, 300px);
}

.grid-4 .box:nth-child(2){
    background-color: black;
    grid-column: 2 / 4;
    grid-row: 1 / 3;
}

/* 5 */
.grid-5{
    display: grid;
    grid-template-rows: repeat(3, 300px);
    grid-template-columns: repeat(3, 300px);

    /* shortHand   rows/columns */ 
    grid: repeat(2, 300px)/ repeat(3 , 300px) ;

}

/* 6 */
.grid-6{
    display: grid;
    grid: repeat(2, 300px)/ repeat(3 , 300px) ;
    grid-auto-flow: dense;
}
.grid-6 .box:nth-child(2){
    grid-column: 1 / 2;
    
}

/* 7 */
.grid-7{
    display: grid;
    /* grid-template-columns: repeat(3, 1fr); */
    height: 1000px;
    grid: repeat(2, 1fr) / repeat(3, 1fr);
}

/* 8 */
.grid-8{
    display: grid;
    grid: repeat(2, 20rem) / repeat(3, 1fr);
    /* column-gap: 2rem;
    row-gap: 2rem; */
    gap: 2rem;
}

.grid-8 .box{
    margin-bottom: 0;
}

/* 9 */
.grid-9{
    display: grid;
    /* height: 120rem; */
    grid-template-areas: "header header header"
                         "nav nav nav"
                         "contenido contenido aside"
                         "footer footer footer"   ;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 25rem 10rem 80rem 25rem;
    gap: 1rem;
}
.grid-9 .box{
    margin: 0;
}
.grid-9 .box:nth-child(1){
    grid-area: header;
}
.grid-9 .box:nth-child(2){
    grid-area: nav;
}
.grid-9 .box:nth-child(3){
    grid-area: contenido;
}
.grid-9 .box:nth-child(4){
    grid-area: aside;
}
.grid-9 .box:nth-child(5){
    grid-area: footer;
}

/* 10 */
.grid-10{
    display: grid;
    height: 1200px;
    grid-template: "header header header" 2fr
                    "nav nav nav" 1fr
                    "aside contenido contenido" 6fr
                    "footer footer footer" 1fr / 1fr 1fr 1fr  ;
    gap: 1rem;
}

.grid-10 .box{
    margin: 0;
}
.grid-10 .box:nth-child(1){
    grid-area: header;
}
.grid-10 .box:nth-child(2){
    grid-area: nav;
}
.grid-10 .box:nth-child(3){
    grid-area: contenido;
}
.grid-10 .box:nth-child(4){
    grid-area: aside;
}
.grid-10 .box:nth-child(5){
    grid-area: footer;
}

/* 11 */
.grid-11{
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    height: 300px;
    border: 1px solid black;
    /* align-items: center; */
    place-content: center;
}

/* 12 */
.grid-12{
    display: grid;
    grid-template-columns: repeat(auto-fill, 200px);
    grid-template-columns: repeat(auto-fit, 200px);
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));

    /* 
    minmax(valor minimo fijo, valor proporcional cuando es mayor que valor minimo)
    quiere decir que va a cojer el espacio de 1fr hasta que al hacer mas pequeño el container 
    su valor se acerque al minimo, a partir de ese momento no será menor que esos 200px
    
    */

}
Footer
© 2022 GitHub, Inc.
Footer navigation
Terms
Privacy
Security
Status
Docs
Contact GitHub
Pricing
API
Training
Blog
About

```
