# CD-LAC SharePoint · espejo público de la maqueta

Piezas interactivas de la maqueta del SharePoint de **Design Technology LAC** (Gensler), servidas con GitHub Pages para incrustarlas en las páginas v2 con el web part **Embed**.

**No edites este repo a mano.** Se genera automáticamente desde el repo privado `ramon-garcia-ayala-gensler/cd-lac-sharepoint`; cualquier cambio directo en `index.html`, `img/` o `brand-kit/index.html` se sobrescribe en el siguiente sync.

## De dónde sale

| Repo privado (fuente) | Aquí |
|---|---|
| `maqueta/index.html` | `index.html` |
| `maqueta/img/**` | `img/**` |
| `docs/brand-kit/index.html` | `brand-kit/index.html` |

Cada push a `main` del repo privado que toca esos archivos corre la GitHub Action *Sync espejo público*, que hace aquí un commit `sync desde cd-lac-sharepoint@<sha>`. GitHub Pages (rama `main`, carpeta `/`) se reconstruye solo.

Dependencia: **SharePoint → este espejo → repo privado.** Este README no lo toca el sync.

## URLs

- Maqueta completa: https://ramon-garcia-ayala-gensler.github.io/cd-lac-sharepoint-maqueta/
- Brand kit: https://ramon-garcia-ayala-gensler.github.io/cd-lac-sharepoint-maqueta/brand-kit/
- Una pieza sola (para el Embed): `https://ramon-garcia-ayala-gensler.github.io/cd-lac-sharepoint-maqueta/?embed=<pieza>`

| Pieza | Página v2 |
|---|---|
| `header`, `clusters`, `impact`, `team` | v2-Home |
| `clusters` | v2-Clusters |
| `banner-vdc` · `banner-rc` · `banner-cd` · `banner-di` | v2-Cluster-VDC · RC · CD · DI |
| `tools` | v2-Tools |
| `onboarding` | v2-Learning |
| `graph` | v2-Community |
| `matrix` | v2-Projects |
| `impact` | v2-Plantillas |

El web part Embed no ajusta el alto solo: usa el alto sugerido de cada pieza (está en el repo privado, `receta/embeds.json`).

## Requisito en SharePoint

El dominio `ramon-garcia-ayala-gensler.github.io` tiene que estar permitido en *Configuración del sitio › Seguridad de campo HTML* del sitio que incrusta las piezas.

## Contenido

Incluye fotos y nombres reales del equipo de DT LAC, publicados con autorización.
