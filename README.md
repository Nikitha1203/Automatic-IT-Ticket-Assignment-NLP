Automatic IT Ticket Assignment NLP
Overview
This project aims to automate the assignment of IT tickets to the right functional groups within an organization by analyzing the given ticket descriptions. By leveraging Natural Language Processing (NLP) techniques and machine learning algorithms, the goal is to enhance the efficiency of incident management and reduce manual intervention.
Business Understanding
In any IT industry, efficient incident management is crucial for delivering quality support to customers. Incident tickets are created and assigned to resolve issues promptly. The Service Desk team performs initial analysis and assigns tickets to the respective teams. Manual assignment has disadvantages like resource usage, human errors, and delays. Automating ticket assignment can lead to cost-effectiveness, faster resolutions, and better focus on productive tasks.
Objective
The main objective is to build an AI-based classifier model capable of assigning tickets to the right functional groups based on their descriptions. The target accuracy for the model is set at a minimum of 85%.
Dataset
The dataset used for training and evaluating the model can be found here.
Steps Followed
1.	Text Pre-processing:
•	Unwanted characters and words were removed from ticket descriptions.
•	Descriptions in other languages were translated to English.
•	Stop words were removed, and lemmatization was applied.
2.	Embedding:
•	Word embeddings were created using Word2Vec.
•	Embeddings were also generated with GloVe.
3.	NLP Algorithms:
•	Different NLP algorithms, including RNN, LSTM, and GRU, were experimented with.
•	Traditional ML algorithms such as RandomForest and SVM were also explored.
Limitations
•	To address data sparsity, assignment groups with less than 10 entries were grouped as 'misc_grp.' In a real-world scenario, additional intervention might be needed for tickets classified under 'misc_grp.'
Conclusion
The model achieved a classification accuracy of 91.24%, showcasing its effectiveness in automating IT ticket assignment. For real-world deployment, collecting additional data (around 300 records for each group) could further improve accuracy. The README file provides an overview of the project's purpose, steps taken, dataset information, and limitations.

