# Spanish-ANSI
Mi configuración personal de keylayout para teclado ANSI que permite escribir en español: tildes, eñe (ñ), signos invertidos (¿¡) y caracteres especiales, sin necesidad de cambiar la distribución física del teclado.

Como programador, descubrí que los teclados con la distribución ANSI me resultaban más cómodos para escribir código. Pero también utilizo el mismo teclado para comunicarme en español, lo que requería poder introducir de manera ágil y sencilla los símbolos de este idioma.

Probé algunas alternativas como configurar Karabiner o utilizar el keylayout adaptado para idiomas internacionales de [keylayout-en-intl-altgr-dead-keys](https://github.com/bteixeira/keylayout-en-intl-altgr-dead-keys)), pero introducían pequeños inconvenientes como un retardo en las tildes que hacía que la siguiente vocal también saliese con la tilde al escribir rápido o lag al cambiar de capa cambiando de orden las letras escribiendo las siguientes antes de la que llevaba tilde. Además se perdían algunos atajos de teclados como pegar sin formato (Command + Option + Shift + V).

Por tanto decidí hacer un keylayout personal con mis propias preferencias. No necesito todos los caracteres especiales de todos los idiomas, busco simpleza. Este keylayout toma como base el keylayout ABC por defecto de MacOS y le introduce los siguientes cambios:

| Combinación de teclas       | Resultado | Descripción                                                 |
|-----------------------------|:---------:|-------------------------------------------------------------|
| `´` (deadkey)               | —         | Espera una vocal para añadir la tilde (ej: `´` + `a` = `á`) |
| `Option + '`                | `'`       | Escribe el apóstrofo recto                                  |
| `Shift + '`                 | `"`       | Escribe la comilla doble                                    |
| `Option + E`                | `€`       | Escribe el símbolo del euro                                 |
| `Option + N`                | `ñ`       | Escribe la letra eñe directamente                           |
| `Option + Shift + N`        | `Ñ`       | Escribe la letra eñe mayúscula directamente                 |
| ``Option + Shift + ` ``     | `˜`       | Recupera la virgulilla que se pierde en la tecla N ¹        |
| `Option + /`                | `¿`       | Signo de apertura de interrogación                          |
| `Option + Shift + /`        | `÷`       | Símbolo de división                                         |
| Resto del layout            | —         | Se mantiene exactamente igual al original                   |

¹: No es la misma que la tilde ~. No creo que la vaya a usar la virgulilla sin la n o una vocal debajo, pero por si acaso.
