# Urban Waterlogging Detection: A Challenging Benchmark and Large-Small Model Co-Adapter (ECCV 2024)
Abstract
------
### Urban waterlogging poses a major risk to public safety and infrastructure. Conventional methods using water-level sensors need high-maintenance to hardly achieve full coverage. Recent advances employ surveillance camera imagery and deep learning for detection, yet these struggle amidst scarce data and adverse environmental conditions. In this paper, we establish a challenging Urban Waterlogging Benchmark (UW-Bench) under diverse adverse conditions to advance real-world applications. We propose a Large-Small Model co-adapter paradigm (LSM-adapter), which harnesses the substantial generic segmentation potential of large model and the specific task-directed guidance of small model. Specifically, a Triple-S Prompt Adapter module alongside a Dynamic Prompt Combiner are proposed to generate then merge multiple prompts for mask decoder adaptation. Meanwhile, a Histogram Equalization Adap-ter module is designed to infuse the image specific information for image encoder adaptation. Results and analysis show the challenge and superiority of our developed benchmark and algorithm.
Citation
------
### If you find the paper helpful in your research or work, please cite:
    @ARTICLE{songlsmadapter,
      author={Zhong, Yuanhong and Zhang, Chenxu and Li, Jin},
      journal={IEEE Signal Processing Letters}, 
      title={Image Compressed Sensing Reconstruction via Deep Image Prior With Structure-Texture Decomposition}, 
      year={2023},
      volume={30},
      number={},
      pages={85-89},
      doi={10.1109/LSP.2023.3241847}}
