# 🛟 Informe Patera

Aplicación web para generar el **mensaje inicial** de cada patera y gestionar sus **fotos** (UF y Menas), con base de datos local por patera. Se instala en el móvil como una app y **no necesita servidor**: todos los datos se guardan en el propio dispositivo.

> **Archivo de la app:** `index.html` (un único archivo).

---

## 📑 Índice

1. [Instalar la app en el móvil](#1-instalar-la-app-en-el-móvil)
2. [Pantalla inicial y pateras](#2-pantalla-inicial-y-pateras)
3. [Mensaje inicial: rellenar los campos](#3-mensaje-inicial-rellenar-los-campos)
4. [Finalizar y compartir el mensaje](#4-finalizar-y-compartir-el-mensaje)
5. [Fotos: UF y Menas](#5-fotos-uf-y-menas)
6. [Finalizar las fotos y crear el ZIP](#6-finalizar-las-fotos-y-crear-el-zip)
7. [Enviar un ZIP descargado (Chrome y Safari)](#7-enviar-un-zip-descargado-chrome-y-safari)
8. [Borrar pateras](#8-borrar-pateras)
9. [Problemas frecuentes](#9-problemas-frecuentes)
10. [Publicar la app en GitHub Pages](#10-publicar-la-app-en-github-pages)

---

## 1. Instalar la app en el móvil

Así tendrás un icono junto a tus demás apps, sin abrir el navegador cada vez.

### 🤖 Android (Chrome)

| Paso | Qué hacer |
|---|---|
| 1️⃣ | Abre el enlace en **Chrome**. No lo abras desde WhatsApp ni otra app: copia el enlace y pégalo en Chrome. |
| 2️⃣ | Pulsa los **3 puntos** (⋮) arriba a la derecha. |
| 3️⃣ | Elige **"Añadir a pantalla de inicio"** (en algunos móviles: **"Instalar aplicación"**). |
| 4️⃣ | Pulsa **Añadir / Instalar**. El icono aparece en la pantalla de inicio y en el menú de apps. |

### 🍎 iPhone (Safari)

| Paso | Qué hacer |
|---|---|
| 1️⃣ | Abre el enlace en **Safari** (en otros navegadores no aparece la opción). |
| 2️⃣ | Pulsa **Compartir** (cuadrado con flecha hacia arriba, en la barra inferior). |
| 3️⃣ | Desliza y elige **"Añadir a pantalla de inicio"**. Si no la ves, baja hasta el final de la lista. |
| 4️⃣ | Pulsa **Añadir**. El icono queda en la pantalla de inicio. |

> 💡 **Después de instalarla**, abre siempre la app desde su icono. Los textos pueden variar según la marca y la versión del sistema.
>
> ⚠️ Tus pateras y fotos se guardan **en el móvil**. Si borras los datos del navegador, también se borran.

---

## 2. Pantalla inicial y pateras

```
┌──────────────────────────┐
│ ☰  Informe Patera        │
├──────────────────────────┤
│ Nueva patera (número)    │
│ [ 129                  ] │ ① Escribe el número
│ [   Crear patera       ] │ ② Pulsa Crear patera
│ [ 🟨 GUIA DE USO 🟨    ] │ ③ Abre la guía
│                          │
│ Pateras guardadas        │
│ ┌──────────────────────┐ │
│ │ Patera 129 · 12 fotos│ │ ④ Toca para abrir
│ └──────────────────────┘ │
└──────────────────────────┘
```

1. **Escribe el número** de la patera (por ejemplo `129`).
2. Pulsa **Crear patera**. Si el número ya existe, abre la que ya tenías.
3. El botón amarillo **GUIA DE USO** abre la guía en PDF. Abajo, siempre visible, el botón **Manual detallado** abre este manual.
4. En **Pateras guardadas**, toca una para abrirla, cambiar de patera y editar sus campos y fotos.
5. El botón **☰** (arriba a la izquierda) abre el menú:

| Opción del menú | Para qué sirve |
|---|---|
| 🗂 Pateras | Lista, crear y cambiar de patera |
| 📝 Mensaje inicial | Rellenar y compartir el informe |
| 📷 Fotos | Fotos UF y Menas y ZIP |
| 🗑 Borrar pateras | Eliminar datos y fotos del móvil |

---

## 3. Mensaje inicial: rellenar los campos

Abre **☰ → Mensaje inicial**. Todo se **guarda solo** mientras escribes.

- **Selectores con "Otro":** en *Lugar de llegada*, *Requirente* y *Motores*, si eliges "Otro" aparece un cuadro para escribirlo.
- **Cantidades:** solo números. Los campos de pulseras aparecen un poco a la derecha, dentro de su categoría (por ejemplo, dentro de *Menas varones*).
- **Pulseras:** escríbelas como quieras: `1, 2, 3`, `1,2,3`, `P1,P2,P3` o `P 1, P 2, P 3`. Al pasar al siguiente campo se ven así: `P1, P2, P3`.
- **Unidades familiares y vinculadas:** escribe cuántas hay y aparecen casillas numeradas. La casilla 1 trae un ejemplo (`Px padre Py hijo` en UF, `Px hermano mayor Py hermano menor` en UV): edítalo o bórralo. Si no lo tocas, no sale en el mensaje.
- **Nacionalidades:** debajo del cuadro hay botones **+Senegal, +Gambia, +Guinea, +Mauritania, +Guinea Bissau y +Costa Marfil**. Al pulsarlos se añaden al cuadro, sin repetir. También puedes escribir a mano.
- **Textos ya escritos:** *Avistamiento*, *Datos del rescate*, *Quién realiza el rescate* y *Datos embarcación* vienen con un texto escrito. Edítalo o bórralo.

### Qué escribes y qué sale en el mensaje

| Escribes | Se ve en el campo | Sale en el mensaje |
|---|---|---|
| `17, 18` | `P17, P18` | `P-17 y P-18.` |
| `P1,P2,P3` | `P1, P2, P3` | `P-1, P-2 y P-3.` |
| `P 4, P 5` | `P4, P5` | `P-4 y P-5.` |
| *(vacío)* | *(vacío)* | Sin pulseras en esa línea |

---

## 4. Finalizar y compartir el mensaje

1. Pulsa **Finalizar mensaje inicial** (al final de la pantalla).
2. **Aviso de totales:** la app comprueba que

   `TOTAL PERSONAS = TOTAL MENORES + MUJERES ADULTAS + HOMBRES ADULTOS`

   Si no coincide, muestra la **diferencia**.

   ```
   ⚠ Los totales no coinciden
   TOTAL PERSONAS: 56
   Menores + mujeres + hombres: 55
   Diferencia: 1
   [ Finalizar de todos modos ]
   [ Volver a editar ]
   ```

3. Tú decides: **Volver a editar** para corregir, o **Finalizar de todos modos** si es correcto así.
4. Se abre el **menú de compartir** del móvil: WhatsApp, correo, etc. Los totales salen en negrita en WhatsApp.
5. Si no se abre, aparece una ventana con **Copiar mensaje**, **Enviar por WhatsApp** y **Enviar por correo**.
6. **Ver / compartir mensaje** muestra el texto completo para revisarlo y volver a enviarlo más tarde.

> ✅ **Ejemplo que cuadra:** 55 personas = 8 menores + 5 mujeres adultas + 42 hombres adultos. No sale ningún aviso.

---

## 5. Fotos: UF y Menas

Abre **☰ → Fotos**. Hay cuatro zonas, en este orden: **Fotos UF**, **Fotos hoja de filiación UF**, **Fotos Menas** y **Fotos hoja de filiación MENAS**.

1. **📷 Hacer foto:** abre la cámara. La primera vez, el móvil pide permiso: pulsa **Permitir**.
2. **🖼 Añadir desde la galería:** elige una o varias fotos que ya tengas.
3. **Escribe el nombre** en el cuadro de debajo de cada foto:

| Zona | Título del cuadro | Ejemplos |
|---|---|---|
| **UF** y su hoja de filiación | Introducir N°UF-N°Foto | `1-1`, `2-1`, `2-2`, `3-1` |
| **Menas** y su hoja de filiación | Introducir N°Pulsera menor | `1`, `2` |

4. **✕ (roja):** quita una foto.

> ⚠️ El archivo se llamará **exactamente** como lo escribas. Si dejas una foto sin nombre, se guardará como `sin_nombre_1`, `sin_nombre_2`… Si repites un nombre en la misma carpeta, se añade `_2` para no perder ninguna.

---

## 6. Finalizar las fotos y crear el ZIP

1. Pulsa **Finalizar y descargar ZIP** (pon nombre a todas las fotos antes).
2. Espera unos segundos: el botón muestra *Comprimiendo…*
3. Aparece la ventana del ZIP con el botón **⬇ Descargar ZIP** y un aviso de lo que hacer después.
4. **Correo de destino (opcional):** encima del botón final hay un cuadro para guardar el correo al que envías, con un botón **Copiar** para pegarlo al enviar. Se guarda en el móvil.
5. **Compártelo desde Descargas:** la app no puede enviar el ZIP por sí sola. Ábrelo desde Descargas o Archivos y compártelo por correo o WhatsApp (sección 7).

El archivo se llama **`Fotos Patera X UF+MENAS.zip`**, donde X es el número de la patera.

### Qué contiene el ZIP

```
Fotos/
├── UF/
│   ├── 1-1.jpg
│   └── Hoja de filiación UF/
│       └── 1-1.jpg
└── Menas/
    ├── 1.jpg
    └── Hoja de filiación MENAS/
        └── 1.jpg
```

---

## 7. Enviar un ZIP descargado (Chrome y Safari)

El ZIP se descarga en el móvil. Así lo envías por correo o WhatsApp:

### 🤖 Android (Chrome)

1. **Abre la descarga:** baja la barra de notificaciones y toca *Descarga completa*, o ve a Chrome → ⋮ → **Descargas**.
2. **Busca el ZIP:** se llama `Fotos Patera 129 UF+MENAS.zip` (el número es el de tu patera).
3. **Pulsa Compartir:** mantén pulsado el archivo, o toca sus 3 puntos, y elige **Compartir**. Si no aparece, abre la app **Archivos → Descargas**.
4. **Elige dónde enviarlo:** WhatsApp, Gmail, Drive… No hace falta descomprimirlo.

### 🍎 iPhone (Safari)

1. **Pulsa Descargar** cuando Safari pregunte si quieres descargar el archivo.
2. **Abre la descarga:** toca el icono de flecha en la barra de direcciones y elige el ZIP, o ve a la app **Archivos → Descargas**.
3. **Pulsa Compartir:** mantén pulsado el ZIP y elige **Compartir**. **No lo abras**, porque el iPhone lo descomprime.
4. **Elige dónde enviarlo:** WhatsApp, Mail, AirDrop…

> 📧 El correo suele limitar los adjuntos a unos 25 MB. Si pesa más, usa WhatsApp o Drive.

---

## 8. Borrar pateras

1. **☰ → Borrar pateras:** se muestra la lista con el número de fotos de cada una.
2. **Marca** las pateras a borrar (puedes marcar varias).
3. Pulsa **Borrar seleccionadas**. El botón cambia a *"Pulsa otra vez para confirmar el borrado"*: púlsalo otra vez.

> 🚨 **Atención:** se borran los datos y las fotos del móvil y **no se pueden recuperar**. Envía antes el mensaje y el ZIP.

---

## 9. Problemas frecuentes

| Problema | Solución |
|---|---|
| La cámara o la galería no se abren | Abre la app en Chrome o Safari (o desde su icono), no desde WhatsApp ni desde el visor de otra app. Revisa que el permiso de cámara esté en **Permitir**. |
| La app no envía el ZIP | Es normal: el navegador no lo permite. Descárgalo y compártelo desde Descargas o Archivos (sección 7). |
| Salta el aviso de totales | Revisa *Total personas*, *Total menores*, *Mujeres adultas* y *Hombres adultos*. Si es correcto, pulsa **Finalizar de todos modos**. |
| Se han perdido las pateras | Pasa si se borran los datos del navegador o se desinstala la app. Envía siempre el mensaje y el ZIP al terminar. |
| Falla al crear el ZIP | Necesitas conexión a internet al menos la primera vez (carga el compresor ZIP). |

---

## 10. Publicar la app en GitHub Pages

1. Crea una cuenta en [github.com](https://github.com) y un **repositorio nuevo** (por ejemplo `informe-patera`), público.
2. Sube a la raíz del repositorio el archivo **`index.html`** (opción *Add file → Upload files*). Puedes subir también este `README.md`.
3. Ve a **Settings → Pages**.
4. En *Source* elige **Deploy from a branch**, rama **main** y carpeta **/ (root)**. Pulsa **Save**.
5. Espera uno o dos minutos. GitHub muestra la dirección de la web, normalmente `https://TU-USUARIO.github.io/informe-patera/`.
6. Abre esa dirección en el móvil y sigue el apartado [1. Instalar la app](#1-instalar-la-app-en-el-móvil).

> Los nombres de los menús de GitHub pueden cambiar un poco con el tiempo.
>
> 🔓 Una web de GitHub Pages es pública para quien tenga el enlace, pero **los datos de cada usuario se guardan solo en su móvil**.
>
> 🔄 Para actualizar la app, sube el nuevo `index.html` al mismo repositorio sustituyendo el anterior.

---

## 🧱 Notas técnicas

- App de un solo archivo HTML, sin servidor.
- Datos y fotos guardados localmente en el navegador (IndexedDB).
- El ZIP se genera en el móvil con [JSZip](https://stuk.github.io/jszip/) (cargado desde cdnjs).
- Para compartir se usa la función de compartir del sistema (Web Share API) cuando está disponible.
