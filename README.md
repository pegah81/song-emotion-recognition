### Audio-Visual Emotion-Based Music Recommendation System
#### Abstract
This project combines music and facial expression analysis to create a personalized experience. Using the DEAM dataset, we apply machine learning to predict emotions from audio and facial features, developing a recommendation engine that syncs songs with the user's emotions for an immersive experience.

### Music Emotion Recognition (MER)
  * Audio Features: We analyze pitch, frequency, and amplitude to understand the emotional tone of music. These features are used to 
    construct spectrograms and mel-spectrograms, which serve as inputs for our deep learning models.

  * Deep Learning Models:
   * Convolutional Neural Networks (CNNs): Used to extract features from spectrograms for emotion classification.
   * CNN + LSTM Hybrid: Combines spatial feature extraction with temporal dependencies to better understand the emotional dynamics of songs.
    
 ### Face Emotion Recognition (FER)
  * Dataset: We use the Cohn-Kanade Dataset (CK+) for training facial emotion models.
  
  * Model Architecture: A CNN model is designed to classify seven basic emotions (anger, disgust, fear, happiness, sadness, surprise,   neutral) using real-time facial images extracted from video frames.
   
  * Real-Time Processing: The OpenCV library with Haar Cascade classifiers is employed for real-time face detection and emotion classification.



