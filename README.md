# Stele-12K Dataset & SteleGen Project

## Project Profile
This repository is used for presentations on the Stele-12K dataset and the SteleGen project. Here, we have uploaded sample images within the Stele-12K dataset, along with their corresponding text descriptions.

## SteleGen
The salvage restoration of ancient stele images has long confronted severe challenges posed by large-scale physical spalling and topological fragmentation. When addressing such extreme degradation, existing visual diffusion models and controllable generation paradigms often suffer from severe stroke artifacts and modern typography hallucinations due to the absence of explicit linguistic knowledge constraints. Furthermore, forcibly injecting external conditions midway through diffusion denoising triggers irreversible structural and semantic artifacts.

To overcome these challenges, we propose **SteleGen**, a framework for Cross-Modal RAG Semantic Inference and Skeleton Context-Aware Diffusion for Ancient Stele Image Restoration. First, we introduce a Stele-OCR feature extraction network equipped with a Residual Dual-Stream Macro-Topological Adapter (DS-MTA) to robustly extract fragmented visual cues and truncate extreme visual blind zones into masks. Besides, we construct a dual-engine semantic inference mechanism cascading SikuRoBERTa and Retrieval-Augmented Generation (RAG) to achieve hallucination-free, high-order inference within extreme blind zones. Significantly, we employ a dynamic skeleton renderer and propose a stage-decoupled mechanism with a zero-initialization residual injection (Zero-Init Residual Injection) strategy to smoothly couple discrete skeleton constraints into the pre-trained diffusion network without destroying the native data manifold.

More crucially, we construct the **Stele-12K** dataset for robust training via a dynamic mask superposition strategy. We also extensively evaluate our method on the real-world degraded test set from the Xi'an Beilin Museum.

Experimental results demonstrate that the SteleGen model achieves overwhelmingly state-of-the-art (SOTA) performance in both pixel fidelity and character-level topological reconstruction. Additionally, on the Noah-Wukong generalization test set, our model exhibits exceptional zero-shot generalization capabilities on unseen, severely damaged handwritten texts and abstract graphics.

## Code
We will upload the training as well as the test code and the full dataset at an appropriate time!
