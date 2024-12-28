# PRODIGY_ML_TASK-05
Key Steps and Features:
Calorie Data Loading:

Reads a CSV file containing food_item names and their respective calories.
Preprocesses the data by normalizing food item names (lowercasing and trimming).
Stores the calorie information in a dictionary for quick lookups.
Dataset Loading and Preprocessing:

Loads food images from a directory structured by food categories (e.g., pizza, burger).
Resizes images to 64x64 pixels and normalizes pixel values to [0, 1].
Assigns numeric labels to each food category and creates a label-to-category mapping.
Pre-trained Model Setup:

Uses MobileNetV2 as the base model (with pre-trained ImageNet weights).
Freezes the base layers and adds a custom dense head for classification.
Optimized with Adam optimizer and trained using sparse categorical cross-entropy loss.
Model Training:

Augments training images using random transformations like rotation, zoom, and flips.
Trains the model for 10 epochs with an 80-20 train-test split.
Prediction and Visualization:

Predicts the food category for a given image and retrieves its calorie count.
Displays the original image with the predicted food item and calorie information.
Model Saving:

Saves the trained model as a .h5 file for future use
