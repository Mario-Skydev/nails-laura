# Página de reservas: cómo publicarla gratis en GitHub Pages

## Qué hay en esta carpeta

| Archivo | Para qué sirve |
|---|---|
| `index.html` | La página que ven las clientas: servicios, precios, día, hora y reserva por WhatsApp. |
| `admin.html` | El panel de administración donde la dueña cambia todo. |
| `config.json` | Los datos del negocio. El panel lo actualiza solo. |
| `LEEME.md` | Esta guía. |

## 1. Crear la cuenta y el repositorio

1. Crea una cuenta gratis en **github.com**.
2. Pulsa **+** (arriba a la derecha) y luego **New repository**.
3. Ponle un nombre corto, por ejemplo `unas-maria`. Será parte de la dirección web.
4. Márcalo como **Public**, que es necesario para usar GitHub Pages gratis, y pulsa **Create repository**.

## 2. Subir los archivos

1. En el repositorio, pulsa **Add file** y luego **Upload files**.
2. Arrastra `index.html`, `admin.html` y `config.json`.
3. Pulsa **Commit changes**.

## 3. Activar la página

1. En el repositorio, entra en **Settings** y luego en **Pages**.
2. En **Source** elige **Deploy from a branch**.
3. En **Branch** elige `main` y la carpeta `/ (root)`. Pulsa **Save**.
4. En 1 o 2 minutos aparece la dirección, por ejemplo:
   `https://TU-USUARIO.github.io/unas-maria/`

Esa es la dirección que se comparte con las clientas, en el estado de WhatsApp, en Instagram o en Facebook.

## 4. Crear la clave para el panel

1. En GitHub, abre tu foto y entra en **Settings**, luego en **Developer settings**, **Personal access tokens**, **Fine-grained tokens** y **Generate new token**.
2. **Token name:** "Panel reservas". **Expiration:** el máximo que permita. Cuando caduque, se crea otra igual.
3. En **Repository access** elige **Only select repositories** y marca el repositorio de la página.
4. En **Permissions**, busca **Contents** y elige **Read and write**.
5. Pulsa **Generate token** y copia la clave. Solo se muestra una vez.

## 5. Configurar el negocio

1. Abre `https://TU-USUARIO.github.io/unas-maria/admin.html`.
2. El usuario y el repositorio se rellenan solos. Pega la clave y pulsa **Conectar**.
3. Cambia el nombre, el logo, los colores, los servicios, los precios, el horario y el WhatsApp.
4. Usa **Vista previa** para ver cómo queda y **Guardar** para publicarlo. La página se actualiza en 1 o 2 minutos.

**Importante:** no compartas la dirección del panel ni la clave. La clave solo se guarda en el teléfono o la computadora donde la pegues. Si pierdes el dispositivo, borra la clave en GitHub (en el mismo sitio donde la creaste) y crea otra.

## Cómo funciona una reserva

1. La clienta elige servicios, día y hora, escribe su nombre y pulsa **Reservar por WhatsApp**.
2. Se abre WhatsApp con un mensaje ya escrito para el negocio. La clienta solo tiene que enviarlo.
3. La dueña responde para confirmar. Si esa hora ya está ocupada, propone otra.
4. La clienta puede pulsar **Añadir recordatorio a mi calendario**. Su teléfono le avisará 1 día antes y 2 horas antes.
5. Para cancelar o cambiar la cita, la clienta usa la sección **¿Necesitas cancelar o cambiar tu cita?**, que también envía un mensaje por WhatsApp.

### Consejo para la dueña: WhatsApp Business (gratis)

- **Respuestas rápidas:** por ejemplo, escribe `/confirmo` para enviar "¡Tu cita está confirmada! Te espero 💅".
- **Etiquetas:** "Cita confirmada" o "Mañana", para saber a quién mandar recordatorio.
- **Recordatorio del día antes:** con una respuesta rápida, por ejemplo `/recuerdo`.

## Límites que conviene conocer

- La página **no bloquea automáticamente** las horas ya reservadas. GitHub Pages no tiene servidor, así que las clientas no pueden guardar datos. La dueña lleva su agenda y confirma por WhatsApp.
- Los recordatorios automáticos dependen del calendario del teléfono de cada clienta. Enviarlos por WhatsApp de forma automática requiere la API de pago de Meta, que no está disponible en Cuba.
