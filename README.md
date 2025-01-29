Dengue Haemorrhagic Fever (DHF) poses a significant public health challenge, especially in regions where the Aedes mosquito acts as a vector for the dengue virus. Accurate classification of DHF stages is crucial for tailored clinical management. In this paper, we introduce a novel framework that leverages Support Vector Machine (SVM) and Random Forest algorithms for categorizing DHF patients into three distinct stages: Early Febrile, Critical, and Recovery. The swift and precise identification of these stages is essential for ensuring timely and appropriate medical interventions, ultimately leading to improved patient outcomes. SVM and Random Forest are chosen for their proficiency in handling complex data, and through rigorous feature engineering and data preprocessing, we extract critical information for precise discrimination between DHF phases. SVM and Random Forest were selected for their ability to handle complex clinical data effectively, and through meticulous feature engineering and data preprocessing, we extracted critical information necessary for accurate discrimination between DHF phases.  Experimental results demonstrate the effectiveness of our framework in classification, offering a data-driven approach to DHF management, with potential profound implications for public health, particularly in regions prone to recurrent dengue outbreaks.

Algorithmic Approaches
i.	Support Vector Machine (SVM): 
![image](https://github.com/user-attachments/assets/260e9d2b-7c84-40f3-85b4-22a2dc0665d3)

  Figure represents the SVM which is a powerful algorithm used for binary and multiclass classification tasks. In our research, SVM was employed to classify DHF cases into the predefined stages of Early Febrile, Critical, and Recovery. SVM maximizes the margin between different classes, offering robust classification results. Parameters were tuned through cross-validation to optimize SVM's performance.
 
Figure 2: SVM Algorithm 
ii.	Random Forest 
![image](https://github.com/user-attachments/assets/fee4f6be-74d7-4d6a-a003-783043207908)

  Figure represents the Random Forest which is an ensemble learning algorithm that leverages the strength of decision trees. It is well-suited for handling large and diverse datasets. In our study, Random Forest was employed for DHF classification, and its ensemble nature enabled effective feature selection and classification accuracy. Parameters were fine-tuned to optimize Random Forest's performance.

 This research methodology hinges on employing machine learning algorithms, particularly Support Vector Machine (SVM) and Random Forest, for the effective classification and management of Dengue Haemorrhagic Fever (DHF). It commences with meticulous data collection and preprocessing, ensuring the dataset encapsulates crucial DHF symptoms and clinical parameters while prioritizing ethical considerations and robust feature engineering. Following this, SVM and Random Forest models are applied to classify DHF, engaging in a comprehensive training, validation, and testing cycle to refine the model parameters and assess their performance. The study conducts a comparative analysis between the SVM and Random Forest models, aiming to discern their individual strengths. Overall, the research strives to enhance classification accuracy, predict early recovery, optimize healthcare resource allocation, and advocate data-driven healthcare practices by harmonizing medical domain insights with machine learning proficiency, aiming to significantly improve patient care and public health outcomes in dengue-prone regions.
- Data Collection and Preprocessing
The dataset utilized in this research encompasses a set of attributes pertaining to Dengue Haemorrhagic Fever (DHF) symptoms and clinical parameters. These attributes were meticulously curated to facilitate the classification of DHF cases into distinct stages, without any involvement in data creation or modification. Each attribute signifies a specific symptom or clinical parameter integral to the DHF diagnostic process. The dataset comprises the following attributes:
•	Dengue days: Denoting the duration since the onset of Dengue symptoms.
•	Dengue current temp: Representing the patient's current body temperature.
•	Dengue WBC: Signifying the White Blood Cell count, a pivotal immunological marker.
•	Dengue severe headache: A binary indicator for the presence of severe headaches.
•	Dengue pain behind the eyes: A binary indicator for pain behind the eyes, a prominent DHF symptom.
•	Dengue joint muscle aches: A binary indicator for joint and muscle aches.
•	Dengue metallic taste in the mouth: A binary indicator for experiencing a metallic taste in the mouth.
•	Dengue appetite loss: A binary indicator for loss of appetite.
•	Dengue abdominal pain: A binary indicator for abdominal pain.
•	Dengue nausea vomiting: A binary indicator for nausea and vomiting.
•	Spontaneous bleeding: A binary indicator for spontaneous bleeding.
•	Dengue plasma leakage: A binary indicator for the presence of plasma leakage, a critical DHF symptom.
•	Dengue circulatory failure: A binary indicator for circulatory failure.
•	Dengue haemoglobin: Denoting the levels of haemoglobin in the patient's blood.
•	Dengue haematocrit: Representing the haematocrit levels, indicating the proportion of red blood cells in the blood.
•	Dengue platelet: Signifying the platelet count, a pivotal parameter in DHF diagnosis.
•	Dengue classification: The final classification of DHF cases into distinct stages, including Early Febrile, Critical, and Recovery.


Machine Learning Framework
i.	Support Vector Machine (SVM): 

![image](https://github.com/user-attachments/assets/cb3695da-2e9a-4662-ac43-adb21291293b)

The output from the SVM model reveals the classification of individuals into the three Dengue Haemorrhagic Fever (DHF) stages—Febrile, Critical, and Recovery. Analysing the count within each phase:
•	Febrile Phase: The model assigned 22 instances to the Febrile Phase, indicating the presence of symptoms related to the initial febrile stage of DHF.
•	Critical Phase: The model classified 72 instances within the Critical Phase, signifying the manifestation of critical symptoms and conditions associated with severe Dengue.
•	Recovery Phase: Only 6 instances were categorized under the Recovery Phase, suggesting a smaller number of cases in the recovery stage.
This distribution implies that the SVM model predominantly identified a substantial number of cases in the Critical Phase, signifying the severity of Dengue symptoms in these cases. The fewer instances assigned to the Recovery Phase might suggest challenges in accurately identifying individuals in this stage or a lower representation of patients in the recovery stage within the dataset. Understanding these categorizations could be essential for tailoring interventions and healthcare strategies, particularly to address the critical stage, which seems to have a higher representation in the dataset.
 
ii.	Random Forest 

![image](https://github.com/user-attachments/assets/afd10195-a1d7-4d46-afcd-682449bb6895)

The output from the Random Forest model reveals the classification of individuals into the three Dengue Haemorrhagic Fever (DHF) stages—Febrile, Critical, and Recovery. Analysing the count within each phase:
•	Febrile phase: There are 59 instances classified as the febrile phase.
•	Critical phase: There are 39 instances classified as the critical phase.
•	Recovery phase: There are only 2 instances classified as the recovery phase.
	The Random Forest algorithm has categorized the instances into three distinct phases of Dengue: febrile, critical, and recovery. It appears that the critical phase has the most instances, indicating that, in the dataset used for classification, more cases were identified as critical. Conversely, the recovery phase has the fewest instances, implying that this phase might be less frequent or easily distinguishable in the dataset. This classification allows for a breakdown of Dengue cases into these three categories, aiding in better understanding and categorization for targeted interventions and patient care strategies. 

A.	Model Evaluation Metrics
The evaluation of our machine learning models revealed several essential metrics. The Accuracy of both Support Vector Machine (SVM) and Random Forest models stood at 56%. This metric depicts the models' overall correctness in predicting class labels. Despite its moderate nature, accuracy alone might not suffice, especially when dealing with imbalanced datasets.
 
![image](https://github.com/user-attachments/assets/cde4e063-6331-4b93-bbd8-35826c0bb804)
i.	Precision, Recall, and F1-Score
Both SVM and Random Forest models achieved a Precision score of 0.56, emphasizing their capacity to make accurate positive predictions. Similarly, the Recall metric was also 0.56, indicating the models' ability to capture 56% of the actual positive cases. The F1-Score, a balance between precision and recall, also stood at 0.56 for both models, signifying a balanced approach considering false positives and false negatives.
B.	Confusion Matrix Analysis
The Confusion Matrix for both models delineated a detailed breakdown of their performance across three classes—Early Febrile, Critical, and Recovery stages. The diagonal elements (20, 35, and 1) represented the true positives for each class. However, the off-diagonal elements highlighted the model's errors, indicating instances of false positives and negatives, such as predicting class 3 instead of class 2 in a few cases.

The performance assessment indicated a moderate yet balanced precision and recall for both models. These findings were crucial in identifying specific dataset characteristics and class imbalances affecting performance. Moving forward, the investigation aims to address these challenges to enhance classification accuracy, ultimately refining patient care and resource allocation.

