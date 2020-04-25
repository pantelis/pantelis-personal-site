+++
# A Projects section created with the Portfolio widget.
widget = "portfolio"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 91  # Order that this section will appear.

title = "Projects"
subtitle = ""

[content]
  # Page type to display. E.g. project.
  page_type = "project"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  filter_default = 0
  
  # [[content.filter_button]]
  #   name = "All"
  #   tag = "*"
  
  # [[content.filter_button]]
  #   name = "Deep Learning"
  #   tag = "Deep Learning"
  
  # [[content.filter_button]]
  #   name = "Other"
  #   tag = "Demo"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view = 3

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false

[design.background]
  # Apply a background color, gradient, or image.
  #   Uncomment (by removing `#`) an option to apply it.
  #   Choose a light or dark text color by setting `text_color_light`.
  #   Any HTML color name or Hex value is valid.
  
  # Background color.
  # color = "navy"
  
  # Background gradient.
  # gradient_start = "DeepSkyBlue"
  # gradient_end = "SkyBlue"
  
  # Background image.
  # image = "background.jpg"  # Name of image in `static/img/`.
  # image_darken = 0.6  # Darken the image? Range 0-1 where 0 is transparent and 1 is opaque.

  # Text color (true=light or false=dark).
  # text_color_light = true  
  
[advanced]
 # Custom CSS. 
 css_style = ""
 
 # CSS class.
 css_class = ""
+++

All non-proprietary project code is in my [Github](https://github.com/pantelis). Wireless projects that include extensive NS-3 simulations are not there as they contain proprietary components and algorithms. 

### Computer Vision and Deep Learning

1. Multi-camera Real Time Object Detection. We developed an end to end video pipeline based on Tensorflow and streaming frameworks that can detect using Resnet-50 extracted feature maps various objects in real time. The pipeline was tested a large indoor space covered by tens of cameras.

2. Finding Lane Lines for autonomous vehicles. Various transformations were applied to calibrated video sequence to a histogram-based lane detection algorithm to detect and overlay a spline on traffic lane lines. The algorithm had real time requirements.

3. Traffic Sign Classifier for autonomous vehicles. A dataset of traffic signs was used to train a 5 layer deep CNN - the model was subsequently used to classify test traffic signs.

4. Behavioral Cloning for autonomous vehicles. The human behavior while driving a vehicle inside a simulated closed circuit, was cloned by a DNN successfully allowing the DNN to drive the vehicle in the same circuit.

5. Vehicle Detection and Tracking for autonomous vehicles. Vehicles present in a highway scene were searched, detected and bounding boxes plotted around them. SVM-based algorithms were used due to real-time constraints of the problem.

6. Semantic Segmentation. Transfer learning was implemented on Fully Convolutional Network. Starting from VGG16 the FCN16s architecture was implemented aiming to paint each pixel of a sequence of training images according to the desired class.

### Tracking and Optimal Control

1. Extended and Unscented Kalman Filters for Robots. In this project, EKF and UKF filters were used to estimate the state of a moving object of interest with noisy LIDAR and radar measurements.

2. Localization in Networks. In this project mobile devices were localized using traces of noisy and missing network data. Noting that devices were successfully localized without any explicit trigger to the specific device, the estimated locations help on troubleshooting operational networks, drive anomaly detection algorithms but also help law enforcement agencies to respond to terrorist attacks and other crimes.

3. Model Predictive Control for autonomous vehicles. In this project we optimized MPC parameters, based on a kinematic model of the car. The optimally manipulated variables such as steering and throttle minimize the cost a quadratic function of cross track error (CTE) as well as velocity deviations from a nominal velocity value over a horizon of several seconds.

### Resource Assignment Policy Design

1. Behavioral Cloning for Optimal Resource Assignment. In this project DNNs are used to approximate resource assignment algorithms. Accuracies of 98% have been achieved for simple policies and the work is on going for approximating complex policies.

2. Optimal Parameter Optimization in Networks. In this project series, network training datasets were used to learn interference patterns and the resultant statistics drive iterative structured optimization algorithms that maximize social utility for all network participants.

3. Economic Networks. In this project resource protection limits were derived for each class of users to adjust optimal priority levels that admit and/or define a classes of service.