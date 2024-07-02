# Product-Price-Prediction

This data science project aims to predict the sale price of used cars in India by analyzing a dataset of used car listings. 

The project aims to provide statistical information on the average sale price and the used car market in India, in order to help people make informed buying choices and get a good deal on a used vehicle.

The questions that the project will tackle include:

* What is the average price for a car
* What is the average kms driven for a car
* What are the top car features that influence price
* The machine learning objective of this project is to minimize the difference between the real price and the price estimated by the model.

The model performance will be evaluated using three metrics:

* Mean squared error (MSE)
* Root squared of the mean squared error (RMSE)
* R-squared (R2)

The project will use supervised machine learning techniques and will use the provided dataset to train and test the model. 

The goal is to create a model that can accurately predict the sale price of used cars in India, based on various factors such as car features, kms driven and others.

The final model will be deployed to a web app or API for end-users to use.

<h3>This project was a capstone and below are in-depth explanations for the project as well as an example proposal to a made-up company to impliment it in their company</h3>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <h1>Proposal for Implementing a Predictive Application for Used Car Prices</h1>
</head>
<body>
    <h1>Part A: Letter of Transmittal</h1>
    <p><strong>May Cooper</strong><br>
       Senior Data Scientist<br>
       Data Science Solutions Inc.<br>
       Email: may.cooper@datasciencesolutions.com<br>
       Aurora, ON, Canada
    </p>
    <p>To:<br>
       <strong>Rohan Patil</strong><br>
       Chief Executive Officer<br>
       India Global Used Car Marketplace<br>
       Bangalore, India
    </p>
    <p><strong>Subject:</strong> Proposal for Implementing a Predictive Application for Used Car Prices</p>
    <p>Dear Rohan,</p>
    <p>I am reaching out to propose a robust solution to a significant challenge facing the used car market in India: the inconsistency in pricing that hampers consumers’ ability to make informed purchasing decisions. Our proposed machine learning-based application is designed to offer accurate and reliable predictions of used car prices, thereby enhancing market transparency and efficiency.</p>
    <p>The used car market is currently characterized by significant price variability, making it challenging for consumers to ascertain the fair market value of vehicles. This variability stems from many factors, including differences in car models, years of manufacture, mileage, fuel types, and other specific features. The lack of a reliable mechanism to predict car prices leads to consumer dissatisfaction, a lack of trust in the market, and potential financial losses. Addressing this issue is critical to fostering a more transparent and efficient market environment.</p>
    <p>We will employ the CRISP-DM methodology for this project, encompassing data preparation, exploratory data analysis, model training, and evaluation. The initial funding requirement is estimated at $83,000, covering data acquisition, model development, and deployment costs. The project is expected to take approximately 3 months from inception to deployment.</p>
    <p>To address this issue, I propose developing an advanced predictive tool that employs machine learning algorithms to analyze historical sales data. This application will provide users with precise price estimates for used cars based on input features like model, year, mileage, fuel type, and transmission. By leveraging comprehensive datasets and sophisticated analytical techniques, the application will offer precise and reliable price predictions, empowering consumers with valuable insights for making informed purchasing decisions.</p>
    <p>The implementation of this predictive application offers several tangible benefits to India Global Used Car Marketplace. The application will enhance customer confidence and satisfaction by providing consumers with accurate and reliable price estimates, leading to higher customer loyalty and repeat business.</p>
    <p>Additionally, offering a cutting-edge tool that simplifies the car buying process will position our organization as an innovator and leader in the automotive market, attracting more customers and solidifying our brand’s reputation for excellence and customer-centric solutions. Furthermore, the application will streamline the pricing process for our sales team, enabling them to offer competitive and fair pricing quickly, reducing the time spent on negotiations, and improving overall sales productivity, leading to increased revenue and profitability.</p>
    <h2>Implementation Plan:</h2>
    <ul>
        <li><strong>Costs:</strong> The estimated budget for this project is $83,000 USD, covering data acquisition, model development, application deployment, initial marketing efforts, and ongoing maintenance.</li>
        <li><strong>Timeline:</strong> The project is projected to be completed within three months, including phases such as data preparation, model training, application development, testing, and final deployment.</li>
        <li><strong>Data:</strong> We will utilize a robust dataset scraped from CarDekho, a leading used car online marketplace in India, including detailed records of past used car sales in India, encompassing variables such as selling price, kilometers driven, fuel type, transmission type, and other relevant car features.</li>
        <li><strong>Ethical and Legal Considerations:</strong> Throughout the project, we will strictly adhere to data privacy regulations, maintain transparency in our modeling processes, and implement measures to mitigate potential biases in the model to ensure fair and equitable price predictions.</li>
    </ul>
    <p>As a Senior Data Scientist with extensive experience in machine learning and data analytics, I possess the expertise necessary to lead this project to success. My background includes developing and deploying predictive models across various domains, ensuring they meet high standards of accuracy and reliability. My proficiency in handling large datasets and a deep understanding of the automotive market position me uniquely to deliver a high-quality solution that aligns with our organizational goals.</p>
    <p>I am confident that the proposed predictive application will significantly benefit our organization and our customers. By providing accurate price estimates, the application will enhance market transparency, boost customer satisfaction, and position us as a market leader. I look forward to discussing this proposal further and addressing any questions or concerns you may have.</p>
    <p>I appreciate your consideration.</p>
    <p>Sincerely,<br>
       May Cooper<br>
       Senior Data Scientist<br>
       Data Science Solutions Inc.
    </p>
    <h1>Part B: Project Proposal Plan</h1>
    <h2>Project Summary</h2>
    <p><strong>Problem Description:</strong></p>
    <p>India’s used car market is characterized by significant price variability, creating substantial challenges for consumers seeking to ascertain fair market values. This inconsistency arises from many factors, including differences in car models, years of manufacture, mileage, fuel types, and specific features. Such variability complicates the decision-making process for consumers, leading to several key issues:</p>
    <ul>
        <li>Consumers often feel frustrated and uncertain when faced with widely varying prices for similar vehicles. This dissatisfaction stems from a lack of confidence in their ability to secure a fair deal, resulting in a negative experience that could deter future transactions.</li>
        <li>Inconsistent pricing undermines trust in the used car market. Consumers may perceive the market as unfair or exploitative when encountering substantial price differences without clear justification. This lack of trust could deter participation in the market, reducing overall activity.</li>
        <li>Without reliable price estimates, consumers risk overpaying for vehicles or selling their cars below market value. Both scenarios lead to financial losses, significantly impacting individual finances, particularly in a price-sensitive market like India’s.</li>
        <li>The time and effort required to research and compare prices across various sources adds to the complexity of the buying process. Consumers may need to consult multiple dealerships, online platforms, and private sellers to gather enough information to make an informed decision, which is time-consuming and confusing.</li>
        <li>For sellers, particularly dealerships, the inability to price vehicles accurately results in extended inventory holding periods or missed sales opportunities. Overpriced vehicles remain unsold, while underpriced vehicles may be sold quickly but at a financial loss. These inefficiencies hinder the used car market’s overall fluidity and profitability, affecting consumers and sellers adversely.</li>
    </ul>
    <p>To illustrate the variability in pricing, consider the following examples from the dataset:</p>
    <ul>
        <li>A 2014 Maruti Swift Dzire VDI priced at INR 450,000 with 145,500 kilometers driven, Diesel fuel type, Manual transmission, and being a First Owner vehicle</li>
        <li>A 2014 Skoda Rapid 1.5 TDI Ambition priced at INR 370,000 with 120,000 kilometers driven, Diesel fuel type, Manual transmission, and being a Second Owner vehicle</li>
        <li>A 2006 Honda City EXi priced at INR 158,000 with 140,000 kilometers driven, Petrol fuel type, Manual transmission, and being a Third Owner vehicle</li>
    </ul>
    <p>In this example, three vehicles from different years exhibit a wide range of selling prices, from INR 158,000 to INR 450,000. Factors such as mileage, fuel type, owner history, and vehicle condition contribute to this variability, complicating the determination of a fair price for consumers.</p>
    <p>Addressing these issues requires a reliable and transparent mechanism for predicting used car prices that consumers can trust. By implementing a machine learning-based solution, Data Science Solutions Inc. will address these challenges, strengthen customer satisfaction, build trust in the market, and reduce financial risks for consumers. This approach will also position India Global Used Car Marketplace as an innovative leader in the automotive industry, leveraging technology to provide valuable solutions to market inefficiencies.</p>
    <h2>Client and Their Needs:</h2>
    <p>India Global Used Car Marketplace aims to address the issue of price variability in the used car market by developing a machine learning-based application that will provide accurate and reliable predictions of used car prices. This tool will enhance market transparency and efficiency, making it easier for consumers to evaluate and compare car prices. The primary customers will be used car buyers and sellers needing a reliable and user-friendly tool to make informed car purchase and sale decisions.</p>
    <h2>Deliverables:</h2>
    <ul>
        <li>Standalone Application: A downloadable application that can be used locally on a computer to predict used car prices</li>
        <li>User Guide: Detailed instructions on downloading, installing, and using the application</li>
        <li>Machine Learning Model: A model that can be updated and retrained as new data becomes available to ensure it remains accurate and relevant</li>
        <li>Regular Updates: Periodic updates to the application and model based on new data and user feedback</li>
    </ul>
    <h2>Application Benefits:</h2>
    <p>The application will deliver several key advantages that will significantly impact consumers and India Global Used Car Marketplace. By offering accurate price estimates, it will enhance customer confidence and satisfaction. The streamlined pricing process for sales teams will increase sales productivity, and the company’s reputation as an innovative leader in the automotive market will be solidified. Ultimately, these benefits will increase customer loyalty, higher sales productivity, and enhanced revenue.</p>
    <p>The application will offer:</p>
    <ul>
        <li>Accurate Price Estimates: Providing users with reliable price predictions based on various features of used cars</li>
        <li>Boosted Customer Confidence and Satisfaction: Ensuring that users feel more secure and informed when making purchase decisions</li>
        <li>Streamlined Pricing Process for Sales Teams: Enabling sales teams to price cars quickly and accurately, reducing the time spent on price negotiations</li>
        <li>Positioning as an Innovative Leader: Establishing India Global Used Car Marketplace as a forward-thinking leader in the automotive market</li>
    </ul>
    <h2>Justification:</h2>
    <p>The application will significantly enhance customer confidence and satisfaction by providing accurate and reliable price estimates, leading to higher customer loyalty and repeat business. Offering a cutting-edge tool that simplifies the car buying process will attract more customers and solidify the organization’s reputation for excellence and customer-centric solutions. The streamlined pricing process will improve overall sales productivity, increasing revenue and profitability.</p>
    <h2>Data Summary:</h2>
    <p>The primary data source for this project will be a comprehensive dataset from CarDekho, containing detailed records of past used car sales in India. This dataset will be particularly suited for our project due to its extensive coverage and the variety of variables it includes. The dataset will comprise key features such as car model, year of manufacture, selling price, kilometers driven, fuel type, transmission type, owner history, mileage, engine capacity, maximum power, torque, and number of seats. These variables will provide a holistic view of each car’s characteristics, making the dataset ideal for developing a machine learning model to predict used car prices accurately.</p>
    <p>The dataset includes the following columns:</p>
    <ul>
        <li><strong>name:</strong> The make and model of the car</li>
        <li><strong>year:</strong> The year of manufacture</li>
        <li><strong>selling_price:</strong> The price at which the car was sold</li>
        <li><strong>km_driven:</strong> The total kilometers driven</li>
        <li><strong>fuel:</strong> The type of fuel used by the car (Petrol, Diesel, CNG)</li>
        <li><strong>seller_type:</strong> The type of seller (e.g., Individual, Dealer)</li>
        <li><strong>transmission:</strong> The type of transmission (e.g., Manual, Automatic)</li>
        <li><strong>owner:</strong> The number of previous owners</li>
        <li><strong>mileage:</strong> The fuel efficiency of the car</li>
        <li><strong>engine:</strong> The engine capacity</li>
        <li><strong>max_power:</strong> The maximum power output of the engine</li>
        <li><strong>torque:</strong> The torque produced by the engine</li>
        <li><strong>seats:</strong> The number of seats in the car</li>
    </ul>
    <h2>Data Filtering and Initial Processing:</h2>
    <p>The dataset, in the form of a CSV, will require significant processing to ensure it only contains information relevant to accurately predicting used car prices. Initially, we will filter the dataset to focus on pertinent records, excluding irrelevant data points that do not contribute meaningfully to the price prediction model. For example, records of cars with incomplete data or non-standard features that do not align with typical market offerings will be excluded. This step will be critical to streamline the data processing pipeline and ensure that the model is trained on high-quality, relevant data.</p>
    <h2>Data Cleaning and Preparation:</h2>
    <p>Data cleaning will be an extensive process involving several critical steps to ensure data integrity and quality. Missing data points will be identified and addressed through imputation or removal. Imputation techniques will be employed to fill in gaps with plausible values, while removal will be considered for records with significant missing information that cannot be reliably imputed.</p>
    <p>Additionally, we will detect and handle outliers that could skew the model’s performance. For instance, cars with exceptionally high prices or extreme mileage not representative of typical sales will be analyzed and potentially excluded. This rigorous cleaning process will be essential to prepare the dataset for effective model training.</p>
    <h2>Normalization and Feature Engineering:</h2>
    <p>Normalization will be another vital step in our data processing workflow. Continuous variables, such as kilometers driven and engine capacity, will be normalized to ensure that all data is on a consistent scale. This will be crucial for the model’s accuracy, as it prevents variables with larger ranges from disproportionately influencing the predictions.</p>
    <p>In addition, feature engineering will be conducted to enhance the model’s predictive power. This will involve creating new features from existing ones, such as calculating the car’s age from its manufacturing year or deriving fuel efficiency metrics from mileage and engine specifications. Enriching the dataset with these engineered features can improve the model’s ability to learn and generalize from the data.</p>
    <h2>Data Management and Updates:</h2>
    <p>Effective data management practices will be implemented to ensure the dataset remains current and relevant throughout the project lifecycle. Regular updates will be made to incorporate new records, reflecting the latest trends and changes in the used car market.</p>
    <p>This ongoing maintenance will be critical to the model’s long-term performance and reliability. The processed and cleaned data will be stored in a CSV file, easily accessible for training the model and making predictions. Once the model is trained, the data file will remain within the application for maintenance. New records can be added, or the dataset can be replaced entirely to retrain the model as updated data becomes available.</p>
    <h2>Data Justification:</h2>
    <p>The data from CarDekho, a well-known online used car marketplace in India, will be exceptionally well-suited for this project due to its comprehensive nature and the inclusion of all relevant features needed for accurate price predictions. Key features of the dataset will include:</p>
    <ul>
        <li><strong>Car Model and Year:</strong> Provide essential information about the car’s make and age, which are critical factors in determining its market value</li>
        <li><strong>Selling Price:</strong> The target variable for our predictions, representing the actual transaction value of the vehicle</li>
        <li><strong>Kilometers Driven:</strong> Indicative of the car’s usage, influencing its depreciation and overall condition</li>
        <li><strong>Fuel Type, Transmission Type, and Owner History:</strong> Important factors influencing the car’s market value, affecting its desirability and performance</li>
        <li><strong>Engine Specifications and Mileage:</strong> Critical for determining the car’s performance and efficiency, impacting its resale value</li>
    </ul>
    <p>Standard preprocessing techniques will handle anomalies such as outliers and missing data to ensure data quality. This thorough preprocessing will ensure the model is trained on high-quality data, leading to more accurate and reliable predictions.</p>
    <h2>Ethical and Legal Considerations:</h2>
    <p>All data in this project will comply with relevant data privacy regulations, ensuring adherence to ethical standards. The dataset, scraped from publicly available car records on CarDekho, is de-identified and publicly available, addressing potential data privacy and confidentiality concerns. The dataset is licensed under CC0: Public Domain.</p>
    <p>Moreover, the project will maintain transparency in the modeling processes, allowing stakeholders to understand how predictions are made. Measures will be implemented to mitigate potential biases in the data, ensuring that the price predictions are fair and equitable. This commitment to ethical practices will foster trust in the model’s predictions and ensure the project upholds high data integrity and responsibility standards.</p>
    <h2>Implementation</h2>
    <h2>Methodology:</h2>
    <p>The project will employ the CRISP-DM (Cross-Industry Standard Process for Data Mining) methodology, a widely recognized and industry-standard framework for developing predictive models. CRISP-DM ensures a structured and systematic approach to model development, addressing all critical aspects of the project lifecycle. The methodology will comprise six distinct phases:</p>
    <h3>1. Business Understanding:</h3>
    <p>In this phase, we will define the project objectives and requirements by engaging with stakeholders, including car dealerships, potential buyers, and industry experts. We will gather insights into the key factors influencing used car prices, understand the market dynamics, and identify primary business goals. This phase will also involve determining the data requirements, scope of analysis, and relevant features to be included in the model. The outcome will be a comprehensive project plan and business objectives.</p>
    <h3>2. Data Understanding:</h3>
    <p>During this phase, we will collect and analyze the dataset to deeply understand its structure and the relationships between features. We will initially explore the data, examining its distribution, types, and anomalies or patterns. This exploration will help us identify the most relevant features and potential challenges that may arise during the data preparation phase.</p>
    <h3>3. Data Preparation:</h3>
    <p>The data preparation phase will involve cleaning, normalizing, and transforming the data to ensure it is suitable for model training. This will include:</p>
    <ul>
        <li><strong>Filtering and Cleaning:</strong> Removing irrelevant records, handling missing values through imputation or removal, and detecting and removing outliers</li>
        <li><strong>Normalization:</strong> Ensuring continuous variables such as kilometers driven and engine capacity are on a consistent scale</li>
        <li><strong>Feature Engineering:</strong> Deriving new features from existing ones to enhance the model’s predictive power, such as calculating the car’s age from the manufacturing year</li>
    </ul>
    <p>The outcome will be a final, cleaned, and processed dataset ready for model training.</p>
    <h3>4. Modeling:</h3>
    <p>In this phase, we will prepare a training set and a test set to develop and evaluate the machine learning models. To determine which model performs best, we will experiment with various machine learning algorithms, such as linear regression, random forest, support vector machines (SVM), decision trees, XGBoost, and gradient boosting. The best-performing model will be selected for deployment.</p>
    <h3>5. Evaluation:</h3>
    <p>The evaluation phase will assess the model’s performance to ensure it meets the business objectives. We will use metrics such as mean absolute error (MAE), root mean squared error (RMSE), and R-squared (R²) to evaluate the model’s accuracy and reliability. Additionally, we will validate the model using cross-validation techniques to ensure its robustness. If the model does not meet the desired performance criteria, we may revisit earlier phases for further refinement.</p>
    <h3>6. Deployment:</h3>
    <p>We will integrate the trained model into a user-friendly application interface during deployment. This will involve developing a standalone application that allows users to input relevant car features and receive price predictions. We will also create a detailed user guide with instructions on downloading, installing, and using the application. The deployment process will include thorough testing to ensure the application is easy to use and free of major bugs.</p>
    <h2>Implementation Plan:</h2>
    <p>The implementation plan will outline the detailed steps and timeline for developing and deploying the machine-learning solution:</p>
    <ol>
        <li><strong>Data Collection and Preparation (2 weeks):</strong>
            <ul>
                <li>We will collect data from CarDekho</li>
                <li>We will clean and preprocess the data, including filtering relevant records, handling missing values, and removing outliers</li>
            </ul>
        </li>
        <li><strong>Exploratory Data Analysis (1 week):</strong>
            <ul>
                <li>We will analyze the data to understand distributions, correlations, and key features</li>
                <li>We will identify patterns and relationships within the dataset</li>
            </ul>
        </li>
        <li><strong>Model Development (4 weeks):</strong>
            <ul>
                <li>We will develop and train various machine learning models</li>
                <li>We will experiment with different algorithms and parameters to select the best-performing model</li>
            </ul>
        </li>
        <li><strong>Application Development (3 weeks):</strong>
            <ul>
                <li>We will integrate the model into a user-friendly application interface</li>
                <li>We will develop the user interface and ensure it meets user requirements</li>
            </ul>
        </li>
        <li><strong>Testing and Evaluation (2 weeks):</strong>
            <ul>
                <li>We will test the application rigorously to ensure accuracy and reliability</li>
                <li>We will evaluate the model’s performance using metrics such as MAE and R-squared</li>
            </ul>
        </li>
        <li><strong>Deployment and User Training (1 week):</strong>
            <ul>
                <li>We will deploy the application and provide user training sessions</li>
                <li>We will develop a detailed user guide to assist users in installing and using the application</li>
            </ul>
        </li>
        <li><strong>Maintenance and Updates (Ongoing):</strong>
            <ul>
                <li>We will perform regular updates and maintenance to keep the application accurate and reliable</li>
                <li>We will incorporate new data and user feedback to improve the application continuously</li>
            </ul>
        </li>
    </ol>
    <h2>Outcome:</h2>
    <p>The project will result in a robust, reliable, and user-friendly application that leverages advanced machine-learning techniques to predict used car prices accurately. By following the CRISP-DM methodology, Data Science Solutions Inc. will ensure the project is executed systematically and effectively, addressing consumers’ key challenges in the used car market. This comprehensive approach will lead to a high-quality solution that enhances customer satisfaction, builds market trust, and reduces consumer financial risks.</p>
    <p>The project will follow a structured approach to develop a reliable machine-learning solution for predicting used car prices in India. We will begin with data preprocessing by handling missing values, removing outliers, and re-engineering columns like horsepower, mileage, engine capacity, and torque. Exploratory data analysis using Matplotlib, Seaborn, and Plotly will help us identify key factors influencing car prices through visualizations and correlations. Feature engineering will create new variables, such as car age and fuel efficiency metrics, to enhance model performance.</p>
    <p>We will train multiple models, including Random Forest, XGBoost, and Neural Networks, evaluating them with metrics like MAE, RMSE, and R-squared. Hyperparameter tuning using RandomizedSearchCV and GridSearchCV will optimize the models. Finally, we will develop a user-friendly application interface for price predictions, ensuring usability and reliability through thorough testing. This comprehensive approach will result in a high-quality solution that enhances customer satisfaction and trust in the used car market.</p>
    <h2>Timeline:</h2>
    <table border="1">
        <thead>
            <tr>
                <th>Milestone</th>
                <th>Duration (business days)</th>
                <th>Projected Start Date</th>
                <th>Anticipated End Date</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Data Collection and Preparation</td>
                <td>10</td>
                <td>2024-07-01</td>
                <td>2024-07-12</td>
            </tr>
            <tr>
                <td>Exploratory Data Analysis</td>
                <td>5</td>
                <td>2024-07-15</td>
                <td>2024-07-19</td>
            </tr>
            <tr>
                <td>Model Development</td>
                <td>20</td>
                <td>2024-07-22</td>
                <td>2024-08-16</td>
            </tr>
            <tr>
                <td>Application Development</td>
                <td>15</td>
                <td>2024-08-19</td>
                <td>2024-09-06</td>
            </tr>
            <tr>
                <td>Testing and Evaluation</td>
                <td>10</td>
                <td>2024-09-09</td>
                <td>2024-09-20</td>
            </tr>
            <tr>
                <td>Deployment and User Training</td>
                <td>5</td>
                <td>2024-09-23</td>
                <td>2024-09-27</td>
            </tr>
        </tbody>
    </table>
    <h2>Evaluation Plan:</h2>
    <p>During the business understanding phase, we will engage with all relevant stakeholders, including car dealerships, potential buyers, and industry experts, to define the project objectives and requirements. Success in this phase will be verified by achieving a consensus among all parties. This phase will be considered complete and successful once stakeholders agree on the basic design and business objectives. This consensus will ensure that the project aligns with the needs and expectations of all involved parties.</p>
    <p>In the data exploration and processing phases, we will undertake thorough data validation to ensure data quality and relevance. Verification will include checking for null values and ensuring that they are appropriately handled through imputation or removal. We will also identify and remove outliers that could potentially skew model performance. Additionally, we will verify data consistency by ensuring that the dataset contains only relevant records and that unnecessary columns are removed. Ensuring that all data is in the correct format for analysis and model training will be crucial to this process. Specifically, we will re-engineer columns such as horsepower, mileage, engine capacity, and torque to ensure they are suitable for analysis.</p>
    <p>During the model development and testing phase, we will employ multiple verification measures to ensure our models perform as expected. We will calculate performance metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and the coefficient of determination (R-squared) to assess model accuracy and reliability. Cross-validation techniques will be used to evaluate the model’s performance and ensure its robustness. We will also ensure that the machine learning model can be trained without encountering coding errors, indicating correct data processing. The performance of different machine learning models, including Random Forest, XGBoost, and Neural Networks, will be evaluated, and the best-performing model will be selected. Peer reviews and unit testing will be conducted throughout the development process to ensure each section of code works as intended.</p>
    <p>Verification during the user interface (UI) development phase will involve comprehensive testing to ensure usability and integration. We will perform unit testing on individual UI components to confirm their functionality. Integration testing will follow, ensuring seamless interaction between the UI and the machine learning model. Comprehensive system testing will be performed to ensure that all parts of the application work together as intended.</p>
    <p>Once system testing is successful, we will conduct a final acceptance test. This phase will involve user acceptance testing (UAT), where a representative group of users, including car dealerships and customers, will test the application. They will verify that the application meets the specified requirements and performs according to the objectives outlined in the business understanding phase. This final validation will ensure that the system meets the business objectives and effectively solves the presented problem.</p>
    <p>By implementing these detailed verification and validation steps, we will ensure the development of a high-quality machine learning solution that meets the needs of the used car market in India. This project aims to enhance customer satisfaction by providing accurate and reliable car price predictions.</p>
    <h2>Resources and Costs:</h2>
    <table border="1">
        <thead>
            <tr>
                <th>Category</th>
                <th>Description</th>
                <th>Cost</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Hardware and Software Costs</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>Hardware</td>
                <td>High-performance computing resources (cloud or on-premises) for model training and deployment</td>
                <td>(contractor equipment)</td>
            </tr>
            <tr>
                <td>Software</td>
                <td>Licenses for data processing and machine learning tools (e.g., Python libraries, Jupyter notebooks)</td>
                <td>$0</td>
            </tr>
            <tr>
                <td>Estimated Labor Time and Costs</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>Data Scientist</td>
                <td>480 hours @ $100/hour</td>
                <td>$48,000</td>
            </tr>
            <tr>
                <td>Software Developer</td>
                <td>200 hours @ $80/hour</td>
                <td>$16,000</td>
            </tr>
            <tr>
                <td>Project Manager</td>
                <td>100 hours @ $120/hour</td>
                <td>$12,000</td>
            </tr>
            <tr>
                <td>Total Labor Cost</td>
                <td></td>
                <td>$76,000</td>
            </tr>
            <tr>
                <td>Estimated Environment Costs</td>
                <td></td>
                <td></td>
            </tr>
            <tr>
                <td>Deployment and Hosting</td>
                <td>Initial deployment and hosting on cloud platforms</td>
                <td>$5,000</td>
            </tr>
            <tr>
                <td>Maintenance</td>
                <td>Ongoing maintenance and updates per year</td>
                <td>$2,000/year</td>
            </tr>
            <tr>
                <td>Total Project Cost</td>
                <td></td>
                <td>$83,000</td>
            </tr>
        </tbody>
    </table>
    <h1>Part C: Application</h1>
    <p>The application has been developed as a Jupyter Notebook. I will provide the necessary files, including the Jupyter Notebook and the CSV data file used in this project. These files will not be hosted online but will be included in a zip folder for your convenience. This will allow you to review and run the entire application locally.</p>
    <h1>Part D: Post-implementation Report</h1>
    <h2>Solution Summary:</h2>
    <p>The used car market in India faces significant price variability, making it challenging for consumers to determine a fair market value for vehicles. This variability can lead to consumer dissatisfaction, lack of trust in the market, and potential financial losses. Addressing this challenge required a solution that could provide reliable price estimates, thereby enhancing market transparency and consumer confidence.</p>
    <p>The solution developed was a sophisticated machine learning-based application designed to predict the sale price of used cars accurately. This application processed a comprehensive dataset of historical car sales and used advanced machine-learning techniques to provide precise and reliable price predictions. The objective was to enable consumers to make informed purchasing decisions and to help build trust in the market.</p>
    <h2>Application Features:</h2>
    <ul>
        <li>Data Processing: The application involved extensive data cleaning, normalization, and feature engineering to prepare the dataset for model training</li>
        <li>Machine Learning Models: Multiple machine learning models were developed, trained, and evaluated to ensure the best possible performance</li>
        <li>Predictive Accuracy: The application aimed to minimize the difference between actual sale prices and predicted prices using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-squared (R²)</li>
    </ul>
    <p>The application processed a large dataset of historical car sales, incorporating over 5,000 records of used car sales from across India. Each record in the dataset included various features relevant to the car’s value.</p>
    <h2>Data Summary:</h2>
    <p>The dataset utilized in this project was obtained from CarDekho, a prominent car search platform in India that helps users find the perfect vehicles for their needs. It included comprehensive records of used car sales in India, detailing variables such as car model, year of manufacture, selling price, kilometers driven, fuel type, transmission type, owner history, mileage, engine capacity, maximum power, torque, and number of seats.</p>
    <p>A view of the data in an organized format in Jupyter Notebooks:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/1d719f04-fa0c-4d88-9d50-67b16fca5259" alt="Data View 1">
    <p>This is the view of the scraped data in CSV:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/a4e9f3e7-17b2-4df5-a94f-aab5357e88b2" alt="Data View 2">
    <h2>Data Processing:</h2>
    <h3>Data Collection and Initial Processing:</h3>
    <p>The data was initially filtered to focus on relevant records, removing those with incomplete data or non-standard features. This step ensured that the dataset was manageable and relevant for the machine learning model. For example, records missing key details such as the car model, year, or selling price were excluded to maintain data quality and integrity.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/6fa05ee8-3c22-4f51-a66c-1ec7f16905da" alt="Data Filtering">
    <h3>Data Cleaning:</h3>
    <p>Missing values were handled through imputation or removal, and outliers were detected and removed to avoid skewing the model’s performance. For instance, records with exceptionally high prices or extreme mileage were analyzed and excluded if necessary. Outlier removal example:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/f280c0e5-74fe-4475-95f0-5a9556c0c8f7" alt="Data Cleaning">
    <p>After imputation, no nulls were present in the dataset:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/ea00fc91-ef00-4dcf-8bd7-b3cae87b8f68" alt="Data Imputation">
    <p>Through comprehensive preprocessing, the dataset was prepared for machine learning by splitting it into training and test sets. The dataset was divided into features (X) and target (y) variables. The features encompassed various factors such as kilometers driven, engine capacity, fuel type, and transmission type, while the target variable was the car’s sale price. The training set was utilized to train the machine learning model, and the test set was employed to assess the model’s performance.</p>
    <h3>Normalization and Feature Engineering:</h3>
    <p>Continuous variables such as kilometers driven and engine capacity were normalized. Feature engineering was conducted to create new features from existing ones, such as calculating the car’s age from its manufacturing year.</p>
    <p>As a good illustrative and complex example, the torque column represented significant challenges due to its inconsistent format and various units of measurement. The raw data included torque values expressed in different units and formats, making direct comparisons impossible. For example, some values were given in Newton meters (Nm), while others were in kilogram meters (kgm).</p>
    <p>Additionally, the values included different ranges and annotations, such as RPM (revolutions per minute), which further complicated the data, making it difficult to compare numbers directly. Without addressing these inconsistencies, the machine learning model’s ability to make accurate predictions would be impeded. A quick Google search confirmed that the torque column was a significant factor and could not be ignored, emphasizing the importance of its inclusion and proper standardization.</p>
    <p>Here are some examples from the torque column to illustrate its inconsistencies:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/00f867be-e610-4b13-8adb-612372cd30b4" alt="Torque Values">
    <p>The data had to be converted into the same format to be able to conduct true comparisons. First, the torque types were broken into categories:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/f83ce071-ed2a-4ff5-a710-eab99547f096" alt="Torque Categories">
    <p>To further illustrate the normalization process for this column, torque values were categorized by units (e.g., Nm, kgm), then converted to Newton meters (Nm) using conversion factors like 1 kgm = 9.8 Nm. After normalization to ensure consistency, the standardized torque values replaced the original entries in the dataset.</p>
    <p>Following a series of complex data processing operations as described shortly above, the inconsistent torque values were standardized and integrated into the newly designated updated_torque column:</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/ec6cd1bf-b4fc-4ff6-9f8d-960dd3e5f907" alt="Torque Normalization"> <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/caa9928d-e687-4cd4-8781-1adee8ed2858" alt="Torque Normalization">
    <h3>Data Management:</h3>
    <p>Data management involves regularly updating the dataset to incorporate new records and reflect the latest market trends.</p>
    <h2>Machine Learning:</h2>
    <p>Machine learning was applied in a predictive manner to estimate the sale price of used cars based on various car features. The dataset includes information on car features such as the model, year, kilometers driven, fuel type, and transmission type. This information is used by the machine learning model to predict the car’s selling price.</p>
    <p>In general, a supervised learning regression algorithm was needed to predict used car prices because the target variable, the car’s sale price, is continuous, and the target values were known. The Random Forest Regressor algorithm from the scikit-learn library was chosen for this project due to its high accuracy for regression tasks and its ability to prevent overfitting. This ensemble method utilizes multiple independent decision trees, averaging their predictions to produce a more reliable estimate (Anticipation of Car Price Using Machine Learning Approach, 2023). The algorithm’s bagging technique, which trains each tree on different slices of the training set, helps to reduce overfitting. Linear Regression was considered but found to be less accurate, thus it was not used (Car Price Prediction: An Application of Machine Learning, 2023).</p>
    <p>The development process began with collecting and processing data on used car sales from CarDekho, India’s leading online car marketplace. Python was selected to develop the machine learning model due to its robust support for data processing and machine learning. The pandas library was used to read the dataset from a CSV file into a DataFrame. Data exploration was conducted using pandas, seaborn, and matplotlib to visualize feature distributions and correlations. These visualizations guided the data cleaning process, revealing outliers and incorrect data types that were subsequently corrected.</p>
    <p>Once the data was cleaned and prepared, it was split into training and test sets using the train_test_split function from scikit-learn, with 80% of the data for training and 20% for testing. The random_state parameter was used to ensure consistent data shuffling, enabling controlled model evaluation. Different feature combinations were tested to optimize the independent variable set. The final set of features included car model, year, kilometers driven, fuel type, transmission type, engine capacity, and more.</p>
    <p>A Random Forest Regressor from the scikit-learn library was trained using the dataset, and its predictions were compared to the actual selling prices of used cars (Zhu, 2023). The model’s performance was measured using several metrics: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R2). The Random Forest model achieved an R2 score of 0.9609, indicating it could explain about 96% of the variance in car prices (Car Price Prediction: An Application of Machine Learning, 2023). The MAE was 1067.21, showing the average difference between the predicted and actual prices was around $1067. The RMSE was 2220.44, reflecting the model’s prediction errors.</p>
    <p>The XGBoost model was also evaluated and showed even better performance, with an R2 score of 0.9975, an MAE of 397.08, and an RMSE of 563.94. Additionally, the Random Forest model had a cross-validation score of 0.9561, suggesting it can generalize well to new data. These results highlight the effectiveness of both models, with the Random Forest model providing a strong balance between accuracy and interpretability.</p>
    <p>Through this comprehensive approach, the machine learning model was successfully developed to predict used car prices with high accuracy, enhancing the transparency and reliability of the used car market in India.</p>
    <h3>Overview of Code Implementation for Predicting Used Car Prices</h3>
    <h3>Data Collection and Initial Processing</h3>
    <p>The project began by importing the required libraries for Exploratory Data Analysis (EDA) and data preparation, including pandas, numpy, matplotlib, seaborn, and scikit-learn. The dataset, sourced from CarDekho, was read into a pandas DataFrame.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/0e9e5d93-998e-486c-9981-db6e555d4573" alt="Code Implementation 1">
    <h3>Data Exploration and Cleaning</h3>
    <p>The target variable, selling_price, was analyzed using histograms. A logarithmic transformation was applied to scale the target variable. The dataset was then checked for null values and outliers, which were handled accordingly.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/c82cc481-f609-4350-a73b-f1ca39e52c89" alt="Code Implementation 2">
    <h3>Feature Engineering</h3>
    <p>Feature engineering involved converting relevant columns to appropriate data types and handling inconsistent formats, especially in the torque column. Missing values were imputed using the median.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/514d7faa-d039-470c-b327-57bf4870fce5" alt="Code Implementation 3">
    <h3>Data Normalization and Splitting</h3>
    <p>The data was normalized using the StandardScaler, and then split into training and test sets.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/c9e6bcb1-a3ce-495d-a356-86c672048407"
 alt="Code Implementation 4">
    <h3>Model Training and Evaluation</h3>
    <p>Multiple regression models, including Random Forest, Linear Regression, SVR, Decision Tree, XGBoost, and Gradient Boosting, were trained and evaluated. The Random Forest Regressor showed the best performance.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/0c3c2002-0822-4dbb-883d-1add2634a671" alt="Code Implementation 5">
    <h3>Hyperparameter Tuning</h3>
    <p>Hyperparameter tuning was performed for the best-performing models, Random Forest and XGBoost, to further optimize their performance.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/df915694-9811-44ae-ab52-388ef4fbd088" alt="Code Implementation 6"> <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/4b56754d-5ec0-4bb9-9696-86df621cdbaf" alt="Code">
    <h3>Results</h3>
    <p>The Random Forest Regressor was identified as the best model with high accuracy, and its performance metrics were recorded.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/ceb68494-4164-43a0-ad23-f620e07caf25" alt="Code Implementation 7"> <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/52338cd3-3770-4f32-8a39-491feb91198a" alt="Code Implementation 7">
    <p>Through this comprehensive approach, a robust machine learning model was developed to accurately predict used car prices, enhancing market transparency and consumer trust.</p>
    <h2>Validation</h2>
    <p>Three methods were used to assess the accuracy of the model:</p>
    <h3>1. R2 Score:</h3>
    <p>The built-in score function for the Random Forest Regressor was used to evaluate the performance of the test set data given to the trained model. According to the scikit-learn API documentation, the score method calculates the R2 value, which is the coefficient of determination. For the Random Forest model, the R2 score was calculated as 0.9609, indicating that the model could explain approximately 96.09% of the variance in the car prices. This score was consistently calculated to be around 0.96 each time the model was trained and tested. The XGBoost model achieved an even higher R2 score of 0.9975, indicating excellent predictive performance.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/61e60402-c5ff-4ee6-830d-728a3ebcec43" alt="R2 Score">
    <h3>2. Mean Absolute Error (MAE):</h3>
    <p>This metric is straightforward to interpret as it indicates the average amount, in dollars, that the predictions deviated from the actual values. For the Random Forest model, the MAE was 1067.21, meaning that, on average, the model’s predictions were off by about $1067. The XGBoost model achieved a lower MAE of 397.08, indicating more accurate predictions.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/1afaa4f9-a861-486a-b690-557a869da5b3" alt="MAE">
    <h3>3. Root Mean Squared Error (RMSE):</h3>
    <p>RMSE is a measure of the differences between predicted values by a model and the actual values. For the Random Forest model, the RMSE was 2220.44, and for the XGBoost model, it was 563.94. These values give an indication of the model’s accuracy, with lower values representing better performance.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/61bac199-9814-4d28-b49b-25c5b5924917" alt="RMSE">
    <h3>4. Cross-Validation (CV) Score:</h3>
    <p>The cross-validation score helps to evaluate the model’s performance across different subsets of the data. For the Random Forest model, the CV accuracy score was approximately 0.9561. This consistency across multiple folds indicates that the model generalizes well to unseen data. The XGBoost model also showed strong performance with a mean CV score of 0.95 on the training set.</p>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/859f3d0d-63b5-45a9-8723-b3f091fd350a" alt="CV Score">
    <h3>Summary of Results:</h3>
    <p>Random Forest:</p>
    <ul>
        <li>R2 Score: 0.9609</li>
        <li>MAE: 1067.21</li>
        <li>RMSE: 2220.44</li>
        <li>CV Accuracy Score: 0.9561</li>
    </ul>
    <p>XGBoost:</p>
    <ul>
        <li>R2 Score: 0.9975</li>
        <li>MAE: 397.08</li>
        <li>RMSE: 563.94</li>
    </ul>
    <p>These results demonstrate that both the Random Forest and XGBoost models performed well in predicting used car prices. However, the Random Forest model was ultimately chosen for its balance of performance metrics and interpretability. While XGBoost exhibited slightly better overall accuracy and lower error rates, the Random Forest model consistently provided reliable predictions across different subsets of the data.</p>
    <p>The Random Forest model’s lower complexity compared to XGBoost made it a more robust choice against overfitting. Its ensemble method, which involves averaging the predictions of multiple independent decision trees, ensures that it captures a wide range of patterns in the data without becoming overly sensitive to noise. This characteristic is crucial for maintaining model stability and reliability, particularly when dealing with diverse and potentially noisy datasets like those of used car prices.</p>
    <p>Furthermore, the Random Forest model demonstrated strong generalization capabilities, as evidenced by its consistent performance in cross-validation. The model’s ability to generalize well across different data folds indicates that it can make accurate predictions on new, unseen data. This consistency is essential for practical applications where the model needs to perform reliably in various real-world scenarios.</p>
    <p>In addition to its technical strengths, the interpretability of the Random Forest model played a significant role in its selection. The model’s structure allows for a straightforward examination of feature importance, making it easier to understand which car features most influence the predicted prices. This transparency is valuable for stakeholders who need to trust and verify the model’s decisions, such as car dealers, buyers, and market analysts.</p>
    <p>Overall, the Random Forest model’s combination of reliable performance, robustness against overfitting, strong generalization ability, and interpretability made it the preferred choice for predicting used car prices. Its adoption is expected to enhance market transparency and consumer trust by providing accurate and understandable price predictions.</p>
    <h2>Visualizations</h2>
    <p>To better understand the used car market and the factors influencing prices, we conducted extensive data exploration and visualization. The following visualizations highlight key patterns, distributions, and correlations that guided our model development and feature engineering. While there are many more visualizations in the analysis, these selected examples underscore important findings:</p>
    <h3>1. Histogram of Selling Price:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/a283dc70-1db6-48d6-8c8d-fbe9390c05e4" alt="Histogram of Selling Price">
    <h3>2. Histogram of Log of Selling Price:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/78124993-5a04-47ac-a9c8-a9421a73db10" alt="Histogram of Log of Selling Price">
    <h3>3. Heatmap of Correlations Among Numeric Features:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/7afba623-4a62-4260-8bf5-f2d85c197abb" alt="Heatmap of Correlations">
    <h3>4. Pair Plot of Features:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/57942578-faef-4026-b341-6523be447bbf" alt="Pair Plot of Features">
    <h3>5. Bar Plot of Selling Price by Vehicle Year:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/d1724690-d8c3-47a4-aa95-4e30c9d0444f" alt="Bar Plot of Vehicle Year">
    <h3>6. Pie Chart of Top 10 Car Brands Sold:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/00b00cd0-3808-4983-8908-f9f424d0ed5a" alt="Pie Chart of Car Brands">
    <h3>7. Bar Plot of Kms Driven by Fuel Type:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/8f59bdbf-b1d6-4d0f-8a61-fb687d085a13" alt="Bar Plot of Kms by Fuel Type">
    <h3>8. Scatter Plot of Relationship Between Torque Power and Selling Price:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/73479e3c-a58d-4bb5-80e6-3989d76c0465"
 alt="Scatter Plot of Torque and Selling Price">
    <h3>9. Distribution of Selling Prices by Fuel Type:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/88fc72dc-5d7a-476b-a36b-8e6cdc3f7b8f" alt="Distribution of Selling Prices by Fuel Type">
    <h3>10. Car Brand Popularity:</h3>
    <img src="https://github.com/MayCooper/Product-Price-Prediction/assets/82129870/48ba2c53-4425-4127-b15a-329198c84aef" alt="Car Brand Popularity">
    <h2>User Guide</h2>
    <h2>User Guide for Predicting Used Car Prices</h2>
    <p>Welcome to the User Guide for the Used Car Price Prediction project! This guide will walk you through the steps to load the provided Jupyter Notebook (<code>Capstone Project_Used Car Price Prediction_May Cooper</code>) and the associated CSV file (<code>Car_details_v3.csv</code>) into Jupyter Notebooks and run the project.</p>
    <h3>Prerequisites</h3>
    <p>Before you begin, ensure you have the following installed on your machine:</p>
    <ul>
        <li>Python 3.x</li>
        <li>Jupyter Notebook</li>
        <li>Required Python libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, plotly, xgboost, tensorflow</li>
    </ul>
    <p>If you do not have these libraries installed, you can install them using pip:</p>
    <pre><code>pip install pandas numpy matplotlib seaborn scikit-learn plotly xgboost tensorflow</code></pre>
    <h3>Option 1: Using Jupyter Notebook</h3>
    <h4>1. Download the Files:</h4>
    <ul>
        <li>Ensure you have downloaded the following files:</li>
        <ul>
            <li><code>Capstone Project_Used Car Price Prediction_May Cooper</code></li>
            <li><code>Car_details_v3.csv</code></li>
        </ul>
    </ul>
    <h4>2. Open Jupyter Notebook:</h4>
    <ul>
        <li>Open a terminal or command prompt.</li>
        <li>Navigate to the directory where you have saved the downloaded files.</li>
        <li>Start Jupyter Notebook by running:</li>
        <pre><code>jupyter notebook</code></pre>
        <li>This will open the Jupyter Notebook interface in your web browser.</li>
    </ul>
    <h4>3. Load the Notebook:</h4>
    <ul>
        <li>In the Jupyter Notebook interface, navigate to the directory where the <code>Capstone Project_Used Car Price Prediction_May Cooper</code> file is located.</li>
        <li>Click on the <code>Capstone Project_Used Car Price Prediction_May Cooper</code> file to open it.</li>
    </ul>
    <h4>4. Run the Notebook:</h4>
    <ul>
        <li>The notebook is organized into cells. To run the cells:</li>
        <ul>
            <li>Click on the first cell.</li>
            <li>Press <code>Shift + Enter</code> to execute the cell and move to the next one.</li>
            <li>Continue pressing <code>Shift + Enter</code> to run all the cells sequentially.</li>
            <li>Alternatively, you can run all cells at once by selecting <code>Cell</code> -> <code>Run All</code> from the menu.</li>
        </ul>
    </ul>
    <h3>Option 2: Using Anaconda</h3>
    <h4>1. Download and Install Anaconda:</h4>
    <ul>
        <li>Download Anaconda from the official website: <a href="https://www.anaconda.com/products/individual">https://www.anaconda.com/products/individual</a> and follow the installation instructions for your operating system.</li>
    </ul>
    <h4>2. Open Anaconda Navigator:</h4>
    <ul>
        <li>Launch Anaconda Navigator from your applications menu.</li>
    </ul>
    <img src="anaconda_navigator.png" alt="Anaconda Navigator">
    <h4>3. Launch Jupyter Lab/Notebook:</h4>
    <ul>
        <li>In Anaconda Navigator, click on the <code>Launch</code> button under the Jupyter Lab/Notebook section.</li>
        <li>This will open Jupyter Lab in your web browser.</li>
        <li>Note: Both Jupyter Lab and Jupyter Notebook will work.</li>
    </ul>
    <h4>4. Load the Notebook:</h4>
    <ul>
        <li>In the Jupyter Lab interface, navigate to the directory where the <code>Capstone Project_Used Car Price Prediction_May Cooper</code> file is located.</li>
        <li>Click on the <code>Capstone Project_Used Car Price Prediction_May Cooper</code> file to open it.</li>
    </ul>
    <img src="jupyter_lab_interface.png" alt="Jupyter Lab Interface">
    <p>The car details csv in the same directory:</p>
    <img src="csv_directory.png" alt="CSV Directory">
    <h4>5. Run the Notebook:</h4>
    <ul>
        <li>Follow the same steps as described in Option 1 to run the notebook cells.</li>
    </ul>
    <h3>What to Expect</h3>
    <p>The notebook performs the following tasks:</p>
    <ol>
        <li><strong>Import Libraries:</strong> Imports necessary Python libraries for data processing, visualization, and machine learning.</li>
        <li><strong>Load and Explore the Data:</strong> Loads the <code>Car_details_v3.csv</code> dataset and performs initial data exploration, including viewing the dataset’s structure and summary statistics.</li>
        <li><strong>Data Cleaning and Feature Engineering:</strong> Handles missing values and outliers, performs feature engineering to create new variables and convert data types as needed.</li>
        <li><strong>Data Visualization:</strong> Generates various visualizations to explore the relationships between features and the target variable (selling price).</li>
        <li><strong>Data Preprocessing:</strong> Normalizes the data and splits it into training and test sets.</li>
        <li><strong>Model Training and Evaluation:</strong> Trains multiple regression models (Random Forest, Linear Regression, SVR, Decision Tree, XGBoost, and Gradient Boosting) and evaluates the performance of each model using metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (R2).</li>
        <li><strong>Hyperparameter Tuning:</strong> Performs hyperparameter tuning for the best-performing models to optimize their performance.</li>
        <li><strong>Results and Visualizations:</strong> Provides detailed performance metrics and visualizations for the trained models.</li>
    </ol>
    <p>Important Notes:</p>
    <ul>
        <li>Ensure that the CSV file (<code>Car_details_v3.csv</code>) is in the same directory as the Jupyter Notebook file (<code>Capstone Project_Used Car Price Prediction_May Cooper</code>) to avoid file path issues.</li>
        <li>Running all the cells will generate visualizations and model performance metrics. Take the time to review each section to understand the data processing, model training, and evaluation steps.</li>
        <li>If you encounter any issues or errors while running the notebook, make sure all necessary libraries are installed and that the CSV file is correctly loaded.</li>
        <li>Please Note: The cell that involves training machine learning models, particularly the hyperparameter tuning cell, can take an hour or more to run, depending on your computer’s processing power and whether you have a dedicated GPU.</li>
    </ul>
    <p>By following this guide, you should be able to successfully run the project and gain insights into predicting used car prices using machine learning models.</p>
    <h2>References:</h2>
    <ul>
        <li>Anticipation of Car Price Using Machine Learning Approach. (2023, May 8). IJRASET; IJRASET. Retrieved June 12, 2024, from <a href="https://www.ijraset.com/research-paper/anticipation-of-car-price-using-machine-learning-approach">https://www.ijraset.com/research-paper/anticipation-of-car-price-using-machine-learning-approach</a></li>
        <li>Car Price Prediction: An Application of Machine Learning. (2023, April 26). IEEE Conference Publication | IEEE Xplore. <a href="https://ieeexplore.ieee.org/document/10134142">https://ieeexplore.ieee.org/document/10134142</a></li>
        <li>Zhu, Y. (2023). Prediction of the price of used cars based on machine learning algorithms. Applied and Computational Engineering, 6(1), 671–677. <a href="https://doi.org/10.54254/2755-2721/6/20230917">https://doi.org/10.54254/2755-2721/6/20230917</a></li>
    </ul>
</body>
</html>
