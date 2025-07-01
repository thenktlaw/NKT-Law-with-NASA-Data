📘 **Read full documentation in the [Wiki](https://github.com/thenktlaw/NKT-Law-with-NASA-Data/wiki)**
# NKT-Law-with-NASA-Data
Experimental verification of the NKT Law using planetary motion data
NKT-Law-with-NASA-Data
🔬 Introduction
The NKT Law on Position and Varying Inertia Interaction proposes a new physical principle:

Inertia is not constant but varies with position in space.

This challenges a long-standing assumption in classical mechanics — that mass (or inertia) is invariant. The NKT Law offers a compact formalism to describe planetary motion where inertia is a function of position.

📐 Theoretical Framework
The NKT Law is represented through two scalar expressions:

𝑆
1
=
𝑥
⃗
⋅
𝑝
⃗
and
𝑆
2
=
𝑝
⃗
⋅
𝑑
𝑚
⃗
𝑑
𝑡
S 
1
​
 = 
x
 ⋅ 
p
​
 andS 
2
​
 = 
p
​
 ⋅ 
dt
d 
m
 
​
 
Where:

𝑥
⃗
x
 : position vector (e.g., heliocentric distance)

𝑣
⃗
v
 : velocity vector

𝑝
⃗
=
𝑚
(
𝑥
⃗
)
𝑣
⃗
p
​
 =m( 
x
 ) 
v
 : momentum vector

𝑚
(
𝑥
⃗
)
m( 
x
 ): position-dependent inertia

𝑑
𝑚
𝑑
𝑡
dt
dm
​
 : time derivative of inertia

These expressions quantify how position-dependent inertia alters dynamics, leading to novel physical consequences in gravitational systems.

🧪 Experimental Verification
This repository contains experimental validation of the NKT Law using real planetary motion data from NASA's JPL HORIZONS system. Specifically:

12-month data for Earth in 2022

Data for other planets such as Mars, Venus, and Jupiter (in progress)

Calculated quantities:

𝑥
x: distance from the Sun

𝑣
v: orbital velocity

𝑚
(
𝑥
)
m(x): inferred effective inertia

𝑝
=
𝑚
𝑣
p=mv

𝑑
𝑚
𝑑
𝑡
dt
dm
​
 

𝑆
1
=
𝑥
⋅
𝑝
S 
1
​
 =x⋅p, and 
𝑆
2
=
𝑝
⋅
𝑑
𝑚
𝑑
𝑡
S 
2
​
 =p⋅ 
dt
dm
​
 

The numerical results reveal consistent behavior aligned with the NKT predictions across time.

🌌 Implications
If inertia truly varies with position, this affects all gravitational theories.

Could influence our understanding of galaxy rotation curves without invoking dark matter.

Offers alternative explanations to frame-dragging, energy conservation, and gravitational lensing.

📂 Files and Data
/data/: CSV files of heliocentric data, derived quantities

/graphs/: PNG images of orbital charts, S₁/S₂ trends

/doc/: PDF report for full analysis

📚 References
The NKT Law on Figshare (preprint)

Wikiversity: NKT Law

NASA HORIZONS data system

🔖 License
This repository is licensed under CC BY 4.0.
You may share, adapt, or reuse with attribution.

© Tung Nguyen, 2025

📌 Next steps
Upload experimental data for Mars, Jupiter

Extend model into galactic-scale simulations

Invite peer discussion and critique

📎 Citation (APA)
Nguyen, T. (2025). The NKT Law on Position and Varying Inertia Interaction: Experimental Verification with NASA Data. GitHub. https://github.com/thenktlaw/NKT-Law-with-NASA-Data
