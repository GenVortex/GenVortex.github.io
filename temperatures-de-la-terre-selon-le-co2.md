---
title: "Températures de la Terre selon le CO₂"
layout: math
permalink: /temperatures-de-la-terre-selon-le-co2/
---

<style>
.indent-chap { margin-left: 2em; }
.indent-result { margin-left: 2em; text-align: left; font-weight: bold; display: inline-block; border: 1px solid #eee; padding: 1px 6px; }
.blue-section { color: #1565c0; }
.blue-hr {
  border: none !important;
  border-top: 8px solid #003366 !important;
  height: 0 !important;
  margin: 2em 0 !important;
  opacity: 1 !important;
  background: none !important;
}
</style>

# Températures de la Terre selon le CO₂

<hr class="blue-hr">

## 1. Terre sans atmosphère

*Cas idéal sans aucun gaz à effet de serre. La Terre reçoit uniquement le rayonnement solaire et réémet dans l’infrarouge. La température est déterminée par l’équilibre entre énergie absorbée et énergie réémise.*

<h3 class="blue-section">Modèle physique</h3>
- **Hypothèse** : Corps noir parfait (émissivité = 1)
- **Atmosphère** : Aucune (vide)
- **Calcul** : Bilan radiatif global

<div class="indent-chap">
<h3 class="blue-section">1. Flux solaire absorbé à la surface ($S_{\text{abs}}$)</h3>
$$
S_{\text{abs}} = \frac{S_0}{4} \times (1 - \alpha)
$$
où :
- $S_0 = 1366\ \text{W/m}^2$ (constante solaire)
- $\alpha = 0.30$ (albédo planétaire)
$$
\Rightarrow\ S_{\text{abs}} = 239.75\ \text{W/m}^2
$$

<h3 class="blue-section">2. Bilan énergétique à la surface</h3>
$$
S_{\text{abs}} = \sigma T_e^4
$$

<h3 class="blue-section">3. Température effective</h3>
$$
T_e = \left( \frac{239.75}{5.670367 \times 10^{-8}} \right)^{1/4} = 254.9\ \text{K}
$$
$$
T_e(^\circ\text{C}) = 254.9 - 273.15 = \mathbf{-18.3^\circ\text{C}}
$$

**Résultat** :  
<div class="indent-result">
Température = -18.3 °C
</div>

<h3 class="blue-section">Sources</h3>
- Kopp & Lean, 2011
- Loeb et al., 2018 (CERES)
</div>

<hr class="blue-hr">

## 2. Terre avec atmosphère sans CO₂

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 0 ppm.*

<h3 class="blue-section">Modèle physique</h3>
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds ou rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 0 ppm

<div class="indent-chap">
<h3 class="blue-section">1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)</h3>
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{237.886\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 237.886 W/m²

<h3 class="blue-section">2. Bilan énergétique à la surface</h3>
$$
\boxed{\sigma T_s^4 = S_{\text{abs}} + F_{\text{LW}\downarrow} - (\text{LE} + H)}
$$

| Terme            | Valeur           | Source |
|------------------|------------------|--------|
| **$\sigma T_s^4$** | **298.886 W/m²** | Calculé |
| **$S_{\text{abs}}$** | **161 W/m²**     | Trenberth et al., 2009 |
| **$F_{\text{LW}\downarrow}$** | **237.886 W/m²** | **MODTRAN 3 v1.3** |
| **$\text{LE} + H$** | **100 W/m²**     | Trenberth et al., 2009 |

$$
\sigma T_s^4 = 161 + 237.886 - 100 = \mathbf{298.886\ \text{W/m}^2}
$$

<h3 class="blue-section">3. Température au sol</h3>
$$
T_s = \left( \frac{298.886}{5.670367 \times 10^{-8}} \right)^{1/4} = 278.42\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 278.42 - 273.15 = \mathbf{5.3^\circ\text{C}}
$$

**Résultat** :  
<div class="indent-result">
Température = 5.3 °C
</div>

*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ absent)*

<h3 class="blue-section">Sources</h3>
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)
</div>

<hr class="blue-hr">

## 3. CO₂ à 280 ppm (préindustriel — 1880)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 280 ppm.*

<h3 class="blue-section">Modèle physique</h3>
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds ou rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 280 ppm

<div class="indent-chap">
<h3 class="blue-section">1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)</h3>
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{267.183\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 267.183 W/m²

<h3 class="blue-section">2. Bilan énergétique à la surface</h3>
$$
\boxed{\sigma T_s^4 = S_{\text{abs}} + F_{\text{LW}\downarrow} - (\text{LE} + H)}
$$

| Terme            | Valeur           | Source |
|------------------|------------------|--------|
| **$\sigma T_s^4$** | **328.183 W/m²** | Calculé |
| **$S_{\text{abs}}$** | **161 W/m²**     | Trenberth et al., 2009 |
| **$F_{\text{LW}\downarrow}$** | **267.183 W/m²** | **MODTRAN 3 v1.3** |
| **$\text{LE} + H$** | **100 W/m²**     | Trenberth et al., 2009 |

$$
\sigma T_s^4 = 161 + 267.183 - 100 = \mathbf{328.183\ \text{W/m}^2}
$$

<h3 class="blue-section">3. Température au sol</h3>
$$
T_s = \left( \frac{328.183}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.15\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.15 - 273.15 = \mathbf{15.0^\circ\text{C}}
$$

**Résultat** :  
<div class="indent-result">
Température = 15.0 °C
</div>
*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 280 ppm)*

<h3 class="blue-section">Sources</h3>
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)
</div>

<hr class="blue-hr">

## 4. CO₂ à 420 ppm (2024)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 420 ppm.*

<h3 class="blue-section">Modèle physique</h3>
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds ou rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 420 ppm

<div class="indent-chap">
<h3 class="blue-section">1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)</h3>
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{269.255\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 269.255 W/m²

<h3 class="blue-section">2. Bilan énergétique à la surface</h3>
$$
\boxed{\sigma T_s^4 = S_{\text{abs}} + F_{\text{LW}\downarrow} - (\text{LE} + H)}
$$

| Terme            | Valeur           | Source |
|------------------|------------------|--------|
| **$\sigma T_s^4$** | **330.255 W/m²** | Calculé |
| **$S_{\text{abs}}$** | **161 W/m²**     | Trenberth et al., 2009 |
| **$F_{\text{LW}\downarrow}$** | **269.255 W/m²** | **MODTRAN 3 v1.3** |
| **$\text{LE} + H$** | **100 W/m²**     | Trenberth et al., 2009 |

$$
\sigma T_s^4 = 161 + 269.255 - 100 = \mathbf{330.255\ \text{W/m}^2}
$$

<h3 class="blue-section">3. Température au sol</h3>
$$
T_s = \left( \frac{330.255}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.49\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.49 - 273.15 = \mathbf{15.34^\circ\text{C}}
$$

**Résultat** :  
<div class="indent-result">
Température = 15.34 °C
</div>
*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 420 ppm)*

<h3 class="blue-section">Sources</h3>
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)
</div>

<hr class="blue-hr">

## 5. CO₂ à 560 ppm (doublement de 1880)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 560 ppm.*

<h3 class="blue-section">Modèle physique</h3>
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds ou rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 560 ppm

<div class="indent-chap">
<h3 class="blue-section">1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)</h3>
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{270.731\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 270.731 W/m²

<h3 class="blue-section">2. Bilan énergétique à la surface</h3>
$$
\boxed{\sigma T_s^4 = S_{\text{abs}} + F_{\text{LW}\downarrow} - (\text{LE} + H)}
$$

| Terme            | Valeur           | Source |
|------------------|------------------|--------|
| **$\sigma T_s^4$** | **331.731 W/m²** | Calculé |
| **$S_{\text{abs}}$** | **161 W/m²**     | Trenberth et al., 2009 |
| **$F_{\text{LW}\downarrow}$** | **270.731 W/m²** | **MODTRAN 3 v1.3** |
| **$\text{LE} + H$** | **100 W/m²**     | Trenberth et al., 2009 |

$$
\sigma T_s^4 = 161 + 270.731 - 100 = \mathbf{331.731\ \text{W/m}^2}
$$

<h3 class="blue-section">3. Température au sol</h3>
$$
T_s = \left( \frac{331.731}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.70\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.70 - 273.15 = \mathbf{15.55^\circ\text{C}}
$$

**Résultat** :  
<div class="indent-result">
Température = 15.55 °C
</div>
*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 560 ppm)*

<h3 class="blue-section">Sources</h3>
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)
</div>

<hr class="blue-hr">

## Comparaison des températures selon le CO₂ (MODTRAN)

| Cas | CO₂ (ppm) | Température (°C) |
|-----|-----------|------------------|
| Sans atmosphère | 0 | **-18.3** |
| Avec atmosphère (sans CO₂) | 0 | **5.3** |
| Préindustriel | 280 | **15.0** |
| Actuel (2024) | 420 | **15.34** |
| Doublement (560 ppm) | 560 | **15.55** |

<hr class="blue-hr">

## Et que dit le GIEC ?
<div class="indent-chap">
[Insérez ici votre petit texte explicatif sur le GIEC et les forçages radiatifs.]

<a href="https://www.ipcc.ch/report/ar6/wg1/downloads/report/IPCC_AR6_WGI_FullReport.pdf#page=959" target="_blank">
  <img src="https://www.ipcc.ch/report/ar6/wg1/downloads/report/IPCC_AR6_WGI_FullReport.png" alt="GIEC AR6 Figure 7.8" style="max-width:100%; height:auto;">
</a>

**Faisons les calculs en partant de la valeur de la température de 1880, et regardons ce que produisent ces forçages radiatifs donnés par le GIEC.**
</div>

<hr class="blue-hr">

## 6. Calcul GIEC : 420 ppm et 560 ppm à partir de 1880
<div class="indent-chap">

<h3 class="blue-section">Modèle physique</h3>
- **Température de référence (1880)** : **15.0 °C** = 288.15 K  
- **Forçage radiatif total (1750 → 2019)** : **2.72 W/m²** (GIEC AR6, Figure 7.8, p. 959)  
- **Sensibilité climatique (λ)** : ΔT = λ × ΔF  
  → λ = **0.8 K / (W/m²)** (médiane des modèles CMIP6, GIEC AR6)

<h3 class="blue-section">1. CO₂ à 420 ppm (2024)</h3>
- **Forçage CO₂ seul** : **~1.68 W/m²** (GIEC, p. 959)  
- **ΔT (CO₂ seul)** : 1.68 × 0.8 = **1.34 °C**  
- **Température finale** : 15.0 + 1.34 = **16.34 °C**

<h3 class="blue-section">2. CO₂ à 560 ppm (doublement)</h3>
- **Forçage CO₂ seul** : **~3.71 W/m²** (doublement = +3.71 W/m²)  
- **ΔT (CO₂ seul)** : 3.71 × 0.8 = **2.97 °C**  
- **Température finale** : 15.0 + 2.97 = **17.97 °C**

**Résultat GIEC (forçage + sensibilité)** :

| CO₂ (ppm) | ΔF (W/m²) | ΔT (°C) | T finale (°C) |
|-----------|-----------|---------|---------------|
| 420       | +1.68     | +1.34   | **16.34**     |
| 560       | +3.71     | +2.97   | **17.97**     |

> **Source** : IPCC AR6 WG1, Figure 7.8, p. 959  
> [Lien direct → Page 959](https://www.ipcc.ch/report/ar6/wg1/downloads/report/IPCC_AR6_WGI_Full_Report.pdf#page=959)
>
</div>