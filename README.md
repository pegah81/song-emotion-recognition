## Audio-Visual Emotion-Based Music Recommendation System
### Abstract
This project combines music and facial expression analysis to create a personalized experience. Using the DEAM dataset, we apply machine learning to predict emotions from audio and facial features, developing a recommendation engine that syncs songs with the user's emotions for an immersive experience.

### Music Emotion Recognition (MER)
  * Audio Features: We analyze pitch, frequency, and amplitude to understand the emotional tone of music. These features are used to 
    construct spectrograms and mel-spectrograms, which serve as inputs for our deep learning models.

  * Deep Learning Models:
   * Convolutional Neural Networks (CNNs): Used to extract features from spectrograms for emotion classification.
   * CNN + LSTM Hybrid: Combines spatial feature extraction with temporal dependencies to better understand the emotional dynamics of songs.

<img src="https://github.com/user-attachments/assets/24beb873-06db-459e-b243-19eca975fea4" width="500" height="200"/>

    
 ### Face Emotion Recognition (FER)
  * Dataset: We use the Cohn-Kanade Dataset (CK+) for training facial emotion models.
  
  * Model Architecture: A CNN model is designed to classify seven basic emotions (anger, disgust, fear, happiness, sadness, surprise,   neutral) using real-time facial images extracted from video frames.
   
  * Real-Time Processing: The OpenCV library with Haar Cascade classifiers is employed for real-time face detection and emotion classification.

### Recommendation System
  * Integration: The final system integrates FER and MER. It uses real-time facial emotion data to recommend songs that match the user's current emotional state.
  
  * Methodology:
   * Observation Phase: The system monitors facial expressions for 15 seconds, quantifying emotions expressed during this period.
   * Recommendation Phase: Using cosine similarity, the system calculates the similarity between observed facial emotion vectors and song emotion vectors, recommending the top 5 matching songs.
### Results
 * MER Results: The use of mel-spectrograms with a simpler CNN model provided the best performance for emotion classification, achieving a F1 score of 0.59.
 
 * FER Results: The CNN model effectively classified facial emotions with a satisfactory accuracy using the CK+ dataset.
 
 * Overall System Performance: The integrated system successfully recommends songs that align with users' emotions, based on real-time facial expressions.

### Conclusion
This project demonstrates a successful fusion of audio and visual emotion recognition for a personalized music recommendation system. By leveraging deep learning techniques and integrating MER and FER, the system offers an immersive and emotionally resonant user experience.

