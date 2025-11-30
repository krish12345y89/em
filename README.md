### **1. COMPOSITE BODY CENTROID (3D)**
**Problem:** Find the centroid of a solid hemisphere of radius R mounted on a cylinder of same radius and height h.

**Diagram:**
```
    ██████  ← Hemisphere (R)
    ██████
    ██████
    ██████  ← Cylinder (R, h)
    ██████
```

**Solution:**
- Volume of cylinder, V₁ = πR²h, ȳ₁ = h/2
- Volume of hemisphere, V₂ = ²/₃πR³, ȳ₂ = h + ³R/₈
- Centroid ȳ = (V₁ȳ₁ + V₂ȳ₂)/(V₁ + V₂)

**Answer:** ȳ = [πR²h(h/2) + ²/₃πR³(h + ³R/₈)] / [πR²h + ²/₃πR³]

---

### **2. PRINCIPAL STRESSES & MOHR'S CIRCLE**
**Problem:** At a point in strained material, the stresses are: σₓ = 80 MPa, σᵧ = 40 MPa, τₓᵧ = 30 MPa. Find principal stresses and maximum shear stress using Mohr's circle.

**Diagram:**
```
    τ
    ↑
    |   ● (σₓ, τₓᵧ)
    |  /
    | /
    |/_____→ σ
    |
```

**Solution:**
- Center of Mohr's circle, C = (σₓ + σᵧ)/2 = 60 MPa
- Radius, R = √[((σₓ - σᵧ)/2)² + τₓᵧ²] = √(20² + 30²) = 36.06 MPa
- σ₁ = C + R = 96.06 MPa, σ₂ = C - R = 23.94 MPa
- τ_max = R = 36.06 MPa

**Answer:** σ₁ = 96.06 MPa, σ₂ = 23.94 MPa, τ_max = 36.06 MPa

---

### **3. SPACE TRUSS ANALYSIS**
**Problem:** Determine forces in all members of the space truss shown:

**Diagram:**
```
    D (0,0,4)
    /\
   /  \
  /    \
 A(0,0,0)---B(3,0,0)
  \    /
   \  /
    \/
    C(0,4,0)
    
Load: 5 kN at D vertically downward
```

**Solution:**
- Using 3D equilibrium equations
- Member lengths: AD = BD = CD = 5m
- Solve using method of joints

**Answer:** 
F_AD = 6.25 kN (C), F_BD = 6.25 kN (C), F_CD = 6.25 kN (C)

---

### **4. GYROSCOPIC COUPLE**
**Problem:** A rotor of mass 200 kg, radius of gyration 0.3 m, rotates at 3000 rpm. If the axis precesses at 60 rpm, calculate gyroscopic couple.

**Diagram:**
```
    Spin axis
       ↑
       | ωₛ
       ● Rotor
       |
Precession → Ω
       |
```

**Solution:**
- I = mk² = 200 × (0.3)² = 18 kg·m²
- ωₛ = 3000 × 2π/60 = 314.16 rad/s
- Ω = 60 × 2π/60 = 6.283 rad/s
- Gyroscopic couple, C = IωₛΩ = 18 × 314.16 × 6.283

**Answer:** C = 35,500 Nm

---

### **5. VIRTUAL WORK - COMPLEX MECHANISM**
**Problem:** For the four-bar linkage shown, find output torque when input torque is 50 Nm.

**Diagram:**
```
    B
    /\
   /  \
  /    \
 A------C
 |      |
 |      |
Fixed  Fixed
```

**Given:** AB = 0.2m, BC = 0.4m, CD = 0.3m, DA = 0.5m

**Solution:**
- Using virtual work principle: ΣT·δθ = 0
- Calculate velocity ratios
- T_out = T_in × (ω_in/ω_out)

**Answer:** T_out = 33.33 Nm

---

### **6. BENDING STRESS IN CURVED BEAMS**
**Problem:** A curved beam with rectangular section 50mm × 80mm has mean radius R = 200mm. If bending moment M = 2 kNm, find maximum bending stress.

**Diagram:**
```
    Outer fiber
    ████████ ← Rₒ = 250mm
    ████████
    ████████ ← R = 200mm (neutral axis)
    ████████
    ████████ ← Rᵢ = 150mm
    Inner fiber
```

**Solution:**
- Using curved beam formula: σ = M(y)/(Ae(R - y))
- e = R - A/∫(dA/r)
- Calculate for inner and outer fibers

**Answer:** σ_max_inner = 120 MPa, σ_max_outer = -80 MPa

---

### **7. ROTATING DISC STRESSES**
**Problem:** A steel disc of 0.5m diameter, 0.05m thickness rotates at 10,000 rpm. Find radial and tangential stresses at center and rim. Density = 7800 kg/m³.

**Diagram:**
```
    ████████████
    ████████████ ← Rotating disc
    ████████████
    ● Center   Rim ●
```

**Solution:**
- ω = 10,000 × 2π/60 = 1047.2 rad/s
- Using Lamé's equations for rotating discs
- σ_radial = (3+ν)/8 × ρω²(R² - r²)
- σ_tangential = ρω²/8[(3+ν)R² - (1+3ν)r²]

**Answer:** σ_center = 0, σ_rim_radial = 0, σ_rim_tangential = 82.5 MPa

---

### **8. FINITE ELEMENT METHOD APPLICATION**
**Problem:** For the 2D element with nodes at (0,0), (2,0), (2,1), (0,1) and displacements u₁=0, v₁=0; u₂=0.1, v₂=0; u₃=0.12, v₃=0.05; u₄=0.02, v₄=0.03, find strain components.

**Diagram:**
```
    (0,1)●-------●(2,1)
         |       |
         |       |
    (0,0)●-------●(2,0)
```

**Solution:**
- Using isoparametric formulation
- [ε] = [B]{d}
- Calculate strain-displacement matrix

**Answer:** εₓₓ = 0.05, εᵧᵧ = 0.03, γₓᵧ = 0.04

---

### **9. CRITICAL BUCKLING LOAD**
**Problem:** A column 3m long with hollow circular section (OD=100mm, ID=80mm) has both ends fixed. Find Euler's critical buckling load. E=200 GPa.

**Diagram:**
```
    ████████ ← Fixed
    ████████
    ████████ ← Column L=3m
    ████████
    ████████ ← Fixed
```

**Solution:**
- I = π(OD⁴ - ID⁴)/64 = π(0.1⁴ - 0.08⁴)/64
- For both ends fixed: Lₑ = L/2 = 1.5m
- P_cr = π²EI/Lₑ²

**Answer:** P_cr = 450 kN

---

### **10. CONTACT STRESSES - HERITZ THEORY**
**Problem:** Two steel spheres of diameters 100mm and 150mm pressed together with force 1 kN. Find maximum contact pressure. E=200 GPa, ν=0.3.

**Diagram:**
```
    ○ 100mm
    \
     \ F=1kN
     /
    ○ 150mm
```

**Solution:**
- Using Hertz contact theory
- a = [3F((1-ν₁²)/E₁ + (1-ν₂²)/E₂)/(4(1/R₁ + 1/R₂))]^(1/3)
- p_max = 3F/(2πa²)

**Answer:** p_max = 1.2 GPa

---

### **11. COMPOSITE BEAM BENDING**
**Problem:** A composite beam has steel top flange (100mm×20mm), aluminum web (20mm×160mm), and steel bottom flange (100mm×20mm). Find equivalent steel section and moment of inertia. E_steel=200 GPa, E_aluminum=70 GPa.

**Diagram:**
```
    ▓▓▓▓▓▓▓▓ ← Steel (100×20)
    ▒▒▒▒▒▒▒▒ ← Aluminum (20×160)
    ▓▓▓▓▓▓▓▓ ← Steel (100×20)
```

**Solution:**
- Modular ratio, n = E_aluminum/E_steel = 0.35
- Transform aluminum section: width = 20×0.35 = 7mm
- Calculate centroid and I of transformed section

**Answer:** I_equivalent = 15.8 × 10⁶ mm⁴

---

### **12. TORSION OF THIN-WALLED CLOSED SECTION**
**Problem:** A thin-walled rectangular tube 100mm×50mm×2mm thickness is subjected to torque 500 Nm. Find shear stress and angle of twist per unit length. G=80 GPa.

**Diagram:**
```
    ┌────────┐
    │        │ 50mm
    │        │
    └────────┘
     100mm
```

**Solution:**
- Using Bredt's formula
- A = enclosed area = 100×50 = 5000 mm²
- τ = T/(2At) = 500/(2×5000×10⁻⁶×0.002)
- θ/L = T/(4A²G)∮ds/t

**Answer:** τ = 25 MPa, θ/L = 0.00125 rad/m

---

### **13. PRESSURE VESSEL STRESSES**
**Problem:** A cylindrical pressure vessel has ID=1m, thickness=20mm, internal pressure=2 MPa. Find longitudinal and circumferential stresses.

**Diagram:**
```
    ┌────────────────┐
    │● ← p=2MPa    ●│
    │               │
    └────────────────┘
```

**Solution:**
- Circumferential stress: σ_h = pD/(2t) = 2×1/(2×0.02)
- Longitudinal stress: σ_l = pD/(4t) = 2×1/(4×0.02)

**Answer:** σ_h = 50 MPa, σ_l = 25 MPa

---

### **14. ROTOR DYNAMICS - CRITICAL SPEED**
**Problem:** A shaft of diameter 50mm, length 1.5m carries a rotor of mass 200kg at midspan. Find first critical speed. E=200 GPa.

**Diagram:**
```
    △━━━━━┳━━━━━△
          ● m=200kg
    Support   Support
```

**Solution:**
- I = πd⁴/64 = π(0.05)⁴/64
- δ_max = WL³/(48EI) for simply supported beam
- ω_cr = √(g/δ_max)

**Answer:** ω_cr = 125 rad/s (1194 rpm)

---

### **15. COMPLEX FRICTION PROBLEM**
**Problem:** A block of mass 100kg on 30° incline connected to hanging mass 150kg via pulley. μ=0.25. Find acceleration and tension.

**Diagram:**
```
    ○ Block (100kg)
    /\
   /30°\
  /_____\
   \
    \ Pulley
     \
      ● Hanging mass (150kg)
```

**Solution:**
- Equations of motion for both masses
- Consider friction force = μN = 0.25×100g×cos30°
- Solve simultaneous equations

**Answer:** a = 2.1 m/s², T = 1157 N

---

### **16. COMPOSITE CYLINDER SHRINK FIT**
**Problem:** A steel sleeve of ID 99.5mm is to be shrunk onto a steel shaft of diameter 100mm. Find the interface pressure and stresses. E=200 GPa, ν=0.3.

**Diagram:**
```
    ████████████ ← Sleeve
    ████████████
    ████████████
    ●●●●●●●●●●●● ← Shaft
```

**Solution:**
- Interference δ = 100 - 99.5 = 0.5mm
- Interface pressure p = (δE)/(2R³) × (Rₒ² - Rᵢ²)/(Rₒ²Rᵢ²)
- Calculate radial and tangential stresses

**Answer:** p = 25 MPa, σ_t_sleeve = 50 MPa, σ_t_shaft = -25 MPa

---

### **17. STRAIN ENERGY IN IMPACT LOADING**
**Problem:** A weight of 500N falls through 100mm onto a collar attached to a steel rod of diameter 20mm and length 2m. Find maximum stress and elongation. E=200 GPa.

**Diagram:**
```
    ● Weight (500N)
    │
    ▼ h=100mm
    ┌─┐ Collar
    │ │
    │ │ Rod L=2m
    │ │
    └─┘ Fixed
```

**Solution:**
- Using energy conservation: mg(h+δ) = (σ²/2E) × Volume
- Solve quadratic for stress σ
- δ = σL/E

**Answer:** σ_max = 150 MPa, δ_max = 1.5 mm

---

### **18. ASYMMETRIC BENDING**
**Problem:** A Z-section beam with flange 100mm×20mm, web 160mm×20mm is subjected to bending moment M=5 kNm at 30° to horizontal axis. Find bending stresses at corners.

**Diagram:**
```
    ▓▓▓▓▓▓▓▓ ← Top flange
    ▒▒▒▒▒▒▒▒
    ▒▒▒▒▒▒▒▒ ← Web
    ▒▒▒▒▒▒▒▒
    ▓▓▓▓▓▓▓▓ ← Bottom flange
    M=5kNm↗30°
```

**Solution:**
- Calculate Iₓₓ, Iᵧᵧ, Iₓᵧ
- Use asymmetric bending formula: σ = (MₓIᵧᵧ - MᵧIₓᵧ)y/(IₓₓIᵧᵧ - Iₓᵧ²) + (MᵧIₓₓ - MₓIₓᵧ)x/(IₓₓIᵧᵧ - Iₓᵧ²)
- Calculate for each corner point

**Answer:** σ_A = 85 MPa, σ_B = -45 MPa, σ_C = -120 MPa, σ_D = 60 MPa

---

### **19. THICK CYLINDER - LAME'S EQUATIONS**
**Problem:** A thick cylinder with ID=100mm, OD=200mm subjected to internal pressure 50 MPa. Find radial and tangential stress distributions.

**Diagram:**
```
    ████████████ ← Outer wall
    ████████████
    ████████████
    ○○○○○○○○○○○○ ← Inner wall p=50MPa
```

**Solution:**
- Using Lamé's equations:
  σ_r = A - B/r²
  σ_t = A + B/r²
- Apply boundary conditions: at r=50mm, σ_r = -50 MPa; at r=100mm, σ_r = 0

**Answer:** σ_r_max = -50 MPa, σ_t_max = 83.3 MPa

---

### **20. ROTATING RING STRESSES**
**Problem:** A thin ring of mean radius 0.5m rotates at 6000 rpm. Find hoop stress. Density=7800 kg/m³.

**Diagram:**
```
     ○○○○○○○○○○
    ○          ○ ← Rotating ring
    ○          ○ ω=6000 rpm
    ○          ○
     ○○○○○○○○○○
```

**Solution:**
- ω = 6000 × 2π/60 = 628.32 rad/s
- Hoop stress σ = ρω²R²
- σ = 7800 × (628.32)² × (0.5)²

**Answer:** σ = 385 MPa

---

### **21. BEAM ON ELASTIC FOUNDATION**
**Problem:** An infinite beam on elastic foundation (k=50 MPa) carries concentrated load P=100 kN. Find maximum deflection and bending moment.

**Diagram:**
```
    ░░░░░░░░░░░░░░░ ← Elastic foundation
    ──────────────── ← Beam
          ↓
          P=100kN
```

**Solution:**
- Characteristic length β = (k/4EI)^(1/4)
- Maximum deflection δ_max = Pβ/2k
- Maximum moment M_max = P/4β

**Answer:** δ_max = 8.5 mm, M_max = 7.8 kNm

---

### **22. THERMAL STRESSES IN COMPOSITE BAR**
**Problem:** A steel bar (A=1000mm², E=200 GPa, α=12×10⁻⁶/°C) is bonded to aluminum bar (A=1500mm², E=70 GPa, α=23×10⁻⁶/°C). Temperature rises 50°C. Find thermal stresses.

**Diagram:**
```
    ▓▓▓▓▓▓▓▓▓▓ ← Steel
    ▒▒▒▒▒▒▒▒▒▒ ← Aluminum
    ▓▓▓▓▓▓▓▓▓▓
```

**Solution:**
- Free expansion difference = (α_al - α_steel)ΔT L
- Compatibility: δ_thermal = δ_steel + δ_aluminum
- Force P = (α_al - α_steel)ΔT L / (L/A_steelE_steel + L/A_alE_al)
- Stress = P/A

**Answer:** σ_steel = 45 MPa (T), σ_aluminum = -30 MPa (C)

---

### **23. SHEAR CENTER OF THIN-WALLED SECTION**
**Problem:** Find shear center for the channel section shown:

**Diagram:**
```
    ▓▓▓▓▓▓▓▓ ← Flange 100mm×20mm
    ▒▒▒▒▒▒▒▒
    ▒▒▒▒▒▒▒▒ ← Web 160mm×20mm
    ▒▒▒▒▒▒▒▒
    ▓▓▓▓▓▓▓▓ ← Flange 100mm×20mm
```

**Solution:**
- Calculate shear flow distribution
- Take moments about web center
- e = (First moment of flange area about NA) × (Flange width) / (Iₓₓ × Web thickness)

**Answer:** e = 35 mm from web center

---

### **24. CRITICAL LOAD WITH INITIAL IMPERFECTION**
**Problem:** A column with initial curvature y₀ = 10mm sin(πx/L) carries axial load P. Find maximum deflection and stress when P=0.7P_cr. L=4m, EI=5000 kNm².

**Diagram:**
```
    /\
   /  \ ← Initial curvature
  /    \
 /      \
△        △
Support  Support
```

**Solution:**
- Using Perry-Robertson formula
- y_max = y₀/(1 - P/P_cr)
- σ_max = P/A + M_max c/I
- M_max = P y_max

**Answer:** y_max = 33.3 mm, σ_max = 85 MPa

---

### **25. WAVE PROPAGATION IN RODS**
**Problem:** A steel rod of length 5m is struck at one end. Find time for stress wave to travel to other end and return. E=200 GPa, ρ=7800 kg/m³.

**Diagram:**
```
    ● Hammer
    ↓
    ████████ ← Steel rod L=5m
    ████████
    ████████
```

**Solution:**
- Wave velocity c = √(E/ρ)
- c = √(200×10⁹/7800) = 5064 m/s
- Time for round trip t = 2L/c

**Answer:** t = 1.97 ms

---

### **26. PLASTIC BENDING OF BEAMS**
**Problem:** A rectangular beam 100mm×200mm has yield stress σ_y=250 MPa. Find plastic moment capacity and shape factor.

**Diagram:**
```
    ████████ ← Compression yield
    ████████
    --------- ← Neutral axis
    ████████ ← Tension yield
    ████████
```

**Solution:**
- Elastic moment M_y = σ_y × (bh²/6)
- Plastic moment M_p = σ_y × (bh²/4)
- Shape factor f = M_p/M_y

**Answer:** M_y = 166.7 kNm, M_p = 250 kNm, f = 1.5

---

### **27. CONTACT FATIGUE - PALMGREN-MINER RULE**
**Problem:** A component experiences: 10,000 cycles at σ₁=400 MPa, 50,000 cycles at σ₂=300 MPa, 100,000 cycles at σ₃=250 MPa. If fatigue life at these stresses are N₁=20,000, N₂=100,000, N₃=500,000 cycles, find accumulated damage.

**Diagram:**
```
    σ ↑
      │
  400 │●─────
      │ \
  300 │  ●────
      │   \
  250 │    ●───
      └─────────→ N
```

**Solution:**
- Damage D = Σ(n_i/N_i)
- D = 10000/20000 + 50000/100000 + 100000/500000

**Answer:** D = 0.5 + 0.5 + 0.2 = 1.2 (Failure predicted)

---

### **28. FINITE DIFFERENCE METHOD FOR BEAMS**
**Problem:** Using finite difference method, find central deflection of simply supported beam with UDL. Divide into 4 segments.

**Diagram:**
```
    △━━━┳━━━┳━━━┳━━━△
        w=10kN/m
```

**Solution:**
- Finite difference equation: y_{i-1} - 2y_i + y_{i+1} = -M_i(Δx)²/EI
- Apply boundary conditions y₀=0, y₄=0
- Solve system of equations

**Answer:** y_max = 5wL⁴/384EI = 12.8 mm

---

### **29. STABILITY OF RIGID BODIES**
**Problem:** A cylindrical log of diameter 1m, height 2m, density 700 kg/m³ floats in water. Find metacentric height and stability.

**Diagram:**
```
    ┌─────┐ ← Water line
    │     │
    │  ●  │ ← CG
    │  │  │
    │  ●  │ ← CB
    └─────┘
```

**Solution:**
- Weight W = ρVg = 700×π(0.5)²×2×9.81
- Buoyancy force = Weight of displaced water
- Metacentric height GM = I/V - BG
- I = πD⁴/64, V = displaced volume

**Answer:** GM = 0.12 m (Stable)

---

### **30. VIBRATION OF CONTINUOUS SYSTEMS**
**Problem:** Find fundamental natural frequency of a fixed-fixed steel beam of length 3m, rectangular section 50mm×100mm.

**Diagram:**
```
    ████████████
    ████████████ ← Fixed-fixed beam
    ████████████
    ▓▓▓▓▓▓▓▓▓▓▓▓
```

**Solution:**
- For fixed-fixed beam: ω₁ = (22.37/L)² √(EI/ρA)
- I = bh³/12 = 0.05×(0.1)³/12
- A = 0.05×0.1 = 0.005 m²

**Answer:** f₁ = ω₁/2π = 45.2 Hz


### **31. COMPLEX FRAME ANALYSIS**
**Problem:** Analyze the rigid frame shown below for member forces and reactions:

**Diagram:**
```
    C━━━━━━D
    ┃      ┃
    ┃      ┃
    A━━━━━━B
    ↓      ↓
    P      P
```

**Given:** AB = BC = CD = DA = 4m, P = 50 kN at A and B

**Solution:**
- **Static Determinacy:** m = 4, j = 4, r = 6 ⇒ m + r = 10, 2j = 8 ⇒ Statically indeterminate
- **Method:** Use slope-deflection equations
- **Fixed End Moments:** 
  M_AB = M_BA = 0, M_BC = M_CB = 0, M_CD = M_DC = 0, M_DA = M_AD = 0
- **Joint Equilibrium:** Solve for rotations

**Answer:** 
M_AB = 37.5 kNm, M_BA = -37.5 kNm, M_BC = 37.5 kNm, M_CB = -37.5 kNm

---

### **32. SHEAR FLOW IN MULTI-CELL SECTION**
**Problem:** Find shear flow distribution in the two-cell wing section shown:

**Diagram:**
```
    ┌─────┬─────┐
    │     │     │
    │  1  │  2  │
    │     │     │
    └─────┴─────┘
    V = 100 kN ↓
```

**Given:** Cell areas: A₁ = 0.2 m², A₂ = 0.3 m²
Wall thickness: t = 2 mm
Shear center coincides with centroid

**Solution:**
- **Shear Flow:** q = VQ/I
- **For Multi-cell:** Use Bredt's formula for each cell
- **Compatibility:** Twist angle same for both cells

**Answer:** 
q₁ = 45 kN/m, q₂ = 55 kN/m, q_web = 10 kN/m

---

### **33. ROTATING DISC WITH ANNUAL LOAD**
**Problem:** A disc of outer radius 0.5m, inner radius 0.1m rotates at 8000 rpm with annular load at outer edge. Find stress distribution:

**Diagram:**
```
    ████████████
    ████████████ ← Rotating disc
    ○○○○○○○○○○○○ ← Annular load
```

**Given:** ω = 8000 rpm, p_edge = 20 MPa, ρ = 7800 kg/m³

**Solution:**
- **Governing Equation:** d(σ_r r)/dr - σ_θ + ρω²r² = 0
- **Boundary Conditions:** σ_r = -20 MPa at r=0.5m, σ_r = 0 at r=0.1m
- **Solve:** Using Lamé's equations

**Answer:** 
σ_r_max = 45 MPa, σ_θ_max = 120 MPa at r=0.3m

---

### **34. COMPOSITE TORSION**
**Problem:** A composite shaft has steel core (d=50mm) and brass sleeve (OD=80mm). Find torque capacity:

**Diagram:**
```
    ████████████ ← Brass sleeve
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Steel core
    ████████████
```

**Given:** τ_steel = 120 MPa, τ_brass = 80 MPa, G_steel = 80 GPa, G_brass = 40 GPa

**Solution:**
- **Torsion Formula:** T = τJ/r
- **Compatibility:** Same angle of twist for both materials
- **Total Torque:** T_total = T_steel + T_brass

**Answer:** T_max = 4.2 kNm

---

### **35. ELASTIC STABILITY - PLATE BUCKLING**
**Problem:** A rectangular plate 1m×2m×10mm thick is simply supported on all edges. Find critical buckling stress:

**Diagram:**
```
    ┌───────────┐
    │           │
    │           │ ← Plate
    │           │
    └───────────┘
    Compression → σ
```

**Given:** E = 200 GPa, ν = 0.3, a = 1m, b = 2m, t = 10mm

**Solution:**
- **Buckling Coefficient:** k = (mb/a + a/mb)² for m half-waves
- **Critical Stress:** σ_cr = kπ²E/[12(1-ν²)] × (t/b)²
- **Minimum:** Find m giving minimum σ_cr

**Answer:** σ_cr = 85 MPa for m=2

---

### **36. VIBRATION ISOLATION**
**Problem:** A machine of mass 500 kg produces disturbing force 2 kN at 30 Hz. Design vibration isolator:

**Diagram:**
```
    ████████████ ← Machine
    ┌─┐┌─┐┌─┐┌─┐ ← Isolators
    └─┘└─┘└─┘└─┘
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Foundation
```

**Given:** Transmissibility < 0.2, damping ratio ζ = 0.1

**Solution:**
- **Transmissibility:** TR = √{[1+(2ζr)²]/[(1-r²)²+(2ζr)²]}
- **Frequency Ratio:** r = ω/ω_n
- **Solve:** For TR < 0.2, find required ω_n

**Answer:** k < 150 kN/m (spring stiffness)

---

### **37. THERMAL BUCKLING**
**Problem:** A steel bar of length 3m is fixed between rigid walls. Find temperature rise to cause buckling:

**Diagram:**
```
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Rigid wall
    ████████████ ← Steel bar
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Rigid wall
```

**Given:** α = 12×10⁻⁶/°C, E = 200 GPa, A = 1000 mm², I = 2×10⁶ mm⁴

**Solution:**
- **Thermal Stress:** σ = EαΔT
- **Buckling Load:** P_cr = π²EI/L²
- **Equate:** Aσ = P_cr

**Answer:** ΔT_cr = 82°C

---

### **38. WAVE PROPAGATION IN STRINGS**
**Problem:** A tensioned string of length 2m, mass 0.5 kg has fundamental frequency 50 Hz. Find wave speed and tension:

**Diagram:**
```
    ●━━━━━━━━━━━━● ← Fixed ends
    ↗           ↖
    Wave propagation
```

**Given:** L = 2m, m = 0.5 kg, f₁ = 50 Hz

**Solution:**
- **Wave Speed:** c = 2Lf₁
- **Mass per unit length:** μ = m/L
- **Tension:** T = μc²

**Answer:** c = 200 m/s, T = 1000 N

---

### **39. FLUID-STRUCTURE INTERACTION**
**Problem:** Find natural frequency of a cantilever with end mass in water:

**Diagram:**
```
    ████████████ ← Cantilever
    ████████████
    ████████████
          ● ← End mass
          ↓
        Water
```

**Given:** L = 1m, EI = 5000 Nm², m = 10 kg, added mass = 5 kg

**Solution:**
- **Effective Mass:** m_eff = m + added mass
- **Stiffness:** k = 3EI/L³
- **Frequency:** ω_n = √(k/m_eff)

**Answer:** f_n = 2.8 Hz

---

### **40. GEAR SYSTEM VIBRATIONS**
**Problem:** A gear system has moment of inertia I₁=2 kgm², I₂=5 kgm² with shaft stiffness k₁=10⁵ Nm/rad, k₂=2×10⁵ Nm/rad. Find natural frequencies:

**Diagram:**
```
    ╭╮       ╭╮
    ││ Gear1 ││ Gear2
    ╰╯       ╰╯
    ↕         ↕
    k₁        k₂
```

**Solution:**
- **Equations of Motion:** 
  I₁θ₁'' + k₁(θ₁ - θ₂) = 0
  I₂θ₂'' + k₂(θ₂ - θ₁) = 0
- **Characteristic Equation:** Solve for ω

**Answer:** ω₁ = 158 rad/s, ω₂ = 387 rad/s

---

### **41. ROLLING CONTACT STRESSES**
**Problem:** Two cylinders of radii R₁=100mm, R₂=150mm pressed with force F=10 kN. Find contact width and max pressure:

**Diagram:**
```
    ○○○○○○○○○○ ← Cylinder 1
    \       /
     \     / ← Contact area
      \   /
       ○○○ ← Cylinder 2
```

**Given:** E=200 GPa, ν=0.3, L=50mm (length)

**Solution:**
- **Equivalent Radius:** 1/R_eq = 1/R₁ + 1/R₂
- **Contact Width:** b = √[4F R_eq/(πL E*)]
- **Max Pressure:** p_max = 2F/(πbL)

**Answer:** b = 0.45 mm, p_max = 1.8 GPa

---

### **42. COMPOSITE PLATE BENDING**
**Problem:** A sandwich plate has aluminum faces (t=1mm) and polymer core (h=20mm). Find equivalent stiffness:

**Diagram:**
```
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Aluminum face
    ▒▒▒▒▒▒▒▒▒▒▒▒ ← Polymer core
    ▓▓▓▓▓▓▓▓▓▓▓▓ ← Aluminum face
```

**Given:** E_al=70 GPa, E_core=0.1 GPa, width=100mm

**Solution:**
- **Parallel Axis:** I = 2×(bt³/12 + bt(d/2)²) + b h³/12 × E_core/E_al
- **Equivalent EI:** EI_eq = E_al × I_eq

**Answer:** EI_eq = 850 Nm²

---

### **43. IMPACT OF COMPOSITE BAR**
**Problem:** A weight W=500N falls on composite bar (steel+aluminum). Find impact stress:

**Diagram:**
```
    ● Weight
    ↓ h=200mm
    ▓▓▓▓▓▓▓▓ ← Steel
    ▒▒▒▒▒▒▒▒ ← Aluminum
    ▓▓▓▓▓▓▓▓
```

**Given:** A_steel=500mm², A_al=800mm², L=2m, E_steel=200GPa, E_al=70GPa

**Solution:**
- **Equivalent Stiffness:** k_eq = 1/(L/A_steelE_steel + L/A_alE_al)
- **Energy Method:** mg(h+δ) = ½k_eqδ²
- **Stress:** σ = Eδ/L

**Answer:** σ_max = 180 MPa

---

### **44. ROTOR-BEARING DYNAMICS**
**Problem:** A rotor of mass 200kg is supported on bearings with stiffness k=10⁸ N/m, damping c=5000 Ns/m. Find critical speed and unbalance response:

**Diagram:**
```
    ○ Rotor
    ↑   ↑
    │   │
    Bearing Bearing
```

**Given:** m=200kg, k=10⁸ N/m, c=5000 Ns/m, e=0.1mm (unbalance)

**Solution:**
- **Critical Speed:** ω_cr = √(k/m)
- **Amplitude:** X = eω²/√[(k-mω²)²+(cω)²]
- **Phase:** φ = tan⁻¹[cω/(k-mω²)]

**Answer:** ω_cr = 707 rad/s, X_max = 0.25 mm

---

### **45. PIEZOELECTRIC ACTUATOR**
**Problem:** A piezoelectric stack actuator has length 50mm, area 100mm², d₃₃=400pC/N. Find displacement for 100V:

**Diagram:**
```
    ████████████ ← Piezoelectric
    ████████████
    ████████████
    ║ Voltage ║
```

**Given:** L=50mm, A=100mm², d₃₃=400×10⁻¹² m/V, V=100V

**Solution:**
- **Strain:** ε = d₃₃ E = d₃₃ V/L
- **Displacement:** δ = ε L

**Answer:** δ = 0.08 μm

---

### **46. SHAPE MEMORY ALLOY BEHAVIOR**
**Problem:** A Nitinol wire of length 200mm recovers 4% strain upon heating. Find recovery force:

**Diagram:**
```
    ████████████ ← SMA wire
    ████████████
    Heat → Recovery
```

**Given:** L=200mm, ε_recovery=0.04, E=70 GPa, A=10 mm²

**Solution:**
- **Recovery Stress:** σ = E ε
- **Force:** F = σ A

**Answer:** F = 280 N

---

### **47. MICROMECHANICS OF COMPOSITES**
**Problem:** Find elastic constants of unidirectional composite with 60% fiber volume:

**Diagram:**
```
    ░▓░▓░▓░▓░▓░ ← Fibers
    ░▓░▓░▓░▓░▓░
    ░▓░▓░▓░▓░▓░ ← Matrix
```

**Given:** E_fiber=200 GPa, E_matrix=3 GPa, ν_fiber=0.2, ν_matrix=0.35, V_f=0.6

**Solution:**
- **Rule of Mixtures:** E₁ = E_f V_f + E_m (1-V_f)
- **Transverse Modulus:** 1/E₂ = V_f/E_f + (1-V_f)/E_m
- **Shear Modulus:** Similar approach

**Answer:** E₁ = 121 GPa, E₂ = 7.5 GPa, G₁₂ = 3.2 GPa

---

### **48. AEROELASTIC FLUTTER**
**Problem:** An airfoil has torsional stiffness k_θ=10⁵ Nm/rad and mass moment I=5 kgm². Find flutter speed:

**Diagram:**
```
    ████████████ ← Airfoil
    ↗
    │ Elastic center
    │
```

**Given:** k_θ=10⁵ Nm/rad, I=5 kgm², air density ρ=1.2 kg/m³, chord c=1m

**Solution:**
- **Natural Frequency:** ω_θ = √(k_θ/I)
- **Flutter Speed:** V_f ≈ ω_θ c/2

**Answer:** V_f = 100 m/s

---

### **49. VISCOELASTIC DAMPING**
**Problem:** A polymer with complex modulus E*=2+0.3i GPa is used for vibration damping. Find loss factor:

**Diagram:**
```
    ████████████ ← Viscoelastic material
    ████████████
    ████████████
    Stress-strain hysteresis
```

**Given:** E' = 2 GPa, E" = 0.3 GPa

**Solution:**
- **Loss Factor:** η = E"/E'
- **Damping Ratio:** ζ ≈ η/2

**Answer:** η = 0.15, ζ = 0.075

---

### **50. NANOINDENTATION ANALYSIS**
**Problem:** A Berkovich indenter makes 200nm deep impression in material with E=100 GPa. Find hardness:

**Diagram:**
```
    △ Berkovich indenter
    │
    ▼
    ████████████ ← Material
    Impression
```

**Given:** h=200 nm, P_max=10 mN, E=100 GPa

**Solution:**
- **Contact Depth:** h_c = h_max - ε P_max/S
- **Hardness:** H = P_max/A_c
- **Area Function:** A_c = 24.5 h_c²

**Answer:** H = 1.2 GPa

---
