# GodotPhysicsExtended

A modular collection of C++ GDExtension physics nodes for Godot 4, adding specialized physics behaviors missing from Godot's built-in node set.

<!-- ![Image](https://github.com/user-attachments/assets/012780b7-403e-4426-b8b7-e1792f3fcb8d) -->

---

## Nodes

### SpringBody2D
> Applies a customizable spring effect to colliding `RigidBody2D` nodes using impulse-based physics.

| Property | Description |
|---|---|
| `Release Magnitude` | Multiplier applied to the release force |
| `Max Force` | Upper limit on the release force |
| `Min Buildup` | Minimum velocity buildup before release triggers |
| `Threshold` | Minimum dot product of velocity against the wall to trigger release |
| `Growth Mult` | Multiplier on the rate of buildup growth |
| `Normal Weight` | Weighting between surface normal and RigidBody2D entry direction |

**Requirements:** Godot 4.3+ · Windows x86_64 (other platforms require building from source) · `CollisionPolygon2D` as a direct child

📦 [View Repository](https://github.com/ProudPurple/SpringBody2D) · [Godot Asset Library](https://godotengine.org/asset-library/asset/4911)

---

## Installation

Each node is available as a standalone plugin or as part of this collection.

### Install All (Recommended)
1. Download the latest release from [Releases](https://github.com/ProudPurple/GodotPhysicsExtended/releases)
2. Copy the `addons/` folder into your project root
3. Go to **Project → Project Settings → Plugins**
4. Enable whichever nodes you need

### Install Individual Nodes
See each node's repository for standalone installation instructions.

---

## Roadmap

- [x] SpringBody2D — spring collision response
- [ ] GravityBody2D — radial gravitational field (Mario Galaxy-style attraction)
- [ ] WaterField2D — water resistance and buoyancy simulation

---

## Building From Source

Each node uses the [Godot C++ GDExtension](https://github.com/godotengine/godot-cpp) bindings.

```bash
# Clone with submodules
git clone --recurse-submodules https://github.com/ProudPurple/GodotPhysicsExtended.git

# Enter a node directory and build
cd SpringBody2D
scons
```

Refer to each submodule's README for platform-specific build instructions.

---

## License

All nodes in this collection are released under the [MIT License](LICENSE).

---

*Made with C++ and Godot 4 by [Anderson Kimball](https://github.com/ProudPurple)*
