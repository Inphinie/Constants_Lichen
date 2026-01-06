# ⚛️ Universal Atom & Constants
**Fundamental Physics Kernel**

> **"Si vous voulez trouver les secrets de l'univers, pensez en termes d'énergie, de fréquence et de vibration."** — *Nikola Tesla*

[![Language](https://img.shields.io/badge/Lang-Rust-orange?style=for-the-badge&logo=rust)](https://www.rust-lang.org/)
[![Language](https://img.shields.io/badge/Lang-Python-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![Physics](https://img.shields.io/badge/Physics-Newtonian_&_Quantum-purple?style=for-the-badge&logo=atom)](./FORMULAS.md)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue?style=for-the-badge&logo=apache)](https://opensource.org/licenses/Apache-2.0)

---

## 🌌 Vue d'ensemble

Ce dépôt constitue la couche physique fondamentale ("Physics Layer") de l'architecture. Il a deux fonctions critiques :
1.  **Légiférer :** Définir les constantes immuables de l'univers (Mathématiques & Physiques).
2.  **Simuler :** Fournir l'entité de base (`UniversalAtom`) capable d'interagir dans un espace 3D selon ces lois.

## 🧱 Architecture Hybride

Le système utilise une approche hybride pour allier lisibilité et performance :

### 1. Les Constantes (`fundamental_constants.py`) 🐍
Définition haute précision des invariants universels. Ce fichier sert de "Source de Vérité" pour tout le système.

* **Mathématiques :** $\pi$ (Pi), $\phi$ (Nombre d'Or), $\sqrt{2}$, etc.
* **Physique :** $c$ (Vitesse de la lumière), $G$ (Gravitation), $h$ (Planck).
* **Dérivées :** Calcul automatique des unités de Planck (Temps, Longueur, Masse).
* *Fonctionnalité :* Inclut un script de vérification de la cohérence dimensionnelle (`verify_consistency`).

### 2. L'Atome Universel (`universal_atom.rs`) 🦀
Implémentation en **Rust** de l'entité particulaire pour une performance maximale lors des simulations à n-corps.

* **Propriétés :** Masse, Charge, Spin, Position (Vector3), Vélocité.
* **Méthodes :**
    * `interact()` : Calcul des forces inter-particulaires.
    * `update()` : Intégration temporelle (Euler/Verlet) pour le mouvement.

## 📐 Formules & Modèles

Le moteur repose sur des équations décrites dans le document [FORMULAS.md](./FORMULAS.md).

> Le système intègre des principes de géométrie sacrée et de physique unifiée, utilisant le **Nombre d'Or ($\phi$)** comme ratio d'échelle fondamental pour l'organisation de la matière.

## 🛠️ Usage

### Python (Definitions)
```python
from fundamental_constants import PLANCK_CONSTANT, GOLDEN_RATIO

print(f"L'univers tourne sur un ratio de {GOLDEN_RATIO}")

```

### Rust (Simulation)

```rust
let atom_a = UniversalAtom::new(mass, charge, position_a);
let atom_b = UniversalAtom::new(mass, charge, position_b);

// Calcul de l'interaction
let force = atom_a.interact(&atom_b);

```

---

*Ce module est une composante critique du Lichen Universe Unified.*
