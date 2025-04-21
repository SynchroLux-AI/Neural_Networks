
<h1> 🧠  $$\color{yellow}\text{Convolutional Neural Networks (CNNs) Models} $$</h1>
<!--h1>  🤯 🌟 </h1-->
<nav><ul>
    <li><a href="#what"> What Are CNNs? </a></li>
    <li><a href="#key"> Key Components of CNNs </a></li>
    <li><a href="#applications"> CNN Applications </a></li>
    <ul>
        <li><a href="#accelerator"> Accelerator Physics | Plasma Physics </a></li>
        <li><a href="#hep"> Particle Physics </a></li>        
        <li><a href="#gravy"> Gravitational Wave Physics </a></li>
    </ul>
    <li><a href="#sample"> An Exemplary CNN Model and Results </a></li>
  </ul></nav>

<h2 id="what">$$\color{yellow}\text{What Are CNNs?}$$ </h2>
Convolutional Neural Networks (CNNs), or ConvNets, are a specialized class of deep learning models designed to process grid-like data structures, such as images. Inspired by the human brain's visual processing system, CNNs excel at recognizing patterns and features in visual inputs, making them indispensable in fields like computer vision and beyond.

<h3 id="key"> Key Components of CNNs: </h3>
<ul>
<li><b>Convolutional Layer</b>: Extracts features using filters (kernels) that scan input data, identifying patterns like edges or textures.</li>

<li><b>Pooling Layer</b>: Reduces the spatial size of feature maps, retaining essential information while improving computational efficiency.</li>

<li><b>Fully Connected Layer</b>: Combines extracted features to make predictions or classifications.</li>

This architecture enables CNNs to progressively learn from simple patterns (lines, shapes) to complex ones (faces, objects).
</ul>

<h2 id="applications">$$\color{yellow}\text{Applications of CNNs}$$</h2>

<h3 id="accelerator">📌 Accelerator Physics | Plasma Physics </h3>
<ol type="1">
    
CNNs can accelerate detector simulations by generating realistic outputs for experimental setups. This is particularly useful for large-scale simulations required in HEP experiments.<br>

<li> Beam Dynamics Modeling </li>
CNNs can model charged particle beam dynamics by approximating dynamical systems with high precision. For example:

Physics-based Deep Neural Networks: These networks use symplectic regularization to ensure Hamiltonian system constraints, improving beam optics models and simulations for accelerators.

<li> Time Series Forecasting for Accelerator Control </li>
CNNs can process multivariate time-series data from sensors and monitors within accelerators to:
    <Ul>
    <li>Predict beam behavior and optimize control parameters.</li>
    <li>Enhance diagnostics and pre-emptive maintenance for complex facilities, ensuring operational stability.</li>
    <li>Predict beam behavior and optimize control parameters.</li>
    </Ul>
    
Enhance diagnostics and pre-emptive maintenance for complex facilities, ensuring operational stability.
<li>  Beam Diagnostics and Image Analysis </li>
    <ul>
        <li>Beam Shape Analysis: CNNs can process images of particle beams to determine their shape, size, and intensity distribution, which are critical for ensuring beam stability and quality.</li>
        <li>Anomaly Detection: CNNs can identify irregularities in beam profiles, such as distortions or instabilities, which may indicate equipment malfunctions or operational issues.</li>
    </ul>    
</ol>

<h3 id="hep">📌 High-Energy Physics </h3>
Convolutional Neural Networks (CNNs) are transforming collider physics experiments by enabling the classification of particle collision events through innovative approaches, such as representing physical variables like momenta and jets as image-like data. These methods have demonstrated competitive performance in tasks like signal-versus-background discrimination, offering new insights into high-energy physics data analysis.<br><br>

<ol type="1">    
<li><b>Particle Collision Classification:</b><br>
CNNs can classify particle collision events by converting physical variables (e.g., momenta of particles and jets) into image-like representations. This approach has been tested with data from collider experiments at LHC, demonstrating competitive performance compared to traditional methods like feedforward neural networks. </li><br>
    
<li><b>Noise Reduction and Particle Tracking:</b><br>
CNNs have been used for noise reduction and track identification in drift chamber data, such as in the BESIII experiment. They effectively filter noise, label individual particle tracks, classify charges, and recognize particle pairs based on features like track curvature and transverse momentum.</li><br>

<li><b>Jet Physics:</b><br>
CNNs, including specialized architectures like Particle Convolution Networks (PCNs), are applied to jet tagging tasks (e.g., quark/gluon tagging, top quark tagging). These models leverage symmetries such as rotation invariance in the jet axis plane to improve classification accuracy. </li><br>

<li><b>Fast Detector Simulations:</b><br>
CNNs can accelerate detector simulations by generating realistic outputs for experimental setups. This is particularly useful for large-scale simulations required in HEP experiments. </li>

</ol>

<h3 id="gravy">📌 Gravitational Wave Physics </h3>
<ol type="1">

  <li> Signal Detection and Noise Filtering: </li>
       CNNs can process raw gravitational wave data to detect signals buried in noise. Their ability to extract features from time-series or spectrogram-like data makes them ideal for identifying weak gravitational wave signals.

<li> Event Classification:</li>
     CNNs can classify gravitational wave events based on their source (e.g., black hole mergers or neutron star collisions). By analyzing waveform patterns, they help determine the astrophysical origin of detected waves.

<li>Parameter Estimation:</li>
    CNNs assist in estimating parameters such as mass, spin, and distance of gravitational wave sources by analyzing waveform features.

<li>Real-Time Data Analysis:</li>
    The speed of CNNs enables real-time detection and analysis of gravitational wave signals, supporting rapid follow-up observations with telescopes.
</ol>

<h2 id="why">$$\color{yellow}\text{Why Are CNNs So Powerful?}$$</h2>
CNNs leverage unique features like parameter sharing and local connectivity, allowing them to efficiently process high-dimensional data while maintaining spatial relationships. This makes them robust against variations in input data, such as changes in position, scale, or lighting.

<!--h3>A Glimpse into the Future:</h3>
As CNNs continue to evolve, they are being integrated with other AI technologies like Generative Adversarial Networks (GANs) and Recurrent Neural Networks (RNNs), unlocking new possibilities in creative industries, autonomous systems, and beyond. <-->

<h2 id="sample">$$\color{yellow}\text{An Exemplary CNN Model and Results}$$ </h2>

<h3>Model Construction</h3>
Divided into Filtering layers and Classification layers.

Filtering Layer: Use Conv2D and MaxPooling2D instead of Dense.

<b> Conv2D: </b>
<ul>
    <li> Number of filters </li>
    <li> Filter size </li>
    <li> Stride: Default = 1 </li>
</ul>

<b> MaxPooling2D: </b>
<ul>
    <li>Filter size</li>
    <li>Stride: Default = filter size</li>
</ul>

<b>model.summary():</b>
<ul>
    <li>Count the number of weights and analyze the model structure.</li>
    <li>Output Shape: Feature map dimensions</li>
    <li>Parameter No: Number of weights </li>
</ul>

<!--img src="./cnn_v1_plot_model.png" alt="CNN v1 Plot Model" style="width: 50%; height: auto;"-->
<a href='https://postimg.cc/G8CvxNZX' target='_blank'>
    <img src='https://i.postimg.cc/0Q6ZP1Z1/cnn-v1-plot-model.png' border='0' alt='cnn-v1-plot-model' style="width: 50%; height: auto;">
</a><br><br>

<a href='https://postimages.org/' target='_blank'>
    <img src='https://i.postimg.cc/YSTYNGNT/summary-1-cnn-v1.png' border='0' alt='summary-1-cnn-v1' style="width: 50%; height: auto;">
</a><br><br>

<b>Traninig with Cifar 10 datasets:</b><br>
<!--img src="./animals_cnn_v1.png" alt="Animal Pictures" style="width: 60%; height: auto;"-->
<a href='https://postimg.cc/LhsJF2Bz' target='_blank'>
    <img src='https://i.postimg.cc/05YDmNzH/animals-cnn-v1.png' border='0' alt='animals-cnn-v1'/>
</a><br><br>

<br><b>Accuracy vs. Epoch:</b><br>
<img src="./training_validation_accuracy.png" alt="CNN v1 Training_Validation_Accuracy" style="width: 60%; height: auto;">
<a href='https://postimages.org/' target='_blank'>
    <img src='https://i.postimg.cc/BQJDCGDZ/training-validation-accuracy.png' border='0' alt='training-validation-accuracy' style="width: 60%; height: auto;">
</a><br><br>

<br><b>Recall vs. Epoch:</b><br>
<!--img src="./recall_cnn.png" alt="CNN v1 Recall" style="width: 60%; height: auto;"-->
<a href='https://postimages.org/' target='_blank'>
    <img src='https://i.postimg.cc/Pr6LzvTK/recall-cnn.png' border='0' alt='recall-cnn' style="width: 60%; height: auto;">
</a>
