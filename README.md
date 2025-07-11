# Scene_Editing_and_Inpainting
# SceneCraft: Intelligent Object Placement and Seamless Scene Integration


## 📍 Overview

**SceneCraft** is a computer vision project developed during the Summer Internship at CCBD & CDSAML Center (June–July 2025). It focuses on creating **photorealistic composite images** by intelligently placing or replacing objects in indoor scenes—preserving **semantic, geometric, and visual coherence**.

---

## 🧠 Problem Statement

Traditional image editing techniques often fail at realistic object placement—producing visible seams, lighting inconsistencies, and unnatural arrangements.

**Objective:**  
Develop an end-to-end pipeline that:
- Understands the scene’s layout and context
- Detects placeable regions
- Performs object insertion/removal
- Seamlessly blends objects using inpainting

This allows applications in:
- Interior design
- Augmented reality
- Creative content generation

---

## 🧪 Key Technologies & Models

- **Scene Classification**
- **Semantic & Panoptic Segmentation**
- **Depth Estimation**
- **Object Detection & Removal**
- **User-Guided Object Placement**
- **Depth-Aware Scaling**
- **Generative Inpainting**

---

## 🔁 Pipeline Flow

```mermaid
graph TD
A[Input Image] --> B[Scene Classification]
B --> C[Semantic/Panoptic Segmentation]
C --> D[Generate Placeable Region Mask]
D --> E[Depth Estimation]
A --> F[Optional Object Removal]
F --> G[User Selects Object Placement]
G --> H[Object Segmentation & Scaling]
