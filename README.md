## **📗 UNIT 1: Force Systems & Equilibrium**

### **1. Coplanar Concurrent Forces**
**Problem:** Two forces P = 100 N at 30° and Q = 150 N at 60° act at a point. Find resultant.

**Solution:**
```
Step 1: Resolve forces
Pₓ = 100 × cos30° = 86.60 N
Pᵧ = 100 × sin30° = 50.00 N
Qₓ = 150 × cos60° = 75.00 N  
Qᵧ = 150 × sin60° = 129.90 N

Step 2: Find resultant
Rₓ = 86.60 + 75.00 = 161.60 N
Rᵧ = 50.00 + 129.90 = 179.90 N
R = √(161.60² + 179.90²) = 241.70 N
θ = tan⁻¹(179.90/161.60) = 48.0°
```
**Answer:** Resultant = 241.7 N at 48.0°

---

### **2. Rigid Body Equilibrium**  
**Problem:** A 5m ladder weighs 200 N, leans at 60° to wall. Find reactions at wall and ground.

**Solution:**
```
Step 1: FBD - Weight at center, reactions at ends
Step 2: Take moments about ground contact
Moment due to weight = 200 × 2.5 × cos60° = 250 Nm
Moment due to wall reaction = R_wall × 5 × sin60° = R_wall × 4.33

Step 3: Equilibrium equations
ΣM = 0: R_wall × 4.33 = 250 ⇒ R_wall = 57.74 N
ΣFy = 0: R_ground_y = 200 N  
ΣFx = 0: R_ground_x = R_wall = 57.74 N
```
**Answer:** Wall reaction = 57.74 N, Ground reaction = 208.2 N at 74°

---

## **📘 UNIT 2: Vectors & Tensors**

### **3. Vector Cross Product**
**Problem:** Find cross product of A = 3i + 2j + k and B = i - j + 2k

**Solution:**
```
A × B = |i   j   k|
        |3   2   1|
        |1  -1   2|
        
= i(2×2 - 1×(-1)) - j(3×2 - 1×1) + k(3×(-1) - 2×1)
= i(4 + 1) - j(6 - 1) + k(-3 - 2)
= 5i - 5j - 5k
```
**Answer:** 5i - 5j - 5k

---

### **4. Tensor Eigenvalues**
**Problem:** Find eigenvalues of tensor T = [[2,1],[1,2]]

**Solution:**
```
Step 1: Characteristic equation
det(|2-λ   1|) = 0
    |1    2-λ|)

(2-λ)² - 1 = 0
λ² - 4λ + 3 = 0

Step 2: Solve quadratic
λ = [4 ± √(16-12)]/2 = [4 ± 2]/2
λ₁ = 3, λ₂ = 1
```
**Answer:** Eigenvalues = 3, 1

---

## **📙 UNIT 3: Structural Analysis**

### **5. Truss - Method of Joints**
**Problem:** Find force in member AB of truss with load 1000 N at joint B.

```
    A
    /\
   /  \
  /    \
B-------C
  1000 N↓
```

**Solution:**
```
Step 1: Support reactions
By symmetry: R_A = R_C = 500 N ↑

Step 2: Joint A analysis
ΣFy = 0: AB × sin60° = 500
AB = 500/sin60° = 577.35 N (Compression)
```
**Answer:** Force in AB = 577.35 N (Compressive)

---

### **6. Zero Force Members**
**Problem:** Identify zero force members:

```
    A---B---C
    |   |   |
    D---E---F
        ↓
        P
```

**Solution:**
```
Rule 1: Joint C - Members BC & CF only, no load ⇒ Both zero force
Rule 2: Joint B - AB, BC, BE; BC zero ⇒ Check BE...
Continue analysis...
```
**Answer:** BC, CF are zero force members

---

## **📒 UNIT 4: Centroid & Moment of Inertia**

### **7. Centroid of Composite Area**
**Problem:** Find centroid of T-section:
- Flange: 200mm × 50mm
- Web: 50mm × 150mm

**Solution:**
```
Step 1: Divide into two rectangles
A₁ = 200×50 = 10000 mm², y₁ = 175 mm
A₂ = 50×150 = 7500 mm², y₂ = 75 mm

Step 2: Find centroid
ȳ = (A₁y₁ + A₂y₂)/(A₁ + A₂)
   = (10000×175 + 7500×75)/17500
   = (1750000 + 562500)/17500 = 132.14 mm
```
**Answer:** Centroid = 132.14 mm from base

---

### **8. Moment of Inertia**
**Problem:** Find Ixx of rectangle 200mm × 100mm about centroid.

**Solution:**
```
Ixx = bh³/12 = 200 × 100³/12 
     = 200 × 1000000/12 
     = 200000000/12 = 16,666,667 mm⁴
```
**Answer:** Ixx = 16.67 × 10⁶ mm⁴

---

### **9. Parallel Axis Theorem**
**Problem:** Find Ixx of above rectangle about base.

**Solution:**
```
I_base = I_centroid + A × d²
       = 16,666,667 + (200×100) × 50²
       = 16,666,667 + 20000 × 2500
       = 16,666,667 + 50,000,000 = 66,666,667 mm⁴
```
**Answer:** I_base = 66.67 × 10⁶ mm⁴

---
