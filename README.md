
Content: tutorial on how to use eeglab and analyze the data.

### Project Name: **NeuroWave: EEG Data Analysis**

---

### Project Description

**NeuroWave** is a comprehensive analysis project focusing on the preprocessing and classification of EEG data to identify different types of brain activities. The project examines the effects of various neural, ocular, muscular, and artifactual components on EEG readings. Through systematic cleaning and analysis, the project aims to enhance the understanding of brain signals and their significance in biomedical robotics applications.

---

### Technical Details

1. **Data Overview**
   - **Total Epochs (Before Cleaning):** 1152
   - **Total Epochs (After Cleaning):** 1062
   - **Total Channels:** 52
   - **Channels Removed:** 4 (C6, T8, TP7, CP5)
   - **Total Epochs Removed:** 90

2. **Component Classification**
   - **Neural Components:** 1, 3, 4, 5, 7, 8, 10, 12, 14, 16, 17, 19, 20, 22, 23, 27, 29, 30, 32, 36, 38, 41, 42, 43, 44
   - **Ocular Components:** 2, 6, 9
   - **Muscular Components:** 18, 25, 26
   - **Artifactual Components:** 24, 28, 33, 34, 35, 37, 39, 40, 45, 46, 47, 48, 49, 50, 51, 52

3. **Frequency Analysis**
   - **Prominent Frequency:** 4-10 Hz
   - **Location of Activity:** Predominantly in neural components, indicating brain source activity.

---

### Implementation Details

1. **Data Acquisition**
   - EEG data was collected with a 52-channel setup, ensuring comprehensive coverage of brain activity.
   - Initial preprocessing involved segmenting the data into epochs for analysis.

2. **Manual Cleaning Process**
   - The cleaning process reduced the number of epochs from 1152 to 1062.
   - Channels C6, T8, TP7, and CP5 were removed due to poor signal quality or excessive noise.

3. **Component Identification**
   - Each component was analyzed using Independent Component Analysis (ICA) to classify them into neural, ocular, muscular, or artifactual.
   - For example:
     - **Neural Component:** Demonstrated a peak at 10 Hz, indicating active brain processes.
     - **Ocular Component:** Showed patterns of eye movements affecting the frontal lobe, with lower frequency power decreasing below 5 Hz.
     - **Muscular Component:** Exhibited high-frequency power (>20 Hz), highlighting muscle artifacts.
     - **Artifactual Component:** Displayed irregular activity, often resulting from external noise.

4. **Spectral Analysis**
   - The EEG data was subjected to Fourier Transform to identify the frequency spectrum.
   - Prominent frequencies (4-10 Hz) were correlated with neural activity, enhancing understanding of brain oscillations.

5. **Visualization**
   - Scalp topographies and power spectrum images were generated to visualize brain activity associated with different components.
   - These visualizations provide insight into the spatial distribution of activity across the scalp.

---

### Conclusion

The **NeuroWave** project effectively demonstrates the utility of EEG data analysis in biomedical robotics, providing valuable insights into brain function and potential applications in neurofeedback and brain-computer interfaces. By systematically cleaning and classifying EEG data, the project sets the foundation for future research and technological advancements in neurotechnology.
