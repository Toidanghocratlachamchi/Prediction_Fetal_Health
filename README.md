# Prediction_Fetal_Health
Fetal Health Classification Using Apache Spark and FastAPI
## Problem Statement
The project aims to develop a machine learning model that can accurately classify fetal health into three categories: Normal, Suspect, and Pathological, using cardiotocograms. These classifications can help healthcare professionals take necessary preventative actions to ensure the health of both mother and baby. The machine learning model will be wrapped within a web service that is containerized for consistency across different deployment environments.

## Tools and Technologies:
This project leverages the following tools and technologies:
1. **Apache Spark:** A powerful open-source unified analytics engine for large-scale data processing and machine learning. Spark's in-memory computation capabilities make it an excellent choice for this project.
2. **FastAPI:** A modern, high-performance web framework for building APIs with Python 3.6+, used here to create the web service for the model.
3. **Docker:** A platform that enables developers to automate the deployment, scaling, and management of applications within containers.
4. **ngrok:** A tool used to expose the local server behind a NAT or firewall to the internet, allowing the FastAPI application to be accessed via a public URL.

## Methodology
**Dataset Description:**
The United Nations anticipates that by 2030, countries will put an end to avoidable deaths of newborns and children under the age of 5. All nations are encouraged to aim for reducing the mortality rate for children under 5 to a minimum of 25 per 1,000 live births.
Maternal mortality, which refers to the number of deaths during and after pregnancy and childbirth, is closely related to child mortality. As of 2017, it accounted for 295,000 deaths. The majority of these deaths (94%) occurred in regions with limited resources and could have been prevented.
Considering the information mentioned above, Cardiotocograms (CTGs) provide a straightforward and affordable method to evaluate the health of the fetus. They enable healthcare professionals to take appropriate measures to prevent both child and maternal mortality. CTG equipment operates by emitting ultrasound pulses and analyzing their response, thus providing insights into the fetal heart rate (FHR), fetal movements, uterine contractions, and other relevant factors.
The "Fetal Health Classification" dataset used in this project consists of measurements taken from cardiotocograms, which are a simple and cost-accessible option to assess fetal health. The dataset includes 22 features such as 'baseline value', 'accelerations', 'fetal_movement', 'uterine_contractions', 'light_decelerations', etc., and a target variable that represents the three classes of fetal health.

## Model Selection:
We experimented with several different models to find the one that offered the best performance. The performance of each model was evaluated based on its accuracy on the test data - the proportion of test data points that the model correctly classified. This iterative process involved training a model, evaluating its performance, adjusting its parameters to improve its accuracy, and repeating this process until the model's performance was satisfactory.

## Model Performance Enhancement:
One of the primary areas of focus for future improvement is undoubtedly the model's performance. While the current model provides satisfactory results, there are always ways to further improve its accuracy and reliability. This could be achieved by exploring and implementing more advanced machine learning algorithms. For instance, ensemble methods like Random Forests, Gradient Boosting, and XGBoost could potentially deliver improved results. 
Moreover, deep learning techniques, which have shown remarkable performance in various complex prediction tasks, could also be explored. Neural networks, especially Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs), could potentially enhance the model's ability to recognize intricate patterns in the data and provide more accurate predictions. 
- Explore advanced machine learning algorithms
- Implement ensemble methods
- Experiment with deep learning techniques
- Use neural networks for intricate pattern recognition

## User Interface Improvement:
Another crucial area for future improvement is the user interface of the application. Although the current interface is user-friendly and straightforward, making it more interactive and visually appealing could significantly improve the user experience. 
This could include adding visual elements like graphs and charts to help users understand the input data and the predictions better. Integrating interactive features that guide users through the process of entering data and understanding the results can also make the application more engaging and easy to use.
- Enhance visual appeal with graphs and charts
- Incorporate interactive features for better user engagement
- Improve user guidance throughout data entry and result interpretation


## Application Extension:
Lastly, the scope of the application could be extended to handle other types of health-related data and make additional predictions. This expansion could transform the application into a more comprehensive healthcare prediction tool. 
For instance, it could be adapted to predict other health conditions based on different types of medical data, such as blood test results or medical imaging data. This extension would require incorporating new datasets, training new models, and potentially integrating more sophisticated data processing techniques to handle different types of data.
- Expand the scope to handle various health-related data
- Adapt the model for predicting different health conditions
- Incorporate new datasets and train new models
By continuously refining and expanding this project, we can ensure that it remains at the cutting edge of technology, delivering the most accurate predictions and the best possible user experience.
