# Responsividade

## CSS Units

### Unidades de medidas do CSS

#### Layout Fixo

`px` - Pixels

#### Layout Fluido

`%` - Porcentagem

`auto` - Automática

`vh` - Viewport Height

`vw` - Viewport Width

#### Textos Fixos

`1px` = 0.75pt

`16px` = 12pt

#### Texto Fluidos

`em` - Multiplicado pelo pai

`rem` - Multiplicado pelo root


```css
 {

    /* a cada 1rem será considerado 10px */
    
    font-size: 62.5%
}
```

## CSS Media Queries

```css
@media (max-width: 320px) {
    #form h3 {
        font-size: 2rem;
    }
}
```

## Em Impressoras

```html
<link rel="stylesheet" href="print.css" media="print"/>
```

## Em Tela

```html
<link rel="stylesheet" href="responsive.css" media="screen and (max-width: 768px)"/>
```

## HTML Media Attributes

## Imagens

HQ = Imagem media

MQ = Imagem menor

MaxRes = Imagem maior

```html
<picture class="image" alt="imagem">
    <source media="(min-width: 768px)" srcset="maxres.jpg">
    <source media="(min-width: 320px)" srcset="hqimagem.jpg">
    <source media="(min-width: 10px)" srcset="mqimagem.jpg">
    <img src="hqimagem.jpg" alt="Imagem">
```

`<picture>`

JPG, PNG vs SVG