# HDFull Castellano – Plugin para Nuvio

Plugin mínimo solo con el provider **HDFull** (español de España / castellano).

Basado en el scraper de [ticolibre/NuvioLatam](https://github.com/ticolibre/NuvioLatam).

## Instalación

1. Sube esta carpeta a un repositorio de GitHub (público).
2. En Nuvio: **Profile → Content & Discovery → Plugins**
3. Pega la URL del manifiesto, por ejemplo:

```
https://raw.githubusercontent.com/TU_USUARIO/TU_REPO/main/manifest.json
```

4. Instala el repositorio y activa el scraper **HDFull**.

## Importante: el dominio cambia

El scraper usa un dominio fijo. Ahora mismo está en:

```js
const HF_BASE = 'https://hdfull.love';
```

(archivo `providers/hdfull.js`, cerca de la línea 1810)

Cuando HDFull cambie de dominio (pasa a menudo):

1. Abre `providers/hdfull.js`
2. Cambia `HF_BASE` al dominio que esté activo
3. Haz commit y push
4. En Nuvio, actualiza / reinstala el plugin

Dominios habituales a probar: `hdfull.love`, `hdfull.today`, `hdfull.one`, `hdfull.org`, etc. (comprueba cuál responde en el momento).

## Limitaciones

- Depende de que el dominio actual de HDFull esté online y no bloqueado.
- Cloudflare u otros protecciones pueden hacer que falle de forma intermitente.
- No sustituye a Torrentio + MejorTorrent/Wolfmax4k si buscas cobertura estable en castellano.

## Aviso

Este plugin no aloja contenido. Solo busca enlaces públicos en sitios de terceros. Usa bajo tu responsabilidad y según la legislación de tu país.
