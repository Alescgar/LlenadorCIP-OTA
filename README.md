# LlenadorCIP OTA

Canal público oficial de actualización para el firmware Llenador CIP.

Este repositorio contiene únicamente imágenes binarias compiladas y sus
manifiestos de integridad. El código fuente, la configuración de instalaciones,
las contraseñas y los tokens permanecen en el repositorio privado.

Los ESP32 consultan:

```text
https://raw.githubusercontent.com/Alescgar/LlenadorCIP-OTA/main/releases/latest.json
```

Cada manifiesto declara versión, tamaño y SHA-256. El firmware descarga en
streaming a la partición alternativa, comprueba el hash y valida la imagen
antes de reiniciar.

No se debe borrar una versión todavía instalada en clientes. Las releases
publicadas son inmutables.
