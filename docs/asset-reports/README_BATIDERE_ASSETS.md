# Batidere Optimized Assets

Generated from `/Users/zafersavaskivilcim/Desktop/batidere_assets`.

## Folders

- `optimized/`: Static optimized GLB props with Draco compression.
- `rigged/`: Rigged character GLB exports.
- `blend/`: Editable Blender source files for rigged characters.

## Notes

- Duplicate source files were skipped:
  - `Meshy_AI_Create_a_game_ready_s_0619131541_texture.glb`
  - `Meshy_AI_Create_a_game_ready_s_0619134312_texture.glb`
- Texture size was capped at 2048 px where the imported images were larger.
- High-poly meshes were decimated for game use.
- `female_npc_rigged.glb` contains a basic humanoid skeleton and a simple idle test animation.
- The rig is a practical first pass. It should be visually checked in Blender before final character animation work.

## Reports

- `batidere_asset_report.csv`: Original asset inspection.
- `batidere_optimization_report.csv`: Optimization and export details.
