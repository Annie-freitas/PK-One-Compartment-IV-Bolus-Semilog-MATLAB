# One‑Compartment IV Bolus Model – MATLAB

A MATLAB simulation of drug concentration following an intravenous (IV) bolus dose, using a one‑compartment pharmacokinetic model. 
The script solves the ordinary differential equation and generates both linear and semilog concentration‑time plots.

## What I Built

- **One‑compartment PK model** with first‑order elimination.
- **Differential equation**: `dC/dt = -(CL/V) * C`, where:
  - `CL` = clearance (L/h)
  - `V`  = volume of distribution (L)
  - `C`  = drug concentration at time `t`
- **IV bolus dose**: initial concentration `C0 = D / V` (dose `D` = 10 mg).
- **ODE solver**: MATLAB’s `ode23` simulates concentration from 0 to 10 hours.
- **Dual visualization**:
  - Linear plot (left subplot) – shows the exponential decay.
  - Semilog plot (right subplot) – reveals the log‑linear relationship, confirming first‑order kinetics.
<img width="560" height="338" alt="image" src="https://github.com/user-attachments/assets/2cb144bf-aa3e-4067-827d-33c9a900f283" />


## Skills Demonstrated

- MATLAB programming (scripting, function handling, subplots)
- Numerical solution of ODEs (`ode23`)
- Pharmacokinetic modeling (one‑compartment, IV bolus)
- Data visualization (linear vs. semilog scales, subplots, grid)
- Code clarity (parameter definition, comments)

## How to Run

1. Ensure the function `WK3_one_compartment2` (which defines the ODE) is in your MATLAB path or in the same folder.  
   *(If you don’t have it, you can create a local function as shown below.)*
2. Open the script `OneComp_IVBolus.m` in MATLAB.
3. Click **Run** or type the filename in the Command Window.
4. Modify parameters (`D`, `CL`, `V`) at the top to explore different scenarios.


