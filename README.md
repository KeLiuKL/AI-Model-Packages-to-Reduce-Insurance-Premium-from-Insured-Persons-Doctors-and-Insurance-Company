# AI Model Packages to Reduce Insurance Premium Cost from Insured Persons, Doctors, and Insurance Company

## Introduction of Owner

Owner of this GitHub project is Ke Liu, who graduated from NYU's Tandon School of Engineering, and received the degree of Master of Science in Financial Engineering. Ke Liu's working achivements are in both AI field and research field. Now Ke Liu is working for an Insurance Company in New York, and aims to research the reason of increasing insurance premium cost and built AI models package to reduce financial and medical waste which can eventually reduce the insurance premium cost, in order to increase the whole U.S. healthcare welfare. Here is a biref summary of some of her achievements:

- AI field: Accomplished plentiful AI models which are built up to solve financial problems by processing numeric data, text data, image data, time series data etc., with great test scores, such as 97.25% acuuracy score, 96.97% recall score and so on. The financial problems includes pricing financial derivatives, perdicting financial indexes, recognizing non-numeric data to support financial decisions, and so on. Ke Liu also has an APP-Built-Up experience in UBS, the Union Bank of Switzerland, which utilized NLP methods to tag companies in real time to make reference for investors. All AI projects' details could be found in Ke Liu's LinkedIn profile, https://www.linkedin.com/in/ke-liu-459688218/.

- Research field: Researched more than 10 national, provincial and industrial projects during her undergraduate school which are focused on investment facilitating, risk management, national development policies as well as regional development system, and published a paper in China. Here's her Google Scholar profile, https://scholar.google.com/citations?hl=en&user=8yJFZ4IAAAAJ. The research topics includes most of important components of macroeconomics and microeconomics, and these researches are complimented in several Chinese academic conferences.

## Background Information

Health insurance expenditure has always been one of the important living expenditure items for American citizens. According to the National Health Expenditure Accounts (NHEA), which are the official estimates of total health care spending in the United States, U.S. health care spending grew 4.1 percent in 2022, reaching $4.5 trillion or $13,493 per person. As a share of the nation's Gross Domestic Product, health spending accounted for 17.3 percent. Source: https://www.cms.gov/data-research/statistics-trends-and-reports/national-health-expenditure-data/historical#:~:text=The%20data%20are%20presented%20by,spending%20accounted%20for%2017.3%20percent.

Among the huge amount of health spending:
- National Health Expenditure(NHE) grew 4.1% to $4.5 trillion in 2022, or $13,493 per person, and accounted for 17.3% of Gross Domestic Product (GDP).
- Medicare spending grew 5.9% to $944.3 billion in 2022, or 21 percent of total NHE.
- Medicaid spending grew 9.6% to $805.7 billion in 2022, or 18 percent of total NHE.
- Private health insurance spending grew 5.9% to $1,289.8 billion in 2022, or 29 percent of total NHE.

Which shown the rapidly growing healthcare expenditures and insurance expenditures. And it’s time to take action to curb the rise in healthcare expenditures and also insurance premium costs to improve U.S. citizen's healthcare welfare with AI, which could be used to monitor financial and medical resources waste, like insurance fraud or intended medical waste etc., occurred during the healthcare process, in order to improve medical fund’s efficiency, and thereby reduce insurance premium levels, then the overall medical conditions of the American people will be improved, thus improving overall social welfare. 

## Goals

In this project, here are two goals: find the source of financial and medical resources waste & build AI models to reduce financial and medcial waste in order to reduce the healthcare cost as well as the insurance premium cost. By figuring out the source of financial and medical resources waste, AI models could be used to summarize factors, monitor actions, simulate situations, facilitate process and so on.

The source of financial and medical resources waste comes from three aspects:

- **Insured persons' part**
  - ***Medical waste actions***. Given the insurance company will pay part or even most of bills, insured people will unavoidably intend to look for unnecessarily more expensive treatment or even just unnecessary treatment to take advantages of insurance company, which will cause the waste of financial and medical resources.
  - ***Fraud actions***. A more serious situation is that some insured persons will fake medical records to defraud insurance companies. Because all insured people share the same insurance fund, no matter if they are honest or not, and the high usage of the fund will lead to high insurance premium cost, so the fraud actions have to be controled to stop this kind of financial waste.
  - ***Impersonation actions***. Not all people are insured, but all people will take medical cares to some extent. Thus, there are some people will take impersonation actions to lower their medical cost. This behavior will waste insurance funds that do not originally intend to be used on them, and increase the insurance premium the policyholders paid.

- **Doctors' part**
  - ***Substance abuse***. When cooperating with insurance company, patients' bills are paid by both patient and insurance company. Both of them are responsible for part of the bills, and the whole budget will be increased in a certain degree, so a few doctors will intend to do subtance abuse to increase their income. However, even if there's no insurance company's involvement, the substance abuse is inevitable sometimes. The substance abuse is one of the source of financial and medical resources waste which makes the insurance premium cost high.
 
- **Insurance companies' part**
  - ***Inaccurate premium pricing model***. Insurance companies have their own pricing models to decide the insurance premium cost. These models are designed to make sure there's profit for insurance company after paying all medical fees for their insured clients. In order to ensure that, there will be set as much margin space as possible between the premium collected from policyholders and the payment to doctors. More accurate pricing models will make the margin smaller, which won't collect financail resources wastely anymore, and makes the financial resources freely flow to whole society where needs it more.


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
      Principal component analysis(PCA), KMeans, Support Vector Classifier (SVC), K-Nearest Neighbors(KNN), Naive Bayes, XGBoost, RandomForest
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
      0~1, the probability of defrauding

      
  - ***C. AI models to monitor impersonation actions***
    - **a. Data needed**:\
    Insured people's bio information such as photo or fingerprint(Image), and database that includes large amount comparable bio photos.
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
      Bidirectional Encoder Representations from Transformers (BERT), Recurrent Neural Network (RNN), Long Short-Term Memory (LSTM)
    - **c. Input**:\
      Doctors' medical records on one certain insured person (text data series without tag)
    - **d. Output**:\
      0~1, the probability of substance abusing

  - ***E. AI models to build more accurate premium pricing model***
    - **a. Data needed**:\
      History database of insured people's basic information(Yearly, Numeric), all scores above AI models generated(Numeric), usage of insurance fund(Yearly, Numeric), and economic data like inflation rate etc. (Numeric).
    - **b. AI algorithm candidates**:\
      Principal component analysis(PCA), KMeans, Support Vector Regression (SVR), RidgeRegression, XGBoost, Random Forest
    - **c. Input**:\
      Insured people's basic information (Numeric), scores generated from above AI models (Numeric), and economic data (Numeric)
    - **d. Output**:\
      Expectaion of the cost of certain type insured people (Yearly, Numeric)

## Blockchain and Data Collecting

Nowadays, the medical data in the healthcare world is very fragmented. This is the reason why AI is currently developing faster in the property and casualty insurance field than in the medical insurance field. Blockchain technology becomes a great solution of the medical data islands, which can effectively solve the privacy and sharing issues of medical data. And the introduction of Blockchain will be a great data support tool for AI modeling work.

- **Construction of DApps Using Blockchian** 

  DApps(decentralized applications) is the APP using blockchain technology to store and share data safely, which could be the database for AI modeling work. On the DApp, data could be processed automatically in blockchain. Patients can get his or her own keys immediately to encrypt and decrypt data, data providers can upload the original data to the DApp to encrypt data, and data recipients can request the patient's data on the DApp to decrypt and verify data. No one can change or see the medical data, except the patients and authorized people by patients. Patients own the absolute right of data. 

  DApps could be constructed on ETHEREUM and RIPPLE platforms. With Ke Liu's work experience in UBS, in which she completed an App construction on the Streamlit platform, constructing DApps will be easier and faster. And the DApps will ensure that during the use of DApps, all users’ sensitive information is only a binary string of numbers used for identification, such as name, etc. No one will identify the user’s sensitive information through the DApps. DApps will only serve as a blockchain of data storing and data sharing tools, and that’s all. Privacy will be strictly protected. 

- **Data Sharing Incentives**
  
  Blockchain can give patients and other data subjects full ownership and use rights of data, greatly improving the privacy and security of data, and at the same time providing safe and unimpeded communication between data owners and data recipients, which is beneficial to all participants. Here are some proposed data-sharing incentives, which could speed the database's growing:

  - **For insurance companies:** \
    For any insurance company that provides data, after the completion of the blockchain construction and the construction of the AI algorithm models, they can obtain free usage rights of the AI models, including insurance premium pricing model and medical supervision models for three years.
  - **For medical data owners:** \
    Any insured person and patient who provides medical data information will be rewarded with DApp tokens, and DApp tokens can be used to pay medical expenses and insurance premiums, or can be cashed to dollars directly on DApp.
  - **For hospital and medical experts:** \
    Any hospital or medical expert that assists to provide medical data can obtain the right to use the AI models of medical supervision for free for three years, to detect patient’s fraud or medical waste actions, and to improve the hospital's premium recovery rate, and at the same time give them DApp token rewards too, which can be exchanged for medical facilities, etc.

Construction of DAPPs is a supplement for data collecting for AI modeling work, which will improve medical world to a new level. Even though Blockchain has a powerful function, its structure is very simple and easy to construct. As a new technology in medical world, Blockchain has a great space to develop and apply, and everything is possible in this Blue Ocean.

      
## Welcomes

Welcome all data providers and AI experts to contribute to the AI models package together. Please feel free to email me to get access to all codes: kl4246@nyu.edu. Once the models are built up and pass tests, packages will apply for USA patent and be provided to all insurance companies to create more welfare to USA citizens. Participants will get free using of needed AI models for three years, DApps tokens, or patent dividends based on their contribution ratio too.







