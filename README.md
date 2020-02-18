# angular-primeng

https://primefaces.org/primeng

Agregar los estilos glogales:

```javascript
{
    ... 
    "styles": [
              "src/styles.css",
              "node_modules/primeicons/primeicons.css",
              "node_modules/primeng/resources/themes/nova-light/theme.css",
              "node_modules/primeng/resources/primeng.min.css"
            ],
    ...
}
```

Ejemplo de uso de PrimeNG con Calendar:

```javascript
// src/app/app.module.ts
import {CalendarModule} from 'primeng/calendar';


@NgModule({
    ...  
    imports: [
        ...
        CalendarModule
    ],
    ...
})
export class AppModule { }

```

Y en el HTML:

```html
...

Calendario por defecto: 
<p-calendar></p-calendar> <br /><br />

Calendario Date Format: 
<p-calendar dateFormat="yy-mm-dd"></p-calendar> <br />

...
<router-outlet></router-outlet>
```