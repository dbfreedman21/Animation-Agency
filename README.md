# Animation-Agency
Golden Sun

1. Problem / Goal

Create a small, playable animation prototype that captures the look and feel of Golden Sun using pixel sprites, without building a full game.

2. Why this matters

You need a controlled, scoped project that builds real animation skills. A Golden Sun prototype trains you in pixel animation, sprite workflow, scene composition, and Godot integration. It becomes portfolio evidence and a proving ground before larger game ambitions.

3. First Principles
Ground truths

You do not have programming or game-dev experience.

Pixel animations require frame-based iteration and a strict workflow.

Godot is accessible; Golden Sun’s original animations were tile based with 2D sprites.

A remake is impossible. A micro-prototype is doable.

Constraints

You cannot recreate Golden Sun’s full battle or world engine.

You cannot produce high-volume assets.

You must re-create only tiny slices: one character, one short animation, one simple scene.

Non-negotiables

Sprite resolution stays consistent with original assets.

All animations must export cleanly to Godot.

The scope must remain a micro-scene, not a game.

4. Minimal Viable Animation System
Core promise

A single Godot scene with:

One Golden Sun–style character sprite

A short idle or walk animation

A 5–10 second looping in-engine scene

Inputs

1 sprite sheet of Isaac’s idle or walk animation

1 background tile set (very small)

Minimal Godot scene

Free tools only

Outputs

demo.mp4 of the animation running

tiny playable Godot build

documentation of animation pipeline

5. Primitive Steps (Senku-style)

Every step is doable with your current ability.

Step 0 Baseline setup

Create repo and folder scaffold

Install Godot and Aseprite (or free equivalent)

Step 1 Single-frame concept

Recreate one Isaac frame at correct pixel resolution

Export PNG

Commit

Step 2 Primitive motion

Build a 3–5 frame idle or walk cycle

Export as sprite sheet

Step 3 Animation polish

Expand to 6–8 frames

Improve timing

Export clean sheet

Step 4 Background stub

Make a simple terrain tile (grass or platform)

Tile it into a tiny background

Step 5 Engine integration

Import sprite sheet into Godot

Add AnimationPlayer and Sprite2D

Load background

Play idle animation on loop

Step 6 Basic interaction

Add a single input: walk left or right

Character moves with a single animation change

Step 7 Export

Export demo.mp4 and tiny Windows/Web build

Stop here. Prototype is done.

6. Assumptions

People can recognize the style from the sprite resolution.
Test: show to 3 people, ask if they perceive the Golden Sun inspiration.

You can manage 6–8 frame animations without burnout.
Test: track actual time spent on frame creation.

Godot handling sprite sheets is manageable for a beginner.
Test: import a 3-frame sheet without breaking.

7. Risks
Technical

Incorrect sprite slicing in Godot

Misaligned pivots causing jittery animation

Creative

Frame inconsistencies break Golden Sun’s look

Palette mismatch kills the vibe

Execution

Overscoping is the main threat

Trying to recreate too much too soon

8. Evidence Log

Examples:

2025-11-27: Recreated first silhouette.

2025-11-28: Idle animation (3 frames) recognized by 2/3 testers.

9. Cash-Flow Possibilities

Not the point here, but:

Portfolio piece for future animation commissions

Demonstration asset for pitching pixel-art animation services

10. Deliverables for V1

sprite_sheet_idle.png

background_tiles.png

isaac_idle_demo.tscn

demo.mp4

README.md (this file)

one playable build

11. One Next Tiny Task

Create one 64×64 Isaac idle keyframe and commit it.

Directory Scaffold
/assets
  /sprites
    isaac_idle_keyframe.png
    isaac_idle_sheet.png
  /background
    grass_tile.png
    background_mockup.png
  /reference
    golden_sun_original_sprites/
    palette_samples.png
/src
  /godot_project
    project.godot
    /scenes
      isaac_idle_demo.tscn
    /scripts
      player_controller.gd
/tests
  /playtest_notes
/docs
  README.md
  asset_pipeline.md
  export_settings.md
/builds
  demo_web/
  demo_windows/
