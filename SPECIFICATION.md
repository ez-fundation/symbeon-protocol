# Sovereign Codex: Technical Specification v0.2.0

## 1. The Symbeon Intent Schema
The core of the protocol is the **Isomorphic Intent**. This JSON structure serves as the contract between the Archaeologist (AION) and the Generator (EZ-Studios).

### 1.1 structure
```json
{
    "id": "intent_<uuid>",
    "categoria": "Mapa | Actor | Item | Physics | VFX | UI",
    "descricaoNatural": "Natural language synthesis of the findings",
    "parametros": {
        "source_binary": "filename",
        "source_offset": "hex_offset",
        "entropy": "float",
        "estetica": "Dynamic Aesthetic Label",
        "tags": ["keyword1", "keyword2"]
    },
    "metadados": {
        "autorId": "AION_ENGINE",
        "seed": "extraction_seed",
        "hashGeracao": "unique_hash"
    }
}
```

## 2. Isomorphic Mapping Principles
1.  **Conservation of Entropy:** The complexity of the output world must be proportional to the entropy of the source binary.
2.  **Aesthetic Continuity:** Use pattern-scoring to derive visual themes via $\Psi(\text{Geometry}, \text{Estetica})$.
3.  **Algorithmic Injection:** Pure logic from the **Eon-Chess** layer is injected into the generated entities.

## 3. The Generation Pipeline (EZ-Studios HGF)
Once the Intent is received, it is processed by the **Holistic Generation Framework (HGF)**:

### 3.1 Actor Engine (Anatomic WFC)
- Translates `Actor` category intents into physical entities.
- Uses **DNA seeds** derived from the original binary entropy.

### 3.2 Item Factory (Stat-BSP)
- Partitions the "Power Budget" of extracted items based on their original complexity.

### 3.3 Experience Layer
- Maps the "Game Intention" (extracted strings/logic) into quest and event graphs.

## 4. Adaptation & Deployment (Engine Matrix)
The final stage of the protocol is the deployment of the generated blueprint into native engines:

| Stage | Roblox | Unity | Web (Three.js) |
| :--- | :--- | :--- | :--- |
| **Execution** | Luau GETIMPORT | C# Job System | WebAssembly |
| **Instancing** | task.spawn/Batch | Burst Compiler | InstancedMesh |

## 5. Integration Interface
AION exports to `<ROOT>/AION_REPORTS/aion_intent.json`.
EZ-Studios monitors this path to trigger the **Seed-to-World** pipeline.

---
*EZ-Fundation Technical Standards - Sovereign Codex v0.2.0*
