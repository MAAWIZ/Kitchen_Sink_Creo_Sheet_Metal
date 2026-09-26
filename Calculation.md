# Kitchen Sink CAD Calculations

This document details the fundamental geometric and material calculations for the Kitchen Sink based on the provided GD&T dimensions.

## 1. Overall Footprint Area
The total bounding area of the flat sheet before deep drawing operations.

*   **Length ($L$)**: $1200 \text{ mm}$
*   **Width ($W$)**: $600 \text{ mm}$

$$ A_{total} = L \times W $$
$$ A_{total} = 1200 \text{ mm} \times 600 \text{ mm} = 720,000 \text{ mm}^2 = 0.72 \text{ m}^2 $$

## 2. Drain Hole Cutout Area
The area of the material removed for the central drain hole.

*   **Diameter ($D$)**: $96 \text{ mm}$
*   **Radius ($R$)**: $48 \text{ mm}$

$$ A_{drain} = \pi \times R^2 $$
$$ A_{drain} = \pi \times (48 \text{ mm})^2 \approx 7238.23 \text{ mm}^2 $$

## 3. Main Basin Footprint Area (Approximate)
Calculating the top rectangular footprint of the basin, accounting for the outer corner radii ($R90$).

*   **Basin Length ($l$)**: $600 \text{ mm}$
*   **Basin Width ($w$)**: $420 \text{ mm}$
*   **Corner Radius ($r_{corner}$)**: $90 \text{ mm}$

First, calculate the area of a sharp rectangle:
$$ A_{rect} = l \times w = 600 \text{ mm} \times 420 \text{ mm} = 252,000 \text{ mm}^2 $$

Next, calculate the area lost due to the four rounded corners:
$$ A_{corners\_lost} = 4 \times \left( r_{corner}^2 - \frac{\pi \times r_{corner}^2}{4} \right) $$
$$ A_{corners\_lost} = 4 \times \left( 90^2 - \frac{\pi \times 90^2}{4} \right) \approx 4 \times (8100 - 6361.73) \approx 6953.08 \text{ mm}^2 $$

**Total Basin Footprint Area**:
$$ A_{basin} = A_{rect} - A_{corners\_lost} $$
$$ A_{basin} \approx 252,000 - 6953.08 = 245,046.92 \text{ mm}^2 $$

## 4. Initial Blank Volume
The volume of the raw sheet metal before any stamping or extruding, based on the specified thickness.

*   **Thickness ($T$)**: $0.1 \text{ mm}$

$$ V_{blank} = A_{total} \times T $$
$$ V_{blank} = 720,000 \text{ mm}^2 \times 0.1 \text{ mm} = 72,000 \text{ mm}^3 $$

## 5. Estimated Mass
Assuming the sink is manufactured from standard 304 Stainless Steel (Density $\rho \approx 7.93 \text{ g/cm}^3$ or $0.00793 \text{ g/mm}^3$).

$$ Mass = V_{blank} \times \rho $$
$$ Mass = 72,000 \text{ mm}^3 \times 0.00793 \text{ g/mm}^3 \approx 570.96 \text{ grams} $$

*(Note: Actual mass will be slightly less due to the drain hole cutout and drainage groove material stretching/removal).*

---
**Author:** Mohammad Maawi Bin Mukarram