# Trojan-Horse-Traffic-Dataset-Analysis
The goal of this project is to understand how data mining can be used in the
real-world scenarios such as analyzing if network traffic is benign or malicious and other
IT security analysis procedures. The project consisted of a dataset that had to be
preprocessed and then used for various data mining models to analyze which model was
the best for the most accurate detection in Trojan data. In my findings, I discovered that
Random Forest was the best model with a 0.73 accuracy in detecting trojan data as the
model can handle this robust dataset.


Problem description. With today’s advance in technology cyber threats and malware
have become more prevalent. These trojans can be overlooked and deceive users as they
gain access to the connected devices exploiting their information. However, there are
ways that machine learning can be used to detect these trojan threats.


Review of publications Machine learning models can be used to improve accuracy of the
predictions such as using Recurrent Neural Networks (RNN) and Convolutional Neural
Networks(CNN) which according to research has achieved over 15% improvement in
accuracy of detecting these threats (Samia et al., 2024).
Machine learning techniques are being used in the detection of these trojan threats. As
Malware is fast growing it’s designed to infect a computer system with a “virus” by stealing
information or spying on the user. These trojan viruses are always evolving and there are
constantly new needs for virus detection software’s to combat them. Which machine
learning techniques can be used to help protect the systems as “Machine learning models
can be trained to classify the malware into infected execution and legitimate execution”
(Shhadat et al., 2020).
Additionally, artificial intelligence is now being used to help with trojan detection. There
are more ways that data is being obtained such as video data, social media posts, etc.
This increase in the data surface has caused an increase in trojan attacks. AI can used to
hack systems but can also be used to protect against attacks like these through anomaly
detection by evaluating what the deviation is from the normal baseline. By having these
analysis reports, there can be recommended security tools suggested (Budhathoki,
2025).


Software Tools. For Software tools I used Jupyter Notebook and Python scripts to clean
up the dataset through preprocessing. Then I used the same tools for creating the Data
Mining Models and the heatmap to test the predictions of the dataset.
Preprocessing. When reviewing this data set, I was challenged with how to clean this up
to remove problematic or errored data, make the analysis more efficient, and avoid as
many false positives or negatives as possible. For my first preprocessing technique. I
removed columns that had either blank or irrelevant data this took the columns from the
initial 85 columns down to 74 columns. Next in the techniques I got rid of missing or
broken data by removing rows with IP addresses that were blank or 0.0.0.0 which took the
rows from the initial 159733 down to 159706. Another technique I used was cleaning up
the columns to all be cohesive as the column names varied by having spaces in front of
the names. Last in techniques, I got rid of data that had infinite values and zeros which
took the rows from 159706 down to 140977.


Data mining process. For the data mining techniques, I used Logistic Regression,
Random Forest, and Support Vector Machine. I used Logistic Regression as this model is
used when the variable has two outcomes, and in this project case the outcomes would
be “Trojan” and “Benign”. Random Forest models are used when needing multiple
decision trees with large datasets with high dimension, this model works for this dataset
as the dataset was large and had various branches. Support Vector Machine model is
used for classification and regression tasks and trying to find the best hyperplane that
differentiates the classes in the data, which in this case would be the “Trojan” and
“Benign” data.
When looking at all three models: Logistic Regression, Random Forest, and Support
Vector Machine I analyzed the precision, recall, and F1 score for the initial prediction
results. For Logistic Regression the precision, recall, and f1 score for benign was 0.54,
0.53, and 0.5. For Trojan it was 0.56, 0.56, and 0.56. Overall, the model provided a 0.55
accuracy which means there is balanced performance between the Benign and Trojan
classes.
For Random Forest, the precision, recall, and f1 score for benign was 0.71, 0.75, and 0.73.
For Trojan it was 0.75, 0.71, and 0.73. Overall, the model provided 0.73 accuracy which is
a higher improvement than the Logistic Regression’s 0.55. This means compared to the
Logistic Regression model, the Random Forest model caught more in the data that was
missed.
Finally for Support Vector Machine Model, the precision, recall, and f1 score for benign was
0.50, 0.40, and 0.44. For Trojan it was 0.52, 0.62, and 0.56. Overall, the model provided a
0.51 accuracy which, compared to Logistic Regression’s 0.55 accuracy and Random
Forest’s 0.73 accuracy, is worse in detecting Trojans which means its missing most of the
malicious data. This was the weakest model out of the three and Random Forest was the
strongest model.


Results/Conclusion.
When analyzing the models and creating a visualization chart to showcase the differences,
I found that Random Forest was the best model in accuracy of catching malicious data. The
heat map created shows the three models compared and Random Forest was at the
darkest blue of the heat map, then Logistic Regression being somewhat in the lower middle
of the heat map with the light green, and Support Vector Machine being last on the heat
map with the pale yellow. Random Forest better preformed due to the model’s ability to
handle non-linear patterns, features, and outliers with use of decision trees. The Logistic
Regression model is linear and is unable to separate the Trojan and Benign Data which is
why it wasn’t the best model for this dataset. Finally, the Support Machine Vector model
was not the best model because while it can be non-linear, it is affected by the scaling of
data which means it misclassified some of the data which lowered the accuracy. Thus,
Random Forest is the best model for the dataset.


References.
• Budhathoki, N. (2025, August 1). The role that AI and Machine Learning plays in
Cybersecurity. DSS Blog. https://roundtable.datascience.salon/the-role-that-ai-
and-machine-learning-plays-in-
cybersecurity?gad_source=1&gad_campaignid=22114556059&gbraid=0AAAAA-
Q8n0vt8RnrB4npnd8ayuWY-
LOXg&gclid=CjwKCAjwpOfHBhAxEiwAm1SwEmKRFE5p5CqiHwHXCrEK9NH7-
xWnaL7Av6Uvv4X0RAdgYNlT6K_yAhoCP_sQAvD_BwE
• Shhadat, I., Bataineh, B., Hayajneh, A., & Al-Sharif, Z. A. (2020). The use of machine
learning techniques to advance the detection and classification of unknown
malware. Procedia Computer Science, 170, 917–922.
https://doi.org/10.1016/j.procs.2020.03.110
• Samia, N., Saha, S., & Haque, A. (2024). Predicting and mitigating cyber threats
through Data Mining and machine learning. Computer Communications, 228,
107949. https://doi.org/10.1016/j.comcom.2024.107949
• Merriam-Webster. (n.d.). Fraud definition & meaning. 
