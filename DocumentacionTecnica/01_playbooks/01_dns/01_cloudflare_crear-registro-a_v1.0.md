# Guía para Crear un Registro A en Cloudflare v1.0

## Descripción

Este documento describe los pasos necesarios para crear un registro A en Cloudflare. Un registro A se utiliza para asociar un nombre de dominio con una dirección IP (IPv4). Esto es útil cuando deseas que tu dominio apunte a un servidor específico.

## Requisitos Previos

Antes de comenzar, asegúrate de tener:

- Acceso a tu cuenta de Cloudflare.
- El dominio que deseas configurar ya agregado a tu cuenta de Cloudflare.
- La dirección IP (IPv4) del servidor al que deseas apuntar el dominio.

## Pasos para Crear un Registro A

### Paso 1: Iniciar sesión en Cloudflare

1. Dirígete a [Cloudflare](https://www.cloudflare.com/) y haz login con tus credenciales.
2. En el panel de control, selecciona el dominio para el cual deseas crear el registro A.

### Paso 2: Acceder a la Configuración de DNS

1. En la barra de navegación superior, selecciona la opción **DNS**.
2. Esto te llevará a la página donde podrás gestionar los registros DNS para tu dominio.

### Paso 3: Crear un Nuevo Registro A

1. En la página de DNS, verás una tabla con todos los registros DNS actuales. 
2. Haz clic en el botón **Add record** (Agregar registro).
3. En el formulario que aparece, selecciona **A** en el campo **Type**.
4. En el campo **Name**, ingresa el subdominio que deseas asociar con la IP (por ejemplo, "www" o "api").
5. En el campo **IPv4 address**, ingresa la dirección IP del servidor al que deseas apuntar el dominio.
6. Deja el campo **TTL** (Time to Live) en **Auto** para que Cloudflare administre la configuración automáticamente.
7. Si deseas que el tráfico pase a través de Cloudflare (lo que mejorará la seguridad y rendimiento), asegúrate de que el ícono de la nube esté **naranja**. Si prefieres que el tráfico pase directamente al servidor sin pasar por Cloudflare, haz clic en la nube para que se vuelva **gris**.

### Paso 4: Guardar el Registro

1. Una vez completados los campos, haz clic en **Save** (Guardar).
2. El registro A se añadirá a la lista de registros DNS de tu dominio.

### Paso 5: Verificación

1. La propagación del nuevo registro A puede tomar algunos minutos. Para verificar si el registro se ha configurado correctamente, puedes usar herramientas como [Whatsmydns](https://www.whatsmydns.net/) para comprobar si el dominio resuelve correctamente a la IP configurada.

## Notas

- Los cambios en DNS pueden tardar algunos minutos en propagarse por completo a nivel global.
- Si tienes problemas con la propagación del registro, puedes intentar borrar el caché de DNS de tu dispositivo local.

## Conclusión

¡Listo! Ahora has configurado un registro A en Cloudflare para tu dominio. Esto debería permitir que el dominio resuelva a la dirección IP que configuraste. Si tienes más configuraciones DNS que hacer, repite estos pasos para cada nuevo registro.

