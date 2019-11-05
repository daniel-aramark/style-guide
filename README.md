## Variables
### Declaracón
El nombre de la variable es en *Camel Case*.
Para la declaración utilizaremos la sentencia ***inferencia de tipos*** en lugar del tipo.

Correcto:
```
var miNombreEnCamelCase = "Manolo";
```

Incorrecto:
```
string miNombreEnCamelCase = "Manolo";
```

#### Variables locales
El primer caracter será en minúscula. **nombreDeMiVariable**.
Serán lo más cortas posible.

```
public void MiMetodo()
{
    var nombre = "Manolo";
}
```

#### Variables globales públicas
El primer caracter será en mayúscula. **NombreDeMiVariable**.
Serán lo más descriptivas posible.

```
public string MiNombreDePila = "Manolo";
```

#### Variables globales privadas
El primer caracter será en minúscula. **nombreDeMiVariable**.
Serán lo más descriptivas posible.

```
private string miNombreDePila = "Manolo";
```

##### Ejemplo
```
private string miNombreDePila = "Manolo";
private string misApellidos = "García González";

public string GetNombreCompleto()
{
    var nombre = miNombreDePila + " " + misApellidos;
    return nombre;
}
```

## Contantes
El nombre será en *snake case* con todos los caracteres en mayúculas.

```
public const string MI_CONSTANTE = "Contante";
```

## Servicios
Se declaran globales, privados y readonly. La primera letra será minúscula y tendrá un guión bajo **_** al principio. **_miServicio**.oo

```
private readonly MiServicio _miServicio = new MiServicio();
```
