# 🌲 First-Person Unity Landscape Sandbox

An interactive 3D game environment built in Unity featuring a fully controllable 1st-person player capsule and dynamic gameplay settings.

## ✨ Features

* 🗺️ **3D Terrain Landscape**: Explore a dynamic Unity terrain with varied topography and environmental structures.
* 🧍 **Capsule First-Person Controller**: Smooth, physics-based movement using a capsule collider to represent the player body.
* ⚙️ **Real-Time Settings Panel**: Adjust player stats and game parameters on the fly via UI sliders.
* 🎥 **Dynamic Camera Look**: Smooth first-person perspective with adjustable look sensitivity.

## 🎮 Player Controls

Use the following default inputs to navigate the world:

* **W, A, S, D**: Move Forward, Left, Backward, Right
* **Left Shift**: Sprint / Run
* **Spacebar**: Jump
* **Mouse Move**: Look / Rotate Camera
* **Escape (ESC)**: Unlock mouse cursor / Open Settings

## 🎛️ Controllable Settings

Access the in-game UI panel to adjust these variables in real-time:

| Setting | Default | Description |
| :--- | :--- | :--- |
| **Walk Speed** | `5.0` | Adjusts the normal walking pace. |
| **Sprint Speed** | `8.0` | Adjusts running speed when holding Shift. |
| **Jump Force** | `5.0` | Controls the vertical height of player jumps. |
| **Gravity** | `-9.81` | Alters the downward physics pull on the capsule. |
| **Mouse Sensitivity** | `2.0` | Changes the camera rotation response to mouse movement. |

## 🛠️ Built With

* **Game Engine**: Unity 2022.3 LTS (or newer)
* **Physics**: Unity RigidBody & Capsule Collider
* **Input**: Traditional Input Manager / New Input System

## 🚀 Getting Started

### Prerequisites
* Unity Hub installed.
* Unity Editor version `2022.3 LTS` or higher.

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com
   ```
2. Open **Unity Hub**.
3. Click **Add** -> **Add project from disk**.
4. Select the cloned repository folder.
5. Open the project and navigate to `Assets/Scenes/MainWorld.unity`.
6. Press the **Play** button at the top of the editor.

## 📝 Setup Guide (How it Works)

1. **The Player**: A standard 3D Capsule GameObject with a `Rigidbody` (Frozen X/Z rotations) and a `Capsule Collider`.
2. **The Camera**: Placed inside the Capsule near the top to act as the first-person eyes.
3. **The Settings Canvas**: A Screen-Space UI Canvas containing Unity Sliders bound to the player script variables via `OnValueChanged` events.
