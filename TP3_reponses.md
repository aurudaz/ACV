# TP3 — Réponses et interprétations

## Exercice 1 — Canette vs PET (IMPACT World+ Footprint)

### Partie 1 — Canette en aluminium primaire
**Graphique contribution** : `outputs/ex1_contribution_Canette_Al_primaire.png`

**Processus le plus contributeur (global)** : **Aluminium primaire** (dominant sur CC, EQ_r, FNEU, HH_r).  
**Transfert d’impact** : la catégorie **WS** est dominée par **le sucre de betterave** plutôt que l’aluminium, ce qui montre un déplacement vers les impacts liés aux matières agricoles.

**Totaux par catégorie (FU)**
| Catégorie | Total |
|---|---:|
| CC | 0.25399769 |
| EQ_r | 0.061544222 |
| FNEU | 2.8482661 |
| HH_r | 3.6041179e-07 |
| WS | 0.12677334 |

---

### Partie 2 — Canette avec aluminium recyclé (cut-off)
**Graphique contribution** : `outputs/ex1_contribution_Canette_Al_recyclé.png`

**Processus le plus contributeur (global)** : **Aluminium primaire** reste dominant pour CC, EQ_r, FNEU, HH_r.  
**Transfert d’impact** : la catégorie **WS** reste dominée par **le sucre de betterave**, alors que les autres catégories sont dominées par l’aluminium primaire.

**Totaux par catégorie (FU)**
| Catégorie | Total |
|---|---:|
| CC | 0.159735782 |
| EQ_r | 0.043853614 |
| FNEU | 1.8674629 |
| HH_r | 2.29585094e-07 |
| WS | 0.107951004 |

---

### Partie 3 — Bouteille PET
**Graphique contribution** : `outputs/ex1_contribution_Bouteille_PET.png`

**Processus le plus contributeur (global)** : **PET** (dominant sur CC, FNEU, HH_r).  
**Transfert d’impact** : **EQ_r** et **WS** sont dominés par **le sucre de betterave**, montrant un déplacement vers les impacts agricoles malgré le changement d’emballage.

**Totaux par catégorie (FU)**
| Catégorie | Total |
|---|---:|
| CC | 0.09623809 |
| EQ_r | 0.025805932 |
| FNEU | 1.2997011 |
| HH_r | 7.232979e-08 |
| WS | 0.06925694 |

---

### Partie 4 — Comparaison des scénarios
**Graphique comparatif** : `outputs/ex1_comparison_totals.png`

**Conclusion** : la **bouteille PET** présente les **impacts les plus faibles dans toutes les catégories**. La canette avec aluminium recyclé est intermédiaire, et la canette en aluminium primaire est la plus impactante. Il n’y a **pas de scénario “meilleur” uniquement sur certaines catégories** : le PET est systématiquement meilleur dans ce calcul.

---

## Exercice 2 — SOFC

### Analyse de contribution
**Graphique contribution** : `outputs/ex2_contribution_sofc.png`

**Processus le plus contributeur (global)** : **Hydrogène** (dominant dans toutes les catégories).  
**Transfert d’impact** : pas de transfert marqué entre catégories ; les contributions des matériaux (Ni, ZrO₂, La, acier) et du BoP restent secondaires.

**Totaux par catégorie (FU)**
| Catégorie | Total |
|---|---:|
| CC | 0.106557595 |
| EQ_r | 0.032136582 |
| FNEU | 1.265291087 |
| HH_r | 1.525732432e-07 |
| WS | 0.346527181 |

---

### Analyse de sensibilité (CC)
**Tornado plot** : `outputs/ex2_sensitivity_tornado.png`

**Paramètres les plus sensibles (ordre décroissant)** :
1. **H2** (de très loin le plus influent)  
2. **BoP (units)**  
3. **Stack (units)**  
4. **Masse_Nickel**  
5. **Masse_Acier**  
6. **Masse_Lanthane**  
7. **Masse_Zircone**  
8. **EoL (units)**  

**Conclusion** : l’incertitude sur la consommation d’H2 domine largement la robustesse du résultat CC ; les paramètres de BoP et de durée de vie (via les unités) ont un impact secondaire mais non négligeable.
