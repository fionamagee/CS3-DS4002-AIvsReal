# REFERENCES

The following resources informed the design and execution of this case study. All citations are in IEEE documentation style.

---

[1] S. Guevara, A. L. Sandoval Orozco, and L. J. García Villalba, "A survey on deep-learning-based techniques for detecting AI-generated synthetic images," *Engineering Proceedings*, vol. 123, no. 1, p. 32, 2026, doi: 10.3390/engproc2026123032.

> This survey paper organizes existing AI-image detection methods into CNN-based and transformer-based families and explains why each architecture catches different kinds of artifacts. It informed the decision to compare a CNN against a Vision Transformer rather than relying on a single model type.

---

[2] T. Say, M. Alkan, and A. Kocak, "Advancing GAN deepfake detection: Mixed datasets and comprehensive artifact analysis," *Applied Sciences*, vol. 15, no. 2, p. 923, 2025, doi: 10.3390/app15020923.

> This paper demonstrates that ensembling multiple architectures consistently outperforms individual models on deepfake detection tasks. It directly motivated the inclusion of a logistic-regression ensemble combining EfficientNet and ViT predictions in the final pipeline.

---

[3] P. Morgan, "New research suggests folks are relying on outdated visual cues to identify AI-generated faces," *PC Gamer*, 2025. [Online]. Available: https://www.pcgamer.com/software/ai/new-research-suggests-folks-are-relying-on-outdated-visual-cues-to-identify-ai-generated-faces-but-i-did-get-14-20-on-the-test/

> An accessible explainer on the UNSW Sydney study showing that even "super-recognizers" cannot reliably distinguish modern AI-generated faces from real ones. It provided the framing for why automated detection is necessary and helped shape the hook document's narrative.

---

[4] Y. Wang, L. Linyan, W. Wenjuan, et al., "AI-generated artwork detection using self-distilled transformers with global–local feature learning and Grad-CAM interpretability," *Scientific Reports*, vol. 16, p. 497, 2026, doi: 10.1038/s41598-025-29229-2.

> This paper supports the use of Vision Transformers for AI-image detection by showing that self-attention mechanisms capture global compositional cues that CNNs miss. It informed the choice of ViT-B/16 as the transformer architecture in this project.

---

[5] T. Roca, A. Cintron Roman, J. Torres Vega, M. Duarte, P. Wang, K. White, A. Misra, and J. Lavista Ferres, "How good are humans at detecting AI-generated images? Learnings from an experiment," arXiv preprint arXiv:2507.18640, May 2025. [Online]. Available: https://arxiv.org/abs/2507.18640

> The Microsoft study that established the ~62% human-detection baseline. This number is the floor that any successful classifier must exceed and is referenced throughout the hook and rubric as the project's primary success metric.

---

[6] R. Roy, N. Imanpour, A. Aziz, S. Bajpai, G. Singh, S. Biswas, K. Wanaskar, P. Patwa, S. Ghosh, S. Dixit, N. R. Pal, V. Rawte, R. Garimella, G. Jena, V. Sharma, V. Jain, A. Chadha, A. N. Reganti, and A. Das, "A Comprehensive Dataset for Human vs. AI Generated Image Detection," arXiv preprint arXiv:2601.00553, 2026. [Online]. Available: https://arxiv.org/abs/2601.00553

> The paper introducing the Defactify Image Dataset used in this case study. It documents the captioning method, the five generative models (SD2.1, SDXL, SD3, DALL·E 3, Midjourney), and the caption-family structure that allows for controlled real-vs-AI comparison.

> Direct dataset link: https://huggingface.co/datasets/Rajarshi-Roy-research/Defactify_Image_Dataset
