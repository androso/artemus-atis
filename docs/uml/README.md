# Diagrama de Clases — Artemus App (Práctica 03)

Modelo estructural UML del dominio derivado del Product Backlog (US-01 a US-10).

- Fuente Mermaid: `diagrama_clases_artemus.mmd`
- Imagen exportada: `diagrama_clases_artemus.png`

## Entidades

| HU | Entidades |
|---|---|
| US-01 | `Usuario`, `RolUsuario` |
| US-02 | `Terreno`, `OrientacionCardinal` |
| US-03 | `EspacioRequerido` |
| US-04 | `PreferenciasVivienda` |
| US-05 / US-06 / US-07 | `VersionLayout` (`EstadoVersion`), `EspacioColocado` |
| US-08 | `Exportacion`, `FormatoExportacion` |
| US-09 | `RevisionTecnica`, `DecisionRevision` |
| US-10 | `Proyecto` (agrega terreno, espacios y preferencias) |

## Regenerar la imagen

```bash
npx @mermaid-js/mermaid-cli -i diagrama_clases_artemus.mmd -o diagrama_clases_artemus.png -s 3 -b white
```
