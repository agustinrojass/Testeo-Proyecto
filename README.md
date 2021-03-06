# UTN WALLET

Wallet virtual de la UTN para poder pagar el buffet, la fotocopiadora y la cuota de la carrera.

## Creado por

- Agustin Rojas
- Gonzalo Marsala
- Francisco Ugalde
- Zeus Testa

## Progreso semanal

| Semana | Progreso |
| - | - |
| Semana 1 | Funciones de creación de cuenta e inicio de sesión, menus de navegación. | 
| Semana 2 | Funciones de muestra "pantallas", estado de cuenta, datos personales, generación de token. |
| Semana 3 | Funciones de modificación de datos, acreditación, historiales, listas. |
| Semana 4 | Más funciones de muestra "pantallas", asteriscos para las contraseñas, modularización, alta y baja del alumno. |

## Referencia de colores

| Color  |  Imagen | Hex |
| - | - | - |
| Azul | ![#0037da](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Azul.png) | #0037da |
| Blanco | ![#f2f2f2](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Blanco.png) | #f2f2f2 |
| Gris | ![#767676](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Gris.png) | #767676 |
| Azul claro | ![#3b78ff](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Azul%20Claro.png) | #3b78ff |
| Rojo | ![#c50f1f](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Rojo.png) | #c50f1f |
| Verde | ![#13a10e](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Verde.png) | #13a10e |

## Vista de la aplicación

### Inicio

![Image text](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Screenshots/Inicio.png)

### Inicio de sesión

![Image text](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Screenshots/Inicio%20de%20sesi%C3%B3n.png)

### Estado de cuenta

![Image text](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Screenshots/Estado%20de%20cuenta%20alumno.png)

### Historial de transacciones

![Image text](https://github.com/agustinrojass/Prueba-Proyecto/blob/ar/Historial%20transacciones%20del%20alumno.png)

## Estructuras

```c
typedef struct  //STRUCT FECHA
{
    int dia;
    int mes;
    int ano;
} stFecha;
typedef struct  //STRUCT USUARIO
{
    char nombre[20];
    int dni;
    int edad;
    stFecha nacimiento;
    char usuario[20];
    char contrasena[20];
    float saldo;
} stUsuario;
typedef struct  //STRUCT ADMIN
{
    int tipo;
    char nombre[20];
    char usuario[20];
    char contrasena[20];
    float saldo;
} stAdmin;
typedef struct  //STRUCT TOKEN
{
    int token;
    int dni;
    char origen[20];
    char destino[20];
    char detalle[50];
    float monto;
    stFecha fecha;
    int acreditado;
} stToken;
```
