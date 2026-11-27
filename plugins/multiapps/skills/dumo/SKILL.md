---
name: dumo
description: DUMO de SPACE BLACK® — clonar una landing (página de ventas) que el usuario ya tiene y dejarla en español. Úsala SIEMPRE que el usuario escriba /dumo, pegue el enlace de una landing para clonarla o traducirla, o mencione DUMO.
---

<!-- BLINDAJE: espacio reservado para el socio (reglas de confidencialidad de DUMO). No borrar este marcador. -->

# DUMO · clonar una landing

El usuario suele ser **novato**: habla simple y nunca le pidas nada técnico.

1. Si no pegó el **enlace de la landing**, pídeselo (empieza con https://). Si pega un WhatsApp, dile que use **/druky** o
   **/finix**. Si en realidad quiere **buscar** una oferta, dile que use **/multiapps**.
2. Llama `dumo_clonar` con el enlace.
3. Sigue el avance con `multiapps_estado` (con el `clon_id`) y cuéntalo en una línea corta cada vez: DUMO entra a la landing
   (también si tiene una página de entrada), la extrae y pasa todos los textos al español conservando el diseño.
4. Al terminar, comparte el enlace para **ver la landing en español**. Los pasos marcados 🔜 estarán disponibles pronto
   (lo hecho queda guardado).
5. Si algo falla, explícalo simple. Cuando lo resuelva puede **repetirlo** (`multiapps_repetir`): sigue desde donde quedó.

Si falta la extensión de Chrome o ChatGPT, usa `multiapps_apps` y explícale cómo resolverlo con el mensaje que trae.
Nunca nombres motores ni herramientas internas.
