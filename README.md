# amongus-map-mesh

This repository contains map meshes for creating your own Among Us-inspired game. The meshes are based on The Skeld map from the popular game Among Us.

## 📍 Map Images

### 1. The Skeld - Default Map
![Default Map](https://i.ibb.co/PYWF6sp/The-Skeld-map-map-default.png)
- Original layout of The Skeld map
- Reference for map design and room placement

### 2. The Skeld - 50 Combined Mesh
![Combined Mesh](https://i.ibb.co/xFyNsGP/The-Skeld-map-mesh-50-combined.png)
- 50-node mesh overlay
- Combines walkable areas and vents
- Useful for pathfinding algorithms

### 3. The Skeld - 50 Adapted Mesh
![Adapted Mesh](https://i.ibb.co/BPvsjTX/The-Skeld-map-mesh-50-adapted.png)
- Adapted 50-node mesh
- More precise layout fitting
- Enhanced pathfinding accuracy

### 4. The Skeld - 50 Mesh
![50 Mesh](https://i.ibb.co/MsLzQfC/The-Skeld-map-mesh-50.png)
- Basic 50-node mesh
- Simple pathfinding implementation
- Movement system foundation

### 5. The Skeld - 100 Mesh
![100 Mesh](https://i.ibb.co/dptJ12z/The-Skeld-map-mesh-100.png)
- Detailed 100-node mesh
- Fine-grained pathfinding
- Advanced AI behavior support

### 6. Map Mesh Overview
![Mesh Overview]()
- Comparative mesh visualization
- Different density representations

## 🚀 Usage

```csharp
// Example Unity/C# implementation
public class MapMeshController : MonoBehaviour 
{
    public NavMeshAgent agent;
    public float[] meshDensities = {50, 100};

    void SetupPathfinding(int meshIndex) 
    {
        // Load appropriate mesh based on density
        NavMesh.BuildNavMesh(meshDensities[meshIndex]);
    }
}
