### Dataset Description

This dataset contains technical and categorical attributes describing different cars.
Each observation represents a car model, and the target variable (`price`) classifies it as *cheap* or *expensive*.

---

#### Feature Summary

| Feature | Description |
|----------|-------------|
| **aspiration** | Type of aspiration used in the engine. <br>• `std` = standard aspiration <br>• `turbo` = turbocharged |
| **enginelocation** | Position of the engine within the car (e.g., front or rear). |
| **carwidth** | Width of the car body, expressed in consistent measurement units. |
| **curbweight** | Total weight of the car without passengers or cargo. |
| **enginetype** | Type of engine configuration. <br>• `dohc` = dual overhead cam <br>• `dohcv` = dual overhead cam and valve <br>• `l` = L-shaped engine <br>• `ohc` = overhead cam <br>• `ohcf` = overhead cam and valve (type F) <br>• `ohcv` = overhead cam and valve <br>• `rotor` = rotary engine |
| **cylindernumber** | Number of cylinders in the engine (e.g., 3, 4, 6, 8, 12). |
| **stroke** | Distance traveled by the piston during one half-turn of the crankshaft. |
| **peakrpm** | Maximum revolutions per minute achieved by the engine. |
| **price** | Target variable — indicates whether the car is *expensive* or *cheap*. |

---

#### Notes
- The dataset contains both numerical and categorical variables suitable for feature scaling and encoding.
- Several features (e.g., `carwidth`, `enginetype`, `cylindernumber`) were used for data preprocessing and model training steps in the notebook.
