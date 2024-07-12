## Forest Fire Estimator Classification using Deep Learning

### Project Overview
This project aims to classify forest fires based on various environmental factors and indices using deep learning techniques. The classification problem involves categorizing the size of the fire into two categories: Small Fire and Wide Fire, based on the burned area.

### Problem Statement
- **Small Fire:** If the burned area (`area`) is less than 6 ha, it is labeled as 0.
- **Wide Fire:** If the burned area (`area`) is 6 ha or more, it is labeled as 1.

### Attribute Information
- **X:** x-axis spatial coordinate within the Montesinho park map (1 to 9)
- **Y:** y-axis spatial coordinate within the Montesinho park map (2 to 9)
- **month:** Month of the year ('jan' to 'dec')
- **day:** Day of the week ('mon' to 'sun')
- **FFMC:** Fine Fuel Moisture Code (FFMC) index from the FWI system (18.7 to 96.20)
- **DMC:** Duff Moisture Code (DMC) index from the FWI system (1.1 to 291.3)
- **DC:** Drought Code (DC) index from the FWI system (7.9 to 860.6)
- **ISI:** Initial Spread Index (ISI) index from the FWI system (0.0 to 56.10)
- **temp:** Temperature in Celsius degrees (2.2 to 33.30)
- **RH:** Relative humidity in % (15.0 to 100)
- **wind:** Wind speed in km/h (0.40 to 9.40)
- **rain:** Outside rain in mm/m² (0.0 to 6.4)
- **area:** The burned area of the forest (in ha) (0.00 to 1090.84)

### Tools and Libraries
- **Programming Language:** Python
- **Deep Learning Framework:** TensorFlow and Keras
- **Data Manipulation and Analysis:** NumPy, pandas
- **Data Visualization:** Matplotlib, Seaborn

### Deep Learning Model
The deep learning model is designed to classify the forest fire size. The model includes:
- Sequential layers of dense neurons.
- Activation functions to introduce non-linearity.
- Early stopping to prevent overfitting by monitoring validation loss and stopping training when the loss stops improving.
- Model checkpointing to save the best model during training.

### Results
- **Early Stopping:** Prevented overfitting by stopping training when the validation loss stopped improving.
- **Model Checkpointing:** Saved the best performing model during training.
- **Training Accuracy:** 1.000
- **Validation Accuracy:** 0.971

### Conclusion
This project successfully classified forest fire sizes using deep learning techniques. The implementation of early stopping and model checkpointing helped improve model performance and reliability.
