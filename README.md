

https://github.com/user-attachments/assets/c2c10005-153c-4ab7-969a-017a52165b6e


InterAct retarget
=================

This is version of the [InterAct dataset](https://hku-cg.github.io/interact/) exported in both fbx and bvh format with a different skinned character applied.

The skinned character mesh is available in `Geno.fbx` and is free for non-commercial research use.

This dataset is compatible with:

* [lafan1-resolved](https://github.com/orangeduck/lafan1-resolved)
* [zeroeggs-retarget](https://github.com/orangeduck/zeroeggs-retarget)
* [motorica-retarget](https://github.com/orangeduck/motorica-retarget)
* [100style-retarget](https://github.com/orangeduck/100style-retarget)

For an example raylib application that can visualize this data on a skinned character check out the [GenoView](https://github.com/orangeduck/GenoView) or [GenoViewPython](https://github.com/orangeduck/GenoViewPython) repo.

Single vs Multi
===============

There are two versions of the retargeted data provided - _single_ and _multi_.

In the _single_ version each character is treated individually and each clip is retargetd and exported independently. This produces the best retargeting quality because it effectively scales the source character to better fit the Geno character, but it means that clips from the same interaction no longer fit together since the root translation of each character is not preserved.

In the _multi_ version characters are retargeted without adjusting their scale. This means their interactions are properly preserved with respect to each other, but that there might be some retargeting issues introduced (such as overly bent, or hyper-extended arms or legs) for characters who's size differs greatly from the Geno character.

Download
========

* [BVH Single Data](https://theorangeduck.com/media/uploads/Geno/interact-retarget/bvh_single.zip)
* [BVH Multi Data](https://theorangeduck.com/media/uploads/Geno/interact-retarget/bvh_single.zip)
* [FBX Single Data](https://theorangeduck.com/media/uploads/Geno/interact-retarget/fbx_single.zip)
* [FBX Multi Data](https://theorangeduck.com/media/uploads/Geno/interact-retarget/fbx_single.zip)

License
=======

This version of the data is licensed under the [same terms](https://hku-cg.github.io/interact/) as the original dataset.

This means this data is NOT licensed for commercial use.

Citations
=========

When mentioning this database in an academic paper or other publication please cite the following publication as requested by the original dataset:

```
@article{ho2025interact,
  title={InterAct: A Large-Scale Dataset of Dynamic, Expressive and Interactive Activities between Two People in Daily Scenarios},
  author={Ho, Leo and Huang, Yinghao and Qin, Dafei and Shi, Mingyi and Tse, Wangpok and Liu, Wei and Yamagishi, Junichi and Komura, Taku},
  journal={Proceedings of the ACM on Computer Graphics and Interactive Techniques},
  volume={8},
  number={4},
  pages={1--27},
  year={2025},
  publisher={ACM New York, NY}
  doi={10.1145/3747871}
}
```


