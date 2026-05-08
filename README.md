# Gen4Regen

**Leveraging Image Generators to Address Training Data Scarcity:
The Gen4Regen Dataset for Forest Regeneration Mapping**

Sustainable forest management relies on precise species composition mapping, yet traditional ground surveys are labour-intensive and geographically constrained. While Uncrewed Aerial Vehicles (UAVs) offer scalable data collection, the transition to deep learning-based interpretation is bottlenecked by the severe scarcity of expert-annotated imagery, particularly in complex, visually heterogeneous regeneration zones. This paper addresses the dual challenges of data scarcity and extreme class imbalance in the semantic segmentation of fine-grained forest regeneration species by providing a scalable framework that reduces reliance on manual photo-interpretation for high-resolution, millimetre-level aerial imagery. Importantly, we leverage the large-scale vision-language Nano Banana Pro model to simultaneously generate high-fidelity images and their corresponding pixel-aligned semantic masks from prompts. We introduce WilDReF-Q-V2, an expansion of a natural forest dataset with 13 977 new unlabelled and 50 labelled real images, as well as the Gen4Regen dataset, featuring 2101 pairs of synthetic images and semantic masks. Our methodology integrates real-world data with AI-generated images, highlighting that AI-generated data is highly complementary to real-world data, with unified training yielding an F1 score improvement of over 15 %pt compared to purely supervised baselines. Furthermore, we demonstrate that even small quantities of prompt-generated data significantly improve performance for underrepresented species, some of which saw per-species F1 score gains of up to 30 %pt. We conclude that vision-language models can serve as agile data generators, effectively bootstrapping perception tasks for niche AI domains where expert labels are scarce or unavailable.

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
