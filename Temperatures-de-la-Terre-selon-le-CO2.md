---
title: "Températures de la Terre selon le CO₂"
layout: default
permalink: /Temperatures-de-la-Terre-selon-le-CO2/
---
# Températures de la Terre selon le CO₂

---
## 1. Terre sans atmosphère

*Cas idéal sans aucun gaz à effet de serre. La Terre reçoit uniquement le rayonnement solaire et réémet dans l’infrarouge. La température est déterminée par l’équilibre entre énergie absorbée et énergie rayonnée.*

### Modèle physique
- **Hypothèse** : Corps noir parfait (émissivité = 1)
- **Atmosphère** : Aucune (vide)
- **Calcul** : Bilan radiatif global

### 1. Flux solaire absorbé à la surface ($S_{\text{abs}}$)
$$
S_{\text{abs}} = \frac{S_0}{4} \times (1 - \alpha)
$$
où :
- $S_0 = 1366\ \text{W/m}^2$ (constante solaire)
- $\alpha = 0.30$ (albédo planétaire)

$$
\Rightarrow\ S_{\text{abs}} = 239.75\ \text{W/m}^2
$$

### 2. Bilan énergétique à la surface

$$
S_{\text{abs}} = \sigma T_e^4
$$

### 3. Température effective
$$
T_e = \left( \frac{239.75}{5.670367 \times 10^{-8}} \right)^{1/4} = 254.9\ \text{K}
$$
$$
T_e(^\circ\text{C}) = 254.9 - 273.15 = \mathbf{-18.3^\circ\text{C}}
$$

**Résultat** :  

<p style="text-align:center;">
  <span style="display:inline-block; border:1px solid white; padding:1px 6px; font-weight:bold;">
    Température = -18.3 °C
  </span>
</p>

### Sources
- Kopp & Lean, 2011
- Loeb et al., 2018 (CERES)

---

## 2. Terre avec atmosphère sans CO₂

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 0 ppm.*

### Modèle physique
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds or rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 0 ppm


### 1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{237.886\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 237.886 W/m²

---

### 2. Bilan énergétique à la surface

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

---

### 3. Température au sol
$$
T_s = \left( \frac{298.886}{5.670367 \times 10^{-8}} \right)^{1/4} = 278.42\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 278.42 - 273.15 = \mathbf{5.3^\circ\text{C}}
$$

**Résultat** :  

<p style="text-align:center;">
  <span style="display:inline-block; border:1px solid white; padding:1px 6px; font-weight:bold;">
    Température = 5.3 °C
  </span>
</p>

*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ absent)*

---

### Sources
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)

---

## 3. CO₂ à 280 ppm (préindustriel — 1880)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 280 ppm.*

### Modèle physique
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds or rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 280 ppm


### 1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{267.183\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 267.183 W/m²

---

### 2. Bilan énergétique à la surface

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

---

### 3. Température au sol
$$
T_s = \left( \frac{328.183}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.15\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.15 - 273.15 = \mathbf{15.0^\circ\text{C}}
$$

**Résultat** :  

<p style="text-align:center;">
  <span style="display:inline-block; border:1px solid white; padding:1px 6px; font-weight:bold;">
    Température = 15.0 °C
  </span>
</p>

*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 280 ppm)*

---

### Sources
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)

---

## 4. CO₂ à 420 ppm (2024)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 420 ppm.*

### Modèle physique
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds or rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 420 ppm


### 1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{269.255\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 269.255 W/m²

---

### 2. Bilan énergétique à la surface

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

---

### 3. Température au sol
$$
T_s = \left( \frac{330.255}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.49\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.49 - 273.15 = \mathbf{15.34^\circ\text{C}}
$$

**Résultat** :  

<p style="text-align:center;">
  <span style="display:inline-block; border:1px solid white; padding:1px 6px; font-weight:bold;">
    Température = 15.34 °C
  </span>
</p>

*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 420 ppm)*

---

### Sources
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)

---

## 5. CO₂ à 560 ppm (doublement de 1880)

*Atmosphère réaliste avec H₂O, O₃, CH₄, N₂O, mais CO₂ = 560 ppm.*

### Modèle physique
- **Calcul** : MODTRAN 3 version 1.3,
- **Profil** : 1976 U.S. Standard Atmosphere, no clouds or rain - Altitude 0 km
- **Gaz présents** : Tous gaz par défaut sauf CO₂ = 560 ppm


### 1. Flux IR descendant à la surface ($F_{\text{LW}\downarrow}$)
$$
F_{\text{LW}\downarrow} = I_{\text{A}}^{\text{down}} = \mathbf{270.731\ \text{W/m}^2}
$$
> **Source** : MODTRAN  Downward IR Heat Flux = 270.731 W/m²

---

### 2. Bilan énergétique à la surface

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

---

### 3. Température au sol
$$
T_s = \left( \frac{331.731}{5.670367 \times 10^{-8}} \right)^{1/4} = 288.70\ \text{K}
$$
$$
T_s(^\circ\text{C}) = 288.70 - 273.15 = \mathbf{15.55^\circ\text{C}}
$$

**Résultat** :  

<p style="text-align:center;">
  <span style="display:inline-block; border:1px solid white; padding:1px 6px; font-weight:bold;">
    Température = 15.55 °C
  </span>
</p>

*(Effet de serre partiel dû à H₂O, O₃, CH₄, N₂O — CO₂ = 560 ppm)*

---

### Sources
- **MODTRAN 3 version 1.3**
  [http://climatemodels.uchicago.edu/modtran/](http://climatemodels.uchicago.edu/modtran/)
- **Trenberth et al., 2009** (*BAMS*, doi:10.1175/2008BAMS2634.1)

---

## Comparaison des températures selon le CO₂ (MODTRAN)

| Cas | CO₂ (ppm) | Température (°C) |
|-----|-----------|------------------|
| Sans atmosphère | 0 | **-18.3** |
| Avec atmosphère (sans CO₂) | 0 | **5.3** |
| Préindustriel | 280 | **15.0** |
| Actuel (2024) | 420 | **15.34** |
| Doublement (560 ppm) | 560 | **15.55** |

---

## Et que dit le GIEC ?

[Insérez ici votre petit texte explicatif sur le GIEC et les forçages radiatifs.]

<div style="text-align: center; margin: 20px 0;">
  <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAoAAAAHgCAYAAAAFlDklAAAACXBIWXMAAAsTAAALEwEAmpwYAAAgAElEQVR4nOzdd3gU1dvG8e+m6S0lZSUtLS3tLq6u7m7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u7u:10.0pt;">    <img src="https://www.ipcc.ch/report/ar6/wg1/downloads/report/IPCC_AR6_WGI_Full_Report.pdf#page=959" alt="GIEC AR6 Figure 7.8" style="max-width:100%; height:auto;">  
  </a>
</div>

**Faisons les calculs en partant de la valeur de la température de 1880, et regardons ce que produisent ces forçages radiatifs donnés par le GIEC.**

---

## 6. Calcul GIEC : 420 ppm et 560 ppm à partir de 1880

### Modèle physique
- **Température de référence (1880)** : **15.0 °C** = 288.15 K  
- **Forçage radiatif total (1750 → 2019)** : **2.72 W/m²** (GIEC AR6, Figure 7.8, p. 959)  
- **Sensibilité climatique (λ)** : ΔT = λ × ΔF  
  → λ = **0.8 K / (W/m²)** (médiane des modèles CMIP6, GIEC AR6)

---

### 1. CO₂ à 420 ppm (2024)

- **Forçage CO₂ seul** : **~1.68 W/m²** (GIEC, p. 959)  
- **ΔT (CO₂ seul)** : 1.68 × 0.8 = **1.34 °C**  
- **Température finale** : 15.0 + 1.34 = **16.34 °C**

---

### 2. CO₂ à 560 ppm (doublement)

- **Forçage CO₂ seul** : **~3.71 W/m²** (doublement = +3.71 W/m²)  
- **ΔT (CO₂ seul)** : 3.71 × 0.8 = **2.97 °C**  
- **Température finale** : 15.0 + 2.97 = **17.97 °C**

---

**Résultat GIEC (forçage + sensibilité)** :

| CO₂ (ppm) | ΔF (W/m²) | ΔT (°C) | T finale (°C) |
|-----------|-----------|---------|---------------|
| 420       | +1.68     | +1.34   | **16.34**     |
| 560       | +3.71     | +2.97   | **17.97**     |

> **Source** : IPCC AR6 WG1, Figure 7.8, p. 959  
> [Lien direct → Page 959](https://www.ipcc.ch/report/ar6/wg1/downloads/report/IPCC_AR6_WGI_Full_Report.pdf#page=959)