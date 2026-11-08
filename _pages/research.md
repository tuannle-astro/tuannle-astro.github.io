---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% include base_path %}

{% comment %}
GHI CHÚ (Liquid comment: KHÔNG xuất ra HTML, kể cả khi View Source)
- Mỗi mục: Ý tưởng -> Bức tranh chung (trích bài của nhóm) -> Phần của tôi -> Hình.
- Các đoạn "ý tưởng" dưới đây là NHÁP để giữ chỗ, bạn viết lại theo giọng của mình.
- "I" = việc bạn trực tiếp làm; "we / the group" = việc của nhóm.
- Facilities: ảnh và chú thích sửa trong _data/facilities.yml.
{% endcomment %}

We never see a black hole directly in these measurements. What we see is how stars and gas move around it. My work turns spatially resolved kinematics into black hole masses, using two kinds of tracers (stars and cold molecular gas) and, looking ahead, simulated observations for the next generation of telescopes.

- [Stellar dynamics](#stellar)
- [Molecular-gas dynamics](#gas)
- [Simulations for the Extremely Large Telescope](#elt)
- [Facilities](#facilities)

---

## Stellar dynamics {#stellar}

**The idea.** Stars are present in every galaxy, so they are the most general tracer of the central gravity. Close to the black hole, the stars move faster and their orbits change in ways we can measure from the shapes of their absorption lines. To turn those motions into a mass, we need three things: spectra that resolve the black hole's sphere of influence, a model of how much mass the stars themselves contribute, and a dynamical model that links the two.

**The bigger picture.** In the group we apply this approach with JWST/NIRSpec and Keck/OSIRIS adaptive optics to nearby galaxies. One example is NGC 4258, where the stellar-dynamical mass can be checked against the precise maser mass ([Nguyen et al. 2026](https://doi.org/10.3847/1538-4357/ae32f2)). Others include NGC 4736 (Ngo et al., submitted), NGC 5055 (Ho et al., revised) and M87 (Ngo et al., in prep.).

**My part.** For M81, I separated the non-thermal glow of the active nucleus from the starlight in the JWST/NIRSpec data. This made it possible to build an accurate stellar mass model and extract unbiased stellar kinematics. The result is M<sub>BH</sub> = (4.77 ± 0.37) × 10<sup>7</sup> M<sub>⊙</sub> ([Nguyen, Le et al. 2026](https://doi.org/10.3847/1538-4357/ae64f0)). I led the measurement in IC 342, a bulgeless spiral hidden behind the dust of the Milky Way. There, Keck/OSIRIS K-band spectroscopy reveals a black hole of ~2 × 10<sup>5</sup> M<sub>⊙</sub>, but only once the mass-to-light gradient of the young nuclear star cluster is taken into account (Le et al., submitted). I am now extending this approach to a second dust-obscured nucleus, Maffei 2.

{% comment %}
<figure>
  <img src="{{ base_path }}/images/research/m81.png" alt="">
  <figcaption>[Mô tả 1 câu]. From Nguyen, Le et al. (2026, ApJ 1003, 98).</figcaption>
</figure>
{% endcomment %}

---

## Molecular-gas dynamics {#gas}

**The idea.** Some galaxies, often massive early-type galaxies, host a thin, cold disk of molecular gas in their centres. Gas in such a disk moves on nearly circular orbits, so its rotation curve traces the enclosed mass more directly than the random motions of stars. ALMA observations of carbon monoxide (CO) lines resolve these disks down to the black hole's sphere of influence. We then forward-model the full data cube.

**The bigger picture.** Because the method relies on fewer assumptions about orbits, it is a valuable cross-check. In NGC 315 the group compared several gas-dynamical methods on the same ALMA data, as a benchmark for how robust these masses are ([Nguyen et al. 2026](https://doi.org/10.3847/1538-4357/aea151)). In NGC 4061 the same technique gives dynamical evidence for a billion-solar-mass black hole ([Nguyen et al. 2026](https://doi.org/10.3847/1538-4357/ae771c)).

**My part.** I led the first dynamical black hole mass measurement in the radio galaxy NGC 3862 (3C 264). I modelled the CO(2–1) kinematics of its circumnuclear gas ring with KinMS. To build a clean stellar mass model from HST imaging, I masked the synchrotron jet and the active nucleus and corrected for dust using a colour map. The result is M<sub>BH</sub> ≈ 2 × 10<sup>9</sup> M<sub>⊙</sub> (Le et al., revised).

{% comment %}
<figure>
  <img src="{{ base_path }}/images/research/ngc3862.png" alt="">
  <figcaption>[Mô tả]. Bài đang revised: hỏi nhóm trước khi đăng hình.</figcaption>
</figure>
{% endcomment %}

---

## Simulations for the Extremely Large Telescope {#elt}

**The idea.** Today, dynamical black hole masses are limited to fairly nearby galaxies, because the sphere of influence quickly becomes too small to resolve. The 39-m Extremely Large Telescope, with its integral-field spectrograph HARMONI and imager MICADO, will change that. Since the ELT is not yet operating, we test what it will be able to measure with end-to-end mock observations: we simulate the data and then run the same dynamical modelling on them as on real observations.

**The bigger picture.** The group's simulations show that HARMONI can recover intermediate-mass black holes in nuclear star clusters of nearby galaxies ([Nguyen et al. 2025](https://doi.org/10.3847/1538-3881/ade9ba)). They also quantify how the inner light profile of the cluster affects that recovery ([Le, T. Q. T. et al. 2026](https://doi.org/10.3390/universe12060160)). Combining MICADO and HARMONI, spatially resolved supermassive black hole masses can be measured out to 1 ≲ *z* ≲ 2 ([Nguyen et al. 2026](https://doi.org/10.1093/mnras/stag238)).

**My part.** This is where I started research, in 2022. I ran mock HARMONI observations and MCMC dynamical fits to test the recovery of IMBH masses in nuclear star clusters. I also explored whether IMBHs in extragalactic globular clusters would be detectable, and presented this work at the SAGI workshops in Quy Nhon in 2022 and 2023.

---

## Facilities {#facilities}

Data I have worked with, including space-base, ground-base, and in simulation.

<div class="facility-grid">
{% for f in site.data.facilities %}
  <div class="facility-card">
    <div class="facility-card__img">
      {% if f.image and f.image != "" %}
      <img src="{{ base_path }}/images/facilities/{{ f.image }}" alt="{{ f.name }}" loading="lazy">
      {% else %}
      <span>{{ f.short | default: f.name }}</span>
      {% endif %}
    </div>
    <div class="facility-card__caption">
      <p class="facility-card__name">{{ f.name }}{% if f.short and f.short != "" %} ({{ f.short }}){% endif %}</p>
      {% if f.instrument and f.instrument != "" %}<p class="facility-card__inst">{{ f.instrument }}</p>{% endif %}
      {% if f.credit and f.credit != "" %}<p class="facility-card__credit">Image: {{ f.credit }}</p>{% endif %}
    </div>
  </div>
{% endfor %}
</div>

See [Publications](/publications/) for the full list of papers.
