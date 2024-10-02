# Brain-Tumor
Brain tumors represent a significant challenge in the medical field due to their diverse types and complex presentation. Accurate and timely detection of brain tumors is crucial for effective treatment planning and improving patient prognosis. Traditionally, brain tumor diagnosis relies on manual interpretation of MRI scans by radiologists, which can be time-consuming and prone to variability. To address these challenges, there is a growing interest in leveraging advanced computational techniques for automated and accurate tumor detection and classification. Recent advancements in deep learning have shown promise in medical imaging analysis. Among these techniques, Long Short-Term Memory (LSTM) networks, a specialized type of recurrent neural network, have demonstrated significant potential in handling sequential data and learning long-range dependencies.
We got overall Accuracy 95%


Proposed Methodology:

Data Collection and Preprocessing:
Gather images of brain tumors categorized into folders (glioma, meningioma, pituitary, no tumor). Load and normalize images (scale pixel values to [0, 1]) and reshape them to fit the LSTM input format.
Label Mapping:
Create a mapping to convert tumor type names into numerical labels:
Glioma: 0, Meningioma: 1, No Tumor: 2, Pituitary: 3.
Data Splitting:
Split the dataset into training (80%) and testing (20%) subsets for model evaluation.
Model Development:
Build a Sequential LSTM model with:
An LSTM layer (64 units) followed by Dropout and Dense layer.
Model Training and Evaluation:
Compile the model using the Adam optimizer and train it for 200 epochs. Evaluate its performance on the test set by calculating loss and accuracy.
Prediction and Analysis:
Implement functions to predict tumor types for individual images and analyze a directory of test images, generating classifications based on the trained model.
