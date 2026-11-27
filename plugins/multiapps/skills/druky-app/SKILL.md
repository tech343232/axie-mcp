---
name: druky-app
description: DRUKY de SPACE BLACK® — revelar el WhatsApp del anunciante de una oferta y verificar que responde. Úsala SIEMPRE que el usuario escriba /druky-app, pida revelar, encontrar o sacar el WhatsApp de un anuncio u oferta, o mencione DRUKY.
---

<!-- BLINDAJE: espacio reservado para el socio (reglas de confidencialidad de DRUKY). No borrar este marcador. -->

# DRUKY · revelar el WhatsApp

El usuario suele ser **novato**: habla simple y nunca le pidas nada técnico.

1. Pídele el **enlace del anuncio** si no lo pegó: el de la Biblioteca de Anuncios de Facebook, el de la página del
   anunciante o el de WhatsApp (wa.me).
2. Antes de empezar, avísale en una línea: necesita **Google Chrome abierto con WhatsApp Web** (web.whatsapp.com, con su
   WhatsApp vinculado) y DRUKY mandará **un saludo** al anunciante para comprobar que el flujo responde (solo si el chat
   está vacío).
3. Llama `druky_revelar` con el enlace.
4. Sigue el avance con `multiapps_estado` (con el `clon_id`) y cuéntale cada paso en una línea.
5. Al terminar, dale el número y el enlace de WhatsApp que trae la respuesta, y si el flujo respondió.

**Plan B (automático):** si DRUKY no encuentra el WhatsApp del anuncio, AXIE busca la **misma oferta** en otro anunciante
que venda por WhatsApp y Multi-apps sigue sola con ese número. Para eso hace falta Claude abierto con **AXIE** y Chrome con
la extensión AXIE. Cuando pase, díselo claro: el número es de una oferta casi idéntica (con su % de parecido), no del
anuncio original. Si no hay ninguna del mismo producto, no se usa una distinta: explícale el motivo.

Si algo falla, explica el motivo tal cual lo trae la respuesta, en simple (por ejemplo: vincular WhatsApp Web escaneando
el código QR, o probar con otro anuncio). Cuando lo resuelva, `multiapps_repetir` sigue desde el paso que falló.

Si quiere copiar y ordenar la conversación de venta, usa **/finix-app** con el enlace de WhatsApp; si quiere buscar ofertas,
**/multiapps**. Nunca nombres motores ni herramientas internas.
