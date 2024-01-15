# AI Model Packages to Reduce Insurance Premium Cost from Insured Persons, Doctors, and Insurance Company

## Introduction of Owner

Owner of this GitHub project is Ke Liu, who graduated from NYU's Tandon School of Engineering, and received the degree of Master of Science in Financial Engineering. Ke Liu's working achivements are in both AI field and research field:

- Accomplished several AI models which are built up to solve financial problems by processing numeric data, text data, image data, time series data etc., with great test scores, like 97.25% acuuracy score, 96.97% recall score and so on. The financial problems includes how to price financial derivatives, how to perdict financial index, how to recognize non-numeric data to support financial decisions, and so on. Ke Liu even has an APP-Built-Up experience in UBS, the Union Bank of Switzerland, which utilized NLP methods to tag companies in real time to make reference for investors. All AI projects' details could be found in Ke Liu's LinkedIn profile, https://www.linkedin.com/in/ke-liu-459688218/.

- Researched more than 10 national, provincial and industrial projects during her undergraduate school which are focused on investment facilitating, risk management, national development policies as well as regional development system, and published a paper in China. Here's her Google Scholar profile, https://scholar.google.com/citations?hl=en&user=8yJFZ4IAAAAJ. The research topics includes most of important components of macroeconomics and microeconomics, and the researches are complimented in several conferences. 

Now Ke Liu is working for an Insurance Company in New York, and aims to research the reason of increasing insurance premium cost and built AI models package to reduce the insurance premium cost, in order to increase the whole USA welfare.

## Background Information

Health insurance expenditure has always been one of the important living expenditure items for American citizens. According to the National Health Expenditure Accounts (NHEA), which are the official estimates of total health care spending in the United States, U.S. health care spending grew 4.1 percent in 2022, reaching $4.5 trillion or $13,493 per person. As a share of the nation's Gross Domestic Product, health spending accounted for 17.3 percent. Source: https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/historical#:~:text=The%20data%20are%20presented%20by,spending%20accounted%20for%2017.3%20percent.

Among the huge amount of health spending:
- National Health Expenditure(NHE) grew 4.1% to $4.5 trillion in 2022, or $13,493 per person, and accounted for 17.3% of Gross Domestic Product (GDP).
- Medicare spending grew 5.9% to $944.3 billion in 2022, or 21 percent of total NHE.
- Medicaid spending grew 9.6% to $805.7 billion in 2022, or 18 percent of total NHE.
- Private health insurance spending grew 5.9% to $1,289.8 billion in 2022, or 29 percent of total NHE.

Which shown the rapidly growing insurance expenditure. And it’s time to take action to curb the rise in insurance premium costs to improve USA citizen's whole welfare with AI.

## Goals

In this project, here are two goals: find the reasons of high insurance expenditure & build AI models to reduce insurance premium cost. By figuring out the reasons of high insurance expenditure, AI models could be used to summarize factors, monitor actions, simulate situations, facilitate process and so on.

The reasons of high insurance expenditure come from three aspects:

- **Insured persons' part**
  - ***Medical waste actions***. Given the insurance company will pay part or even most of bills, insured people will unavoidably intend to look for unnecessarily more expensive treatment or even just unnecessary treatment to take advantages of insurance company, which will increase the medical cost, and lead to an increase in insurance premium costs.
  - ***Fraud actions***. A more serious situation is that some insured persons will fake medical records to defraud insurance companies. Because all insured people share the same insurance fund, no matter if they are honest or not, and the high usage of the fund will lead to high insurance premium cost, so the fraud actions have to be controled to make the insurance premium cost reasonable.
  - ***Impersonation actions***. Not all people are insured, but all people will take medical cares to some extent. Thus, there are some people will take impersonation actions to lower their medical cost. This behavior takes up insurance funds that do not originally intend to be used on them, and increase the insurance premium the policyholders paid.

- **Doctors' part**
  - ***Substance abuse***. When cooperating with insurance company, patients' bills are paid by both patient and insurance company. Both of them are responsible for part of the bills, and the whole budget will be increased in a certain degree, so a few doctors will intend to do subtance abuse to increase their income. However, even if there's no insurance company's involvement, the substance abuse is inevitable sometimes. The substance abuse is one of the reasons makes the insurance premium cost high.
 
- **Insurance companies' part**
  - ***Inaccurate premium pricing model***. Insurance companies have their own pricing models to decide the insurance premium cost. These models are designed to make sure there's profit for insurance company after paying all medical fees for their insured clients. In order to ensure that, there will be set as much gap space as possible between the premium collected from policyholders and the payment to doctors. More accurate pricing models will make the gap smaller, which makes the insurance premium cost lower furtherly.


## Plans & Framework of AI model package

AI models are the process of learning. Feed comprehensive and advanced AI models with as much data as possible. After fine tuning, the AI models will show a great performance. Thus, the core of designing these AI models are collecting suitable and feasible data, and find the perfect AI models to train and predict based on different AI models' mathematical principles and functions.

- **Collecting Suitable and Feasible Data**
  - ***Data Type***
    Because the AI models package intend to solve multiple problems from insured people, doctors and insurance companies' aspects, which includes 5 directions, so the data type includes numeric data like insured people's income, age, medical test report, etc., image data like photo of insured people, iamge medical reports, etc., and the text data like reports doctors write, prescriptions doctors made, etc.
  - ***Data Source***
    All these data could be provided from insurance company who has the detailed insured people's information when they sign the contract and the historical records of all kinds of dishonest people and actions, and doctors or medical experts who has the medical experience to tag medical fraud actions to help AI models learn and predict.
  
- **Find Perfect AI Models to Train and Predict**
  - ***A. AI models to monitor medical waste actions***
    - **a. Data needed**: \
      Insured people's basic numeric information collected when signing insurance contract like age(0~150,Integer), income(Numeric, Unit:k), insured people size(Integer), medical test scores(Numeric), credit scores(Numeric), etc.
    - **b. AI algorithm candidates**:\
      Principal component analysis(PCA), KMeans, Support Vector Classifier (SVC), K-Nearest Neighbors(KNN), Naive Bayes
    - **c. Input**: \
      Insured people's basic numeric information collected when signing insurance contract (Numeric)
    - **d. Output**:\
      0~1, the probability of taking medical waste action
   
      
  - ***B. AI models to monitor fraud actions***
    - **a. Data needed**:\
      Doctors' or experts' tagged honest and fraud medical records' database (data series with tag 0 or 1)
    - **b. AI algorithm candidates**:\
      Bidirectional Encoder Representations from Transformers (BERT), Convolutional Neural Network(CNN), Recurrent Neural Network (RNN), Long Short-Term Memory (LSTM)
    - **c. Input**:\
      Insured people's historical medical records and new medical records (Images, text, and numbers data series without tag)
    - **d. Output**:\
      0~1, the probability of defrauding\

      
  - ***C. AI models to monitor impersonation actions***
    - **a. Data needed**:\
    Insured people's bio information such as photo or fingerprint(Image), and database that includes large amount comparable bio photos marked 0 and 1 (Image data with tag 0 or 1).
    - **b. AI algorithm candidates**:\
      Principal component analysis(PCA), Convolutional Neural Network(CNN)
    - **c. Input**:\
      Real-time face recognition video taken when entering insurance information (Image)
    - **d. Output**:\
      0 or 1, stands for it's the exact insured person or not

  - ***D. AI models to monitor substance abuse***
    - **a. Data needed**: \
      Doctors' or experts' tagged abuse or not medical records' database (text data series with tag 0 or 1).
    - **b. AI algorithm candidates**:\
      Bidirectional Encoder Representations from Transformers (BERT), Convolutional Neural Network(CNN), Recurrent Neural Network (RNN), Long Short-Term Memory (LSTM)
    - **c. Input**:\
      Doctors' medical records on one certain insured person (text data series without tag)
    - **d. Output**:\
      0~1, the probability of substance abusing

  - ***E. AI models to build more accurate premium pricing model***
    - **a. Data needed**:\
      History database of insured people's basic information(Yearly, Numeric), all scores above AI models generated(Numeric), usage of insurance fund(Yearly, Numeric), and economic data like inflation rate etc. (Numeric).
    - **b. AI algorithm candidates**:\
      Principal component analysis(PCA), K-Nearest Neighbors(KNN), Support Vector Regression (SVR), RidgeRegression
    - **c. Input**:\
      Insured people's basic information (Numeric), scores generated from above AI models (Numeric), and economic data (Numeric)
    - **d. Output**:\
      Expectaion of the cost of certain type insured people (Yearly, Numeric)
      
## Welcomes

Welcome every data providers and AI experts to contribute to the AI models package together. Please feel free to email me to get access to all codes: kl4246@nyu.edu. Once the models are built up maturely, packages will apply for USA patent and be provided to all insurance companies to create more welfare to USA citizens.

## Test





