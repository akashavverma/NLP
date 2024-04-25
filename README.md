# SemEval 2023 Task 6: LegalEval - Understanding Legal Texts
This Project is made up for course project in NLP offered at IIITD. Theproject is from SemEval 2023 Task 6. The paper about the same can be found at- https://arxiv.org/pdf/2304.09548.pdf 

Task A: Rhetorical Roles (RR) Prediction:
Given that legal documents are long and unstructured, we proposed a task for automatically segmenting legal judgment documents into semantically coherent text segments, and each such segment is assigned a label such as a preamble, fact, ratio, arguments, etc. These are referred to as Rhetorical Roles (RR).

We target 13 RRs as outlined in our previous work Kalamkar et al. (2022b): 
Preamble, Facts, Ruling by Lower Court, Issues, Argument by Petitioner, Argument by Respondent, Analysis,
Statute, Precedent Relied, Precedent Not Relied, Ratio of the decision, Ruling by Present Court and None.
The Evaluation Metrics is F1 Score.

RR Task Relevance: The purpose of creating a rhetorical role corpus is to enable an automated understanding of legal documents by segmenting them into topically coherent units (Refer to Problem Definition in the poster). This segmentation is a fundamental building block for many legal AI applications like judgment summarization, judgment outcome prediction, precedent search, etc.

We proposed an architecture inspired from IRIT_IRIS team which has input as Dynamic-Filled Contextualized Sentence Chunks passed on to Indian System Legal Bert Encoder further passed to an Attention layer and a CRF layer. A better understanding of the project can be understood from the poster below:
![WhatsApp Image 2024-04-25 at 23 41 37_b642c37d](https://github.com/akashavverma/Rhetorical_Roles-Prediction-in-Legal-Documents/assets/47278817/a44acffa-2d76-44c1-95a4-0aa8148865b4)

The saved models can be found here - https://drive.google.com/drive/folders/1c8b_BFukHtXgVi7Ua2_a2JwyjSCwNitY?usp=sharing
To reproduce kindly change the path of the dataset in the application.py and application_longformer.py file and run the run_<Encoder>.py.
Reference and credits - https://github.com/alexlimatds/SemEval_2023_Task_6A
