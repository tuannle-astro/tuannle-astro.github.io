---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

<!--
HƯỚNG DẪN (không hiện lên web, viết xong thì xóa):
- Đặt file ở _pages/research.md
- Đây là BẢN NHÁP: câu chữ chỉ để giữ chỗ, bạn viết lại kỹ.
- [ngoặc vuông] = chỗ bạn điền. Đặc biệt các con số kết quả: lấy ĐÚNG từ bài báo, không ước lượng.
- "My role": Led / Main contributor / Contributed (ghi phần cụ thể).
- Hình: bỏ vào images/, bỏ comment khối <figure>, ghi nguồn. Bài submitted: hỏi nhóm trước khi đăng hình.
-->

Every black hole mass is the output of a dynamical model: we never see the black hole itself, only how stars and gas move around it. I work on turning spatially resolved kinematics into black hole masses, and on using those masses to understand how black holes and their host galaxies grow together.

**Themes**

1. [Black holes across the mass spectrum](#mass-spectrum)
2. [Measuring black hole masses: methods and benchmarks](#methods)
3. [Black holes and their host galaxies](#coevolution)
4. [Preparing for the Extremely Large Telescope](#elt)
5. [Tools](#tools)

---

## Black holes across the mass spectrum {#mass-spectrum}

Black holes span from ~10<sup>5</sup> M<sub>⊙</sub> in small, bulgeless galaxies to >10<sup>9</sup> M<sub>⊙</sub> in massive ellipticals. Direct dynamical measurements at both ends are scarce, yet they are exactly where models of black hole seeding and growth are tested.

**Key results**

- **IC 342**: M<sub>BH</sub> ≈ 1.95 ± 0.61 × 10<sup>5</sup> M<sub>⊙</sub> from Keck/OSIRIS stellar kinematics, in a galaxy with no classical bulge. *Submitted.* *My role:* Led author.
- **NGC 3862**: M<sub>BH</sub> ≈ 2.40 ± 0.91 × 10<sup>9</sup> M<sub>⊙</sub> from high-resolution CO kinematics. *Submitted.* *My role:* Led author

<!--
<figure>
  <img src="/images/ic342-kinematics.png" alt="Stellar kinematic maps of the IC 342 nucleus">
  <figcaption>[Mô tả 1 câu.] From Le et al. (submitted).</figcaption>
</figure>
-->

---

## Measuring black hole masses: methods and benchmarks {#methods}

Different tracers and models do not always agree. Measuring the same black hole with independent methods (stars vs. gas, different dynamical models) tells us how far we can trust the masses that scaling relations are built on.

**Key results**

- **M81** (JWST/NIRSpec): a robust stellar-dynamical mass, M<sub>BH</sub> ≈ 4.77 × 10<sup>7</sup> M<sub>⊙</sub>. [ApJ 2026](https://doi.org/10.3847/1538-4357/ae64f0). *My role:* Main contributor; 
- **NGC 4258** (JWST/NIRSpec): central dark mass compared with the maser-based mass. [ApJ 2026](https://doi.org/10.3847/1538-4357/ae32f2).
- **NGC 315** (ALMA): a multi-method benchmark of gas-dynamical mass measurements, [kết quả chính]. [ApJ 2026](https://doi.org/10.3847/1538-4357/aea151). 

<!--
<figure>
  <img src="/images/m81-jam.png" alt="JAM model compared with JWST/NIRSpec kinematics of M81">
  <figcaption>[Mô tả.] From Nguyen, Le et al. (2026, ApJ, 1003, 98).</figcaption>
</figure>
-->

---

## Black holes and their host galaxies {#coevolution}

Black hole mass correlates with properties of the host galaxy, such as stellar velocity dispersion and bulge mass. New measurements, especially in unusual hosts, test whether these relations hold everywhere.

**Key results**

- Updating
- Updating

<!-- Một hình tổng hợp kiểu M_BH–σ với các điểm của bạn được tô nổi sẽ rất mạnh ở mục này. -->

---

## Preparing for the Extremely Large Telescope {#elt}

The ELT and its instruments HARMONI and MICADO are not yet operating, so end-to-end mock observations are how we test what they will measure: intermediate-mass black holes in nuclear star clusters nearby, and supermassive black holes out to 1 ≲ <i>z</i> ≲ 2.

**Key results**

- Spatially resolved SMBH masses at 1 ≲ <i>z</i> ≲ 2 with MICADO + HARMONI: [MNRAS 2026](https://doi.org/10.1093/mnras/stag238).
- Effect of the inner surface-brightness profile of nuclear star clusters on IMBH mass recovery: [Universe 2026](https://doi.org/10.3390/universe12060160).
- IMBH mass measurements for a sample of nuclear star clusters with HARMONI: [AJ 2025](https://doi.org/10.3847/1538-3881/ade9ba).

---

## Tools {#tools}

Python · Astropy · NumPy · Matplotlib · pPXF (stellar kinematics) · MGE (surface-brightness models) · JAM (Jeans anisotropic models) · KinMS (gas-disk models) · HSIM (HARMONI) · SimCADO (MICADO) · MCMC (AdaMet, emcee)

## What's next

Updating
