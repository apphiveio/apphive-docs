---
description: "Cómo conectar un dominio propio (por ejemplo app.tuempresa.com) a tu web app de Apphive: los dos registros CNAME que debes crear en tu DNS."
---

# Dominio propio para tu web app

Puedes publicar tu web app en un subdominio tuyo, por ejemplo `app.tuempresa.com`, en lugar de la dirección de Apphive.

## Antes de empezar

- La app debe tener **al menos una compilación de web app** terminada.
- Solo el **dueño del proyecto** puede configurar el dominio.
- Se usa un **subdominio** (`app.tuempresa.com`, `www.tuempresa.com`…). El dominio raíz solo (`tuempresa.com`) no se puede usar.

## 1. Registra el dominio en Apphive

En la configuración de la web app, en **Dominio personalizado**, llena:

- **Subdomain:** solo la primera parte (`app`). Entre 3 y 15 caracteres, solo letras minúsculas y números. Si lo dejas vacío se usa `www`.
- **Host:** tu dominio (`tuempresa.com`).

## 2. Crea los dos registros en tu DNS

Al registrarlo, Apphive te muestra **dos registros CNAME**. Créalos tal cual en el panel donde administras tu dominio (GoDaddy, Cloudflare, Hostinger…):

| Para qué | Nombre | Apunta a |
|---|---|---|
| Tráfico de tu web app | tu subdominio (`app`) | la dirección que termina en `.cloudfront.net` |
| Validación del certificado | el nombre que empieza con `_` | la dirección que termina en `.acm-validations.aws` |

!!! warning "Si usas Cloudflare"
    Deja los dos registros en **«Solo DNS»** (nube gris), no en modo proxy.

## 3. Espera la activación

Cuando los dos registros existen, el certificado de seguridad (HTTPS) se valida y el dominio se activa solo. Puede tardar **de unos minutos a unas horas**. Si pasan más de 24 horas, revisa que los dos CNAME estén escritos exactamente como te los mostró Apphive.

!!! tip "Cambiar de dominio"
    Cada web app tiene un dominio a la vez. Para cambiarlo, primero quita el actual desde la misma pantalla.
