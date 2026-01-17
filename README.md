# pentagon-tiling
不規則な五角形が平面を隙間なく敷き詰められるかどうかを、計算機的に検証するためのリポジトリです。 五角形の辺の長さと内角を入力として、同一形状の回転・平行移動のみを用いた配置を試み、平面充填が可能かを判定します。 成功した場合は、実際の充填構造をSVGやPDFなどのベクター形式で出力し、正確な図として可視化します。 理論的分類や証明を目的とせず、構成的・実験的な検証と再現可能な可視化に重点を置いています。
Irregular Pentagon Plane Tiling

This repository provides a computational method to test whether a given irregular pentagon can tile the plane using only translations and rotations of the same shape.

The project focuses on explicit construction and visualization, rather than theoretical classification or proofs.


---

What this project does (very simply)

Take one pentagon (defined by side lengths and interior angles)

Copy it many times

Rotate and shift the copies

Check whether they can fill the plane without gaps or overlaps

If successful, draw the tiling exactly (SVG / PDF)



---

Input

A single irregular pentagon defined by:

Five side lengths

Five interior angles


The pentagon is treated as a rigid shape.


---

Output

The algorithm produces:

A binary decision: tileable / not tileable

An explicit geometric tiling when successful

Vector graphics output suitable for inspection and printing



---

Method overview

1. Place an initial pentagon in the plane


2. Generate copies using translations and rotations


3. Align edges to form local matches


4. Extend the configuration outward


5. Detect either:

a consistent repeating pattern, or

failure due to gaps, overlaps, or inconsistency




This is a constructive test, not a formal impossibility proof.


---

Visualization

When a valid tiling is found, the configuration is exported as:

SVG (for exact geometry)

PDF (for print-quality figures)


These outputs allow precise verification of the tiling structure.


---

Scope and limitations

The method does not enumerate all possible tilings

Failure does not imply mathematical impossibility

Success provides direct geometric evidence of tileability


The goal is exploratory and practical rather than exhaustive.


---

Relation to existing work

Plane tilings by convex pentagons are a classical topic in geometry.

This project does not propose a new theoretical classification. Instead, it offers a computational and reproducible approach to testing individual shapes.


---

Reproducibility

All results are reproducible from the provided code and input parameters. The project is designed so that any generated tiling can be independently verified.


---

Use of computational tools

Computational tools were used to assist in algorithm development and visualization. All design decisions and final results were made by the author.


---

License

MIT License (or specify as appropriate)


---

Citation

If you use this work, please cite the accompanying preprint.


---

Status

This repository accompanies an arXiv preprint and is intended for research, education, and experimentation.
