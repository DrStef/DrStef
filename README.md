
## **Machine Learning - Deep Learning Projects**


###  **Advanced projects**
This section contains Research and Development projects in Machine Learning and Deep Learning that require original developments. They call on our expertise in Digital Signal Processing, Optimization, Calculus, Linear Algebra. <br>

- #### <ul>[Deep Learning and Digital Signal Processing for Environmental Sound Classification (supervised)](https://github.com/DrStef/Deep-Learning-and-Digital-Signal-Processing-for-Environmental-Sound-Classification/blob/main/README.md) </ul>
<ul><ul>
 <img src="https://github.com/DrStef/Deep-Learning-and-Digital-Signal-Processing-for-Environmental-Sound-Classification/blob/main/esc10_sound_classification/docs/figures/esc10_v23_100pc.png"  align="right"  width="200px"/>
 <br>
 <img src="https://github.com/DrStef/Deep-Learning-and-Digital-Signal-Processing-for-Environmental-Sound-Classification/blob/main/esc10_sound_classification/docs/figures/MelSpectrogram.png"  align="right"  width="200px"/>
 <ul></ul>


Automatic Environmental Sound Classification (ESC) leverages the ESC-50 dataset (and its ESC-10 subset) developed by Karol Piczak, as detailed in his paper titled: 
<b><i> "ESC: Dataset for Environmental Sound Classification." </i></b> by Karol J. Piczak. 2015. In Proceedings of the 23rd ACM international conference on Multimedia (MM '15). Association for Computing Machinery, New York, NY, USA, 1015–1018. https://doi.org/10.1145/2733373.2806390" 
<br clear="left"/> <br>
This dataset serves as a foundation for research in audio event recognition. 

Advancements in ESC Using Multi-Feature CNNs:

We propose a two-stages classification approach with Multi-feature Convolutional Neural Networks (CNNs), achieving near-perfect accuracy rates, specifically reaching up to 99%. This high accuracy is attributed to innovative pre-processing techniques that combine mel-spectrograms with complex wavelet transforms (CWT).

Resolution of Remaining Classification Challenges:

A notable challenge in ESC-10 sound classification was the confusion between "sea waves" and "rain" sounds. This issue was addressed by developing an original transformation of the complex CWT, termed <i>aT-CWT</i>. This transformation replaces the phase component of the CWT for stationary and pseudo-stationary sounds with a Gaussian distribution, enhancing the model's ability to differentiate between similar sounding environmental events. <br>
By integrating the <i>aT-CWT</i> transformation, the multi-feature CNN model has now achieved 100% accuracy in classifying environmental sounds from the ESC-10 dataset. 

</ul></ul>

- #### <ul>[Unsupervised anomalous sound detection for machine condition monitoring](https://github.com/DrStef/MIMII/blob/main/README.md)</ul>

<ul><ul>
We developed an unsupervised classification model for detecting valve faults in industrial machinery using acoustic signals from an 8-microphone array, based on the MIMII dataset (CC BY-SA 4.0, Hitachi, Ltd., https://zenodo.org/records/3384388). <br>
We introduced a novel ACSTFT transform, achieving an ROC AUC of 0.99 on the +6dB valve dataset, and trained a CNN-Autoencoder for robust anomaly detection. <br>
By denoising multi-channel signals with MVDR beamforming and a custom Generalized Sidelobe Canceler (GSC), the model transforms the array into a noise-robust "sensor." Focused on valves, it classifies single-microphone and denoised GSC outputs to identify defects, enhancing fault detection in noisy environments. View project

 
 |<p align="center">   <img src="https://github.com/DrStef/MIMII-Unsupervised-classification-of-valve-sounds/blob/main/results/plot/acstft_magnitude_spectrograms_1p5s_July03_v08.png"  width="150"  />  </p>    |  <p align="center"> <img src="https://github.com/DrStef/MIMII-Unsupervised-classification-of-valve-sounds/blob/main/results/plot/id04_ModelACSTFT_seed42_RocAuc_v01.png" width="200"  /> </p> | <p align="center"> <img src= "https://github.com/DrStef/MIMII-Unsupervised-classification-of-valve-sounds/blob/main/results/plot/id04_ModelACSTFT_seed42_MSE_v01.png"  width="200" /></p>|
| ---       | ---                          |   ---         |
 |<p align="center"> <sub><b> <i> ACSTFT Magnitude </i> </b> </sub>  </p>  |  <p align="center"> <sub><b><i> ROC-AUC= 0.99 <br> Single Type Valve id_04  </i> </b> </sub>  </p>       |   <p align="center"> <sub><b><i> Reconstruction error (MSE)  </i></b> </sub>  </p> |




[old] We develop an automatic unsupervised classification model or automatic diagnosis model for detecting failures or breakdowns of industrial machinery based on their acoustics characteristics, recorded with a 8-microphones circular array. 
       
The model is based on the MIMII dataset made available by Hitachi, Ltd. under a Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0) license. <br>
https://zenodo.org/records/3384388

Unlike most classification models found in literature, this study somewhat deviates from the initial challenge's rules: classification of noisy signals. However, since we have access to multiple channels, it makes practical sense to denoise the signals before initiating the classification process.
Thus, the challenge here is transforming the 8-microphone array into a <b>"sensor" for monitoring industrial machinery sounds in noisy environments</b>. Then, we apply the classification model to these denoised signals to automatically identify anomalies, failures, or breakdowns.

Rather than classifying various types of machines (pumps, fans, valves, sliders), our focus will be:
- Concentrating on a specific machine type: valves.
- Denoising the recordings using MVDR beamforming combined with a custom, fixed Generalized Sidelobe Canceler (GSC).
- Applying unsupervised classification techniques (auto-encoder, etc.) to two sets of signals: single microphone recordings and the denoised GSC output, to detect defective valves and demonstrate the benefits of MVDR beamforming combined with GSC.
 
<br>
<b> Applications </b>  <br>
- <b> Rotating machinery </b> Failure Detection: bearings, motors,rotors.  <br>
- <b> HVAC </b> Fault detection and diagnosis (FDD): pumps, compressors, valves.   
</ul></ul>

<!--  <img src="https://github.com/DrStef/MIMII/blob/main/Beampattern_1000Hz.png"  align="right"  width="250px"/>
  <br>
 <img src="https://github.com/DrStef/MIMII/blob/main/MIMII_Microphone_array.png"  align="right"  width="200px"/>  -->


</ul></ul>

- #### <ul>[Machine Learning and Digital Signal Processing for Genome Classification (supervised)](https://github.com/DrStef/Machine-Learning-and-Digital-Signal-Processing-for-Genome-Classification/blob/main/README.md) </ul>
<ul><ul>

<img src="https://github.com/DrStef/Machine-Learning-and-Digital-Signal-Processing-for-Genome-Classification/blob/main/LOG_REG_Fungi_ConfusionMatrix.png"  align="right"  width="200px"/>
<br>
<img src="https://github.com/DrStef/Machine-Learning-and-Digital-Signal-Processing-for-Genome-Classification/blob/main/SVM_Bird_Fish_Mammal_Classification.png"  align="right"  width="300px"/>

In this project, we are developing effective methods for classifying mitochondrial genomes (DNA sequences) using Digital Signal Processing (DSP), Machine Learning (ML), and Deep Learning (DL). This research is ongoing, and we plan to publish our results regularly. As a starting point, we analyzed the paper titled: <br>
 <i><b> "ML-DSP: Machine Learning with Digital Signal Processing for ultrafast, accurate, and scalable genome classification at all taxonomic levels" </b></i> by Gurjit S. Randhawa , Kathleen A. Hill and Lila Kari. https://doi.org/10.1186/s12864-019-5571-y
<br><br>
The alignment-free DNA sequence classification approach: <i>ML-DSP</i>, proposed by Gurjit S. Randhawa has proven to be very effective. <br>  By introducing a simple alignment technique alongside short Fast Fourier Transforms (FFTs), termed <i>ML-FFT + SoftAlign</i>, we have surpassed the performance of <i>ML-DSP</i>, particularly with challenging datasets such as those from Fungi and Insects.

 </ul></ul>

- #### <ul>Deep Learning and Digital Signal Processing: Voice Activity Detection (VAD)</ul>

- #### <ul>Machine Learning and Digital Signal Processing: Sound Source Localization (SSL)</ul>



<br>
<br>

### **Standard projects**
  
This section is a portfolio of Machine Learning projects with Python and various visualization and analysis tools. Most of these projects were carried out within the framework of IBM certifications. They are presented with Jupyter Notebooks. <br>
Some projects have been improved by incorporating more in-depth data analysis, better graphs, advanced ML techniques. 

- #### <ul> [SpaceX Falcon 9 First Stage Landing Prediction](https://github.com/DrStef/Applied_Data_Science_Capstone_SpaceX_IBM/blob/main/README.md) </ul>      
<ul><ul> <img src="https://github.com/DrStef/Applied_Data_Science_Capstone_SpaceX_IBM/blob/main/spacex-MEW1f-yu2KI-unsplash.jpg"  align="right"  width="200px"/>
In this project, we predict if the Falcon 9 first stage will land successfully. Project includes: SpaceX data collection, Data Wrangling, Webscraping,  EDA with SQL Queries & Data visualization, SpaceX Launch Records Dashboard, Launch Sites Locations Analysis with Folium, Machine Learning classification with optimization of hyperparameters and selection of best model: KNN, Decision Tree, SVM, Logistic Regression. </ul></ul>

 
- #### <ul> [**Machine Learning with Python - (IBM Data Science Certificate)**](https://github.com/DrStef/Machine_Learning_with_Python-IBM/blob/main/README.md)

 <ul><ul><img src="https://github.com/DrStef/Machine_Learning_with_Python-IBM/blob/main/density_based_clustering_weather_001.png"  align="right"  width="200px"/>
A widerange of small projects with various ML techniques, prediction, supervised and unsupervised classification: Linear Regression, Polynomial Regression, Non-Linear Regression, Recommandation Systems, KNN, Customer Segmentation with K-Means, Hierarchical Clustering, Density-Based Clustering, Logistic Regression. </ul></ul>

 
- #### <ul> [House sales in King County USA (IBM Course - Data Analysis with Python)](https://github.com/DrStef/House_Sales_in_King_County_USA_IBM/blob/main/README.md) </ul>   
 
<ul><ul>
<img src="https://github.com/DrStef/House_Sales_in_King_County_USA_IBM/blob/main/Project_House_Sales_in_King_County_USA_v003_LTX/output_60_0.png"  align="right"  width="200px"/> 
The project consists of finding the best model for predicting home prices in King County, USA in Washington State, based on a dataset of homes sold between May 2014 and May 2015. Prediction accuracy was improved by implementing a spline regression model.<br>  One Jupyter Notebook includes interactive Folium maps (interactive maps will not display on Github). </ul></ul>
<br> 
 
- #### <ul> [Loan status prediction using Classification Algorithms - (IBM Data Science certificate)](https://github.com/DrStef/Loan-Status-Prediction-using-Classification-Algorithms_IBM/blob/main/README.md)</ul> 
  
<ul><ul><img src="https://github.com/DrStef/Loan-Status-Prediction-using-Classification-Algorithms_IBM/blob/main/Loan_gender.png"  align="right"  width="200px"/> 
Loan Status Prediction using Supervised Classification Algorithms: KNN, Decision Tree, SVM, Logistic Regression.</ul> </ul> 

<br>

## **Data Analysis**

- #### <ul> [Insights in Boston real estate - Statistical analysis](https://github.com/DrStef/Statistics-for-Data-Science-with-Python/blob/main/README.md)    </ul>
    
<ul><ul><img src="https://github.com/DrStef/Statistics-for-Data-Science-with-Python/blob/main/real_estate_boston_001.png"  align="right"  width="200px"/> 
Old dataset on housing prices derived from the U.S. Census Service to present insights based on our experience in Statistics. Median value of houses bounded by the Charles river, of owner-occupied units built before 1940, relationship between Nitric oxide concentrations and the proportion of non-retail business acres per town, impact of weighted distance to the five Boston employment centres on the median value of owner-occupied homes. </ul> </ul> 
 
- #### <ul> [Data Analysis with Python](https://github.com/DrStef/Data-Analysis-with-Python/blob/main/README.md) </ul>

<ul><ul><img src="https://github.com/DrStef/Data-Analysis-with-Python/blob/main/Data_Analysis_Python_003.png"  align="right"  width="200px"/> 
<br>
Dataset: car dataset including various makes, specifications and prices. <br>
After cleaning the dataset, running statistics, identifying the most relevant variables, we develop several models that will predict the price of a car using a set of features/variables.   </ul> </ul> 
<br clear="left"/> 
 
- #### <ul> [Data Visualization with Python](https://github.com/DrStef/Data-Visualization-with-Python/blob/main/README.md)</ul>

<ul><ul> 
 
 |<p align="center">   <img src="https://github.com/DrStef/Data-Visualization-with-Python/blob/main/Canada_immigration_wordcloud.png"  width="150"  />                        </p>    |  <p align="center"> <img src="https://github.com/DrStef/Data-Visualization-with-Python/blob/main/Crime_SF_folium_v02.png" width="200"  /> </p> | <p align="center"> <img src= "https://github.com/DrStef/Data-Visualization-with-Python/blob/main/Choropleth_can_immigration.png" width="200" /></p>|
| ---       | ---                          |   ---         |
 |<p align="center"> <sub><b> <i> Word Cloud </i> </b> </sub>  </p>  |  <p align="center"> <sub><b><i> Folium with markers </i> </b> </sub>  </p>       |   <p align="center"> <sub><b><i> Choropleth </i></b> </sub>  </p> |

 </ul></ul>
 
- #### <ul> **Databases and SQL for Data Science**</ul> 

- #### <ul> **Stock extraction \& vizualisation - yFinance, Webscraping**</ul> 
  

<br>
<br>
 
## **Digital Signal Processing**

 - #### <ul> **Microphone Array - Beamforming** </ul> 
 - #### <ul> **6 microphones circular array - Generalized Sidelobe Canceller (GSC) - Validation**   </ul>
 - #### <ul> [**Binaural Beamforming - Generalized Sidelobe Canceller (GSC) - Validation**](https://github.com/DrStef/Binaural_Beamforming/blob/main/README.md)</ul>
 - #### <ul> **A few words about complex wavelet transforms**   </ul>
 
<br>

 
## **Modeling and Scientific Computing**
<br>

- #### <ul>**Integral equation - Boundary Elements Method (BEM)**</ul> 
 
- #### <ul> [**Electroacoustics - Simulations**](https://github.com/DrStef/Electroacoustics/blob/main/README.md) </ul> 
 
- #### <ul> [**Discrete optimization: Genetic Algorithms - Bin-packing**](https://github.com/DrStef/Discrete-Optimization/blob/main/README.md)</ul> 
 
- #### <ul> [**Matplotlib - 3D surfaces**](https://github.com/DrStef/Complex-3D-surfaces-with-Matplotlib/blob/main/README.md)</ul> 
 
 <ul><ul> 
 
| <p align="center"> <img src= "https://github.com/DrStef/Complex-3D-surfaces-with-Matplotlib/blob/main/Fig8_torus03.png" width="150" /></p>                            |<p align="center">   <img src="https://github.com/DrStef/Complex-3D-surfaces-with-Matplotlib/blob/main/Gyroid.png"  width="150"  />                        </p>    |  <p align="center"> <img src="https://github.com/DrStef/Complex-3D-surfaces-with-Matplotlib/blob/main/Poly_002.png" width="150"  /> </p> | <p align="center"> <img src= "https://github.com/DrStef/Complex-3D-surfaces-with-Matplotlib/blob/main/Helicoid_Catenoid_v3.gif" width="150" /></p>|
| ---     | ---   | ---   |   ---    |
  |  <p align="center">  <sub><b> <i>  "Figure 8" toroid </i> </b> </sub>     </p>               |<p align="center"> <sub><b> <i>  Gyroid </i>  </b> </sub>  </p>  |  <p align="center">  <sub><b><i> Truncated cuboctahedron </i></b> </sub>   </p>       |   <p align="center">  <sub><b> <i> Helicoid-Catenoid </i></b> </sub>  </p> |

 </ul></ul>
 

- #### <ul> **Linear Algebra problems**   </ul>   
<br>
<br>
<br>  

  
🔭 I’m currently working on advanced projects in ML & DL <br>
👯 I’m looking to collaborate on Digital Signal Processing, Machine Learning, Deep Learning <br>
📫 How to reach me: <i>stephane.dedieu@bloo-audio.com</i> <br>
 

<!--
**DrStef/DrStef** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on advanced projects in ML & DL. 
- 🌱 I’m currently learning Tensorflow
- 👯 I’m looking to collaborate on Digital Signal Processing, Machine Learning, Deep Learning
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: <i>stephane.dedieu@bloo-audio.com</i>
- ⚡ Hobbies: stock market, economics, geopolitics.
- ⚡ Fun fact: ...

Modeling is the process that formalizes a concrete problem in mathematical terms accessible to analysis and numerical calculation.

Scientific computing is the interdisciplinary field that brings together the methods and algorithms for performing, using computers, numerical simulations based on a scientific approach. Most models involve equations (differential or partial derivatives) too complicated to be solved by elementary methods or using computer algebra techniques. Scientific computing proposes to give approximate numerical solutions to these models. The development of scientific computing is linked to the regular increase in the power of computers. It is therefore a constantly evolving sector.

Companies that use and develop modeling and scientific computing range from large state-owned or private companies responsible for designing and developing complex systems to small companies or start-ups specializing in software development. They operate in all sectors of activity: aeronautics and space, energy and environment, automotive, services and telecommunications, civil engineering. Reserved for the upstream dimensioning and verification of complex systems until recently, digital simulation has become widespread because it saves significant time on the design and production cycles of more elementary new products. Very often the design of an object or a system responding to general specifications is formalized as a constrained optimization problem. Modeling and scientific computing are therefore very often used in combination with optimization methods
