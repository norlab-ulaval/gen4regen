# Gen4Regen

**Leveraging Image Generators to Address Data Scarcity:
The Gen4Regen Dataset for Forest Regeneration Mapping**

Sustainable forest management relies on precise species composition mapping, yet traditional ground surveys are labour-intensive and geographically constrained. While Uncrewed Aerial Vehicles (UAVs) offer scalable data collection, the transition to deep learning-based interpretation is bottlenecked by the severe scarcity of expert-annotated imagery, particularly in complex, visually heterogeneous regeneration zones. This paper addresses the dual challenges of data scarcity and extreme class imbalance in the fine-grained semantic segmentation of plants by providing a scalable framework that reduces reliance on manual photo-interpretation for fine spatial resolution, millimetre-level aerial imagery. Importantly, we leverage the large-scale Nano Banana Pro model to simultaneously generate high-fidelity images and their corresponding pixel-aligned semantic masks from prompts. We introduce WilDReF-Q-V2, an expansion of a natural forest dataset with 13 977 new unlabelled and 50 hand-labelled *real* images, as well as the Gen4Regen dataset, featuring 2101 pairs of *synthetic* images and semantic masks. Our methodology integrates real-world data with AI-generated images, addressing both data scarcity and class imbalance in forest regeneration mapping. We evaluate the orthogonality of manual labels, automated pseudo-labels, and synthetic data using the Mask2Former, DINOv2, and DINOv3 architectures under spatially distant cross-validation folds, and highlight that AI-generated data is highly complementary to real-world pseudo-labels, with unified training yielding an F1 score improvement of over 13 %pt compared to purely supervised baselines. Furthermore, we demonstrate that even small quantities of prompt-generated data significantly improve performance for underrepresented classes, some of which see per-class F1 score gains of over 30 %pt. We conclude that large-scale vision models show strong potential as agile data generators to effectively bootstrap perception tasks for niche AI domains where expert labels are scarce or unavailable. This work demonstrates a viable path toward bypassing seasonal data collection constraints, suggesting that as generative models continue to mature, practitioners may develop specialized ecological monitoring systems with limited manual effort. Our UAV image datasets, source code, and models will be available at <https://norlab-ulaval.github.io/gen4regen>.

## Website

The project website lives at [`index.html`](index.html) and is hosted via GitHub Pages.

To view it locally, open `index.html` in any modern browser or serve the root directory:

```bash
python3 -m http.server 8080
# then open http://localhost:8080
```

## Contact

Northern Robotics Laboratory, Université Laval, Québec, QC, G1V 0A6, Canada  
gabriel.jeanson@norlab.ulaval.ca
