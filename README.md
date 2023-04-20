# Circle Menu

## Descripción

Efecto css y html basado en el tutorial de youtube sobre HTML y CSS de Easy Learn Axis.

[URL a tutorial Easy Learn Axis](https://www.youtube.com/watch?v=R7e9QguUPrQ)

## Muestra

![](./img/muestra.png)


## Uso

```js
    // Asignacion al id open-menu, evento click para que se produzca el efecto al hacer click sobre el circulo.
    window.onload =function(){ 
    var menuButton = document.getElementById("open-menu");
    menuButton.click();
    }; 
```
```css

/*Apuntamos al 2º elemento a con id menu de modo que queda oculto tras el primero con z-index*/

#menu:not(:target)>a:first-of-type,
#menu:target>a:last-of-type{
    opacity: 1;
    z-index: 1;
}

/*Rotamos y mostramos los elementos hijos del menu que estan ocultos antes de ejecutar el evento click*/

#menu:target>.menu-item:nth-child(6){
    transform: rotate(60deg)/*rota posicion hacia la derecha*/
    transLateY(-150px)/*marca distancia desde el menu-padre*/
    rotate(300deg);
    transition-delay: 0s;
}
```

## Links

[URL](https://github.com/AIPONCEP/CircleMenu.git)

[live site URL](https://aiponcep.github.io/CircleMenu/#menu)