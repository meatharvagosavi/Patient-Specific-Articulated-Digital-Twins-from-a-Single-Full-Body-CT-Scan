# Patient-Specific Articulated Digital Twins from a Single Full-Body CT 😊

## 📖 About This Project
Most CT-derived models are static: they preserve the body configuration captured at scan time, but cannot represent how the same anatomy would appear after patient repositioning. This limitation is especially important for radiographic imaging, where appearance depends jointly on imaging geometry and patient pose. 

To solve this, we developed this **DIGITAL TWIN** project to create articulated, patient-specific models that can be dynamically repositioned.

---

## 🚀 Project Pipeline & Phases

The repository is structured into sequential phases that take a single full-body CT scan and process it into a fully articulated digital twin capable of synthetic radiography:

*   **Semantic Segmentation:** Initial segmentation of anatomical structures from the CT scans.
*   **Mesh Reconstruction:** Generating 3D meshes from the segmented data.
*   **Phase 1: Patient Anatomical Modeling:** Converting CT data to detailed 3D anatomical models.
*   **Phase 2: SMPL Kinematic Scaffold Optimization:** Aligning and optimizing an SMPL kinematic scaffold to fit the patient's specific anatomy.
*   **Phase 3: Anatomy-Aware Kinematic Binding:** Binding the anatomical meshes to the kinematic scaffold so they move naturally.
*   **Phase 4: Pose Retargeting and Forward Kinematics:** Applying new poses to the digital twin using forward kinematics.
*   **Phase 5: Voxelization and Synthetic Radiography (DRR):** Converting the posed meshes back into a voxel grid to generate Digitally Reconstructed Radiographs (DRRs) under new poses and imaging geometries.

---

## 🛠️ Getting Started

To run the code and reproduce the digital twin pipeline, please refer to the **Environmental Setup** guide included in the repository.

---

## 📚 Presentations & Documentation
For a deeper dive into the methodology, architecture, and results, check out the project presentations:
*   `Digital Twin PPT.pptx`
*   `Major Project Presentation.pdf`
