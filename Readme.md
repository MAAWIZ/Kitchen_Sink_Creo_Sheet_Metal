# Kitchen Sink Sheet Metal CAD Model

## Project Overview
This repository contains the 3D CAD model of a Kitchen Sink, designed using sheet metal forming techniques in PTC Creo Parametric. The model is fully constrained and constructed strictly according to the specified Geometric Dimensioning and Tolerancing (GD&T) engineering drawings, focusing on precise sketched forms and extruded cuts.

## Software Used
* PTC Creo Parametric

## Design Specifications & Dimensions
The model's geometry is defined by the `Kitchen_Sink_GD&T.pdf` drawing. Key dimensions include:

* **Overall Footprint:** 1200 mm x 600 mm.
* **Material Thickness:** 0.1 mm.
* **Main Basin:** 600 mm x 420 mm.
    * Outer corner radii: R90.
    * Inner corner radii: R45.
* **Drain Hole:** Center circular cut with a diameter of Ø96 mm.
* **Drainage Grooves:** 5 vertical slots, each 330 mm in length, with edge offsets of 30 mm, 45 mm, and 60 mm.
* **Edge Treatments:** Specific filleting applied throughout, including R60, R30, R12, R0.1, and R0.05 radii.
* **Draft/Form Angles:** 45°, 15°, and 5° angles applied to the basin and lip forms.

## Modeling Workflow
The part was created utilizing a standard sheet metal top-down design methodology. The feature progression in the model tree is as follows:

1. **Planar 1 (First Wall):** The foundational base sheet defining the 1200x600 outer profile and 0.1 thickness.
2. **Sketched Form 1:** The primary punch/form feature establishing the 600x420 main sink basin and draft angles.
3. **Sketched Form 2:** The secondary form defining the raised outer perimeter lip of the sink.
4. **Sketched Form 3:** The patterned stamped grooves on the drainboard section (330 mm length slots).
5. **Extruded Cut 1:** The removal of material for the Ø96 mm center drain hole.
6. **Round 1 & Round 2:** Final application of edge fillets (such as R0.05 and R0.1) to smooth the formed transitions and remove sharp edges.

## Documentation
* `Kitchen_Sink_GD&T.pdf`: Contains the 2D dimensional drawing and tolerancing.
* `Kitchen_Sink_Gif.jpg`: Displays the final modeled part and the feature tree in the CAD environment.