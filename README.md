### **Basic Concepts Samajh (Theory in Short)**

1.  **Particle:** Ek aisa point jahan saara mass concentrate hai. Iska size matter nahi karta.
2.  **Equilibrium:** Jab kisi particle ya body par net force zero hoti hai, toh woh rest mein ya constant velocity se move karti hai. Humare liye, mostly rest ki baat hoti hai.
    - **Condition:** ΣF = 0 (Sum of all forces = 0)
3.  **Rigid Body:** Ek aisi body jo force lagne se deform nahi hoti.
4.  **Coplanar Concurrent Forces:** Saari forces ek hi plane mein hoti hain aur ek hi point par meet karti hain.
5.  **Moment of a Force:** Ye force ka "rotational effect" hota hai. **Moment = Force × Perpendicular Distance**
6.  **Couple:** Do equal, parallel, aur opposite forces jo ek hi body par act karein, lekin different points se. Ye pure body ko sirf rotate karta hai, translate nahi.
7.  **Free Body Diagram (FBD):** Kisi body ko uske surroundings se alag karke, ussi par lagne waali saari forces ko dikhane wala diagram. Ye sabse important step hai.
8.  **Equations of Equilibrium (Coplanar Systems):**
    - ΣFx = 0 (Horizontal forces ka sum zero)
    - ΣFy = 0 (Vertical forces ka sum zero)
    - ΣMabout any point = 0 (Kisi bhi point ke around moments ka sum zero)

---

### **Basic Numericals (Step-by-Step)**

**Numerical 1: Particle Equilibrium (2-D) - Concurrent Forces**

**Problem:** Ek 10 kg ka lamp ek vertical se 30° angle par do wires se latka hua hai. Dono wires mein tension (T1 aur T2) find karo.

```
   A
  / \
 /   \
/  30°\
T1   T2
 \     /
  \   /
   \ /
    O (Lamp, W = m*g)
```

**Solution:**
1.  **Free Body Diagram (FBD):** Lamp (Point O) par teen forces hain:
    - Weight (W) = m*g = 10 * 9.8 = 98 N, vertically downward.
    - Tension T1, wire A-O mein, left side, 30° vertical ke saath.
    - Tension T2, wire B-O mein, horizontally right side. (Maan liya ye horizontal hai simplicity ke liye).

2.  **Equilibrium Equations Lagao:**
    - **ΣFx = 0:** (Forces in x-direction)
        T1 * sin(30°) - T2 = 0 ...(Equation 1)
    - **ΣFy = 0:** (Forces in y-direction)
        T1 * cos(30°) - 98 = 0 ...(Equation 2)

3.  **Solve Karo:**
    - Equation 2 se: T1 * cos(30°) = 98
        T1 = 98 / cos(30°) = 98 / (√3/2) ≈ 98 / 0.866 ≈ **113.2 N**
    - Equation 1 se: T2 = T1 * sin(30°) = 113.2 * 0.5 ≈ **56.6 N**

**Final Answer:** T1 ≈ 113.2 N, T2 ≈ 56.6 N

---

**Numerical 2: Rigid Body Equilibrium & Moment**

**Problem:** Ek 4m lambe beam ke left end (Point A) par ek hinge support hai aur right end (Point B) par a roller support hai. Beam par 2m doori par left end se, ek 200 N ka vertical load downward lag raha hai. Dono supports ke reactions (RA aur RB) find karo.

```
A (Hinge)        C          B (Roller)
|----------------|-----------|
       2m            2m
       ↓
      200 N
```

**Solution:**
1.  **FBD:** Beam ka FBD banao.
    - Point A par: Ek reaction force RA, jiske components honge (RAx horizontal, RAy vertical). (Ya fir hum maan sakte hain ki RA ek resultant force hai jo koi bhi angle par ho sakti hai).
    - Point B par: Roller support sirf vertical reaction de sakta hai, isliye RB purely vertical upward hoga.
    - Load: 200 N downward at point C.

2.  **Equilibrium Equations Lagao (Coplanar System):**
    - **ΣFx = 0:** RAx = 0 ...(Koi horizontal force nahi hai, isliye RAx zero hoga).
    - **ΣMabout A = 0:** (Moment ka equation lagao, kyun ki isse direct RB mil jayega).
        (RB * 4) - (200 * 2) = 0
        Positive moment (Anti-clockwise) liya hai.
    - **ΣFy = 0:** RAy + RB - 200 = 0

3.  **Solve Karo:**
    - Moment equation se: RB * 4 = 400 => RB = 400 / 4 = **100 N (Upward)**
    - ΣFy se: RAy + 100 - 200 = 0 => RAy = 200 - 100 = **100 N (Upward)**

**Final Answer:** Reaction at A (RA) = 100 N (Vertical), Reaction at B (RB) = 100 N (Vertical)

---

**Numerical 3: Couple ka Concept**

**Problem:** Ek steering wheel par do forces lagi hain, dono 20 N ki, parallel aur opposite, jinki lines of action ke beech ki perpendicular distance 0.3m hai. Resultant Couple Moment calculate karo.

**Solution:**
1.  **Concept:** Couple Moment = Force × Perpendicular Distance between forces.
2.  **Calculation:** Moment = 20 N × 0.3 m = **6 N·m**
3.  **Direction:** Yeh moment steering wheel ko rotate karne ki koshish karega (jaise gaadi turn karte waqt).

**Final Answer:** Couple Moment = 6 N·m

---

**Numerical 4: System of Forces & Resultant (2-D)**

**Problem:** Ek particle par teen forces kaam kar rahi hain:
- F1 = 10 N, Right side (+x axis)
- F2 = 15 N, 30° angle par up from right (+x axis)
- F3 = 5 N, Downward (-y axis)
Resultant force find karo.

**Solution:**
1.  **Components Nikalo:**
    - F1x = 10 N, F1y = 0 N
    - F2x = 15 * cos(30°) = 15 * 0.866 = 12.99 N
    - F2y = 15 * sin(30°) = 15 * 0.5 = 7.5 N
    - F3x = 0 N, F3y = -5 N

2.  **Components Sum Karo:**
    - ΣFx = 10 + 12.99 + 0 = **22.99 N**
    - ΣFy = 0 + 7.5 - 5 = **2.5 N**

3.  **Resultant Force (R) Nikalo:**
    - Magnitude: R = √[(ΣFx)² + (ΣFy)²] = √[(22.99)² + (2.5)²] ≈ √[528.54 + 6.25] ≈ √534.79 ≈ **23.12 N**
    - Direction (θ from x-axis): θ = tan⁻¹(ΣFy / ΣFx) = tan⁻¹(2.5 / 22.99) ≈ tan⁻¹(0.1087) ≈ **6.2°**

**Final Answer:** Resultant Force ≈ 23.12 N, 6.2° angle par up from the horizontal.

