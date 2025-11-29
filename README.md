# Soil Moisture Estimation

### Authors

-  Artur Heimola 
-  Kert Moistt 
-  Kaur Kullamäe 

---

##  Motivation & Goal

Soil moisture is an important variable for agriculture, climate research, and environmental monitoring. Estonia has limited direct soil-moisture measurements, therefore we use European ISMN (International Soil Moisture Network) data to train models capable of estimating soil moisture for Estonia.

Our goals:

- Use European ISMN datasets as training data  
- Filter countries that include precipitation and air temperature measurements  
- Train a model:  
  - Random Forest Regressor  
- Obtain daily precipitation and temperature data for Estonia  
- Generate daily soil moisture estimates for Estonia  
- Compute daily averages to reduce noise and data volume  
- Compare model accuracy and document results  

---

## Repository Structure 

```

├── README.md                     # Project overview, instructions, authors
├── requirements.txt              # Python dependencies

├── data/
│   ├── raw/                      # Raw ISMN data
│   ├── estonia/                  # Estonian weather data (precipitation + temperature)
│   └── README.md                 # Data source explanations

├── notebooks/
│   ├── ISMN_data.ipynb
│   ├── main.ipynb

└── results/
    ├── predictions/              # Soil moisture predictions for Estonia
    ├── plots/                    # Generated figures and graphs

```

## How to Reproduce the Analysis

To fully reproduce the soil-moisture estimation workflow, follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/MedvedEE/IDS2025_B7.git
```

### 2. Install Dependencies

```
pip install -r requirements.txt

```

### 3. Prepare the Data

#### 1. Download ISMN soil moisture data and place it in:

```
data/raw/
```

#### 2. Add Estonian precipitation + temperature datasets to: 
```
data/estonia/
```

####  3. Run the Notebooks

* Run the notebooks in:

```
notebooks/
```

### 4. View outplut plots

Figures: ``` results/plots```


