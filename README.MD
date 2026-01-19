Este documento explica cómo reproducir un grafo de commits con dos ramas y un merge final.


## 1. Commit A (rama main)
Crea el archivo readme1.md

Escribe:
```# Inicio del proyecto```

Abre la ventana Commit

Escribe el mensaje:
```A: Inicio del proyecto```

Pulsa Commit

## 2. Commit B (rama main)
Edita readme1.md y añade:
```- Añadido contenido base```

Abre la ventana Commit

Mensaje:
```B: Añadido contenido base```

Pulsa Commit

## 3. Crear la rama exp
En la parte inferior derecha debería aparecer la rama actual: main

Haz clic en ese botón

Selecciona New Branch…

Nombre: exp

Marca Checkout branch para cambiarte a ella

Pulsa Create

## 4. Commit C (rama exp)
Crea el archivo readme2.md

Escribe:
```# Experimentos```

Abre la ventana Commit

Mensaje:
```C: Inicio de experimentos```

Pulsa Commit

## 5. Commit D (rama exp)
Edita readme2.md y añade:
```- Añadido prueba experimental```

Abre la ventana Commit

Mensaje:
```D: Añadido prueba experimental```

Pulsa Commit

## 6. Volver a la rama main
En la esquina inferior derecha, haz clic en exp

Selecciona Checkout main

## 7. Commit E (rama main)
Edita readme1.md y añade:
```- Añadido sección final```

Abre la ventana Commit

Mensaje:
```E: Añadido sección final```

Pulsa Commit

## 8. Commit F (rama main)
Edita readme1.md y añade:
```- Cierre del documento```

Abre la ventana Commit

Mensaje:
```F: Cierre del documento```

Pulsa Commit

## 10. Merge de exp → main
En la esquina inferior derecha, haz clic en main

Selecciona Merge into Current…

Elige la rama exp

Confirma el merge

PyCharm integrará los commits C y D en la rama principal.

## Resultado final
En Git → Log podrás ver un grafo idéntico al del ejercicio:

Línea principal: A → B → E → F

Rama secundaria: B → C → D

Merge final hacia F