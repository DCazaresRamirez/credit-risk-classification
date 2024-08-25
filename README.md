   <h1>Analysis</h1>
    <p>In this analysis, we assessed the performance of a logistic regression model to predict loan risk, using historical lending activity data. The primary goal was to identify the creditworthiness of borrowers by predicting whether a loan is high-risk (label 1) or healthy (label 0).</p>
    
   <h2>Financial Information and Prediction Goals:</h2>
    <ul>
        <li><strong>Data Information:</strong> The dataset contains information on historical lending activities, including loan statuses, which indicate whether a loan was considered high-risk or healthy.</li>
        <li><strong>Prediction Goal:</strong> We aimed to predict the binary outcome of loan status: 0 (healthy loan) or 1 (high-risk loan).</li>
    </ul>
    
   <h2>Variables of Interest:</h2>
    <ul>
        <li><strong>Loan Status (Target Variable):</strong> This is a binary variable where:
            <ul>
                <li><strong>Value Counts for Label 0:</strong> 18,765 instances (healthy loans)</li>
                <li><strong>Value Counts for Label 1:</strong> 619 instances (high-risk loans)</li>
            </ul>
        </li>
    </ul>
    
   <h2>Machine Learning Process Stages:</h2>
    <ol>
        <li><strong>Data Preparation:</strong>
            <ul>
                <li>Loaded the dataset and reviewed its structure.</li>
                <li>Separated the target variable (<code>loan_status</code>) from the feature variables.</li>
                <li>Split the dataset into training and testing sets.</li>
            </ul>
        </li>
        <li><strong>Model Training:</strong>
            <ul>
                <li>Implemented a Logistic Regression model to classify loan risk.</li>
                <li>Fitted the model using the training dataset.</li>
            </ul>
        </li>
        <li><strong>Model Evaluation:</strong>
            <ul>
                <li>Generated predictions using the test dataset.</li>
                <li>Evaluated model performance using a confusion matrix and classification report.</li>
            </ul>
        </li>
    </ol>
    
   <h2>Methods Used:</h2>
    <ul>
        <li><strong>Logistic Regression:</strong> A statistical model used for binary classification tasks, in this case, to predict loan risk.</li>
    </ul>
    
   <h1>Results</h1>
    
   <h2>Machine Learning Model 1: Logistic Regression</h2>
    <ul>
        <li><strong>Accuracy:</strong> 0.99
            <ul>
                <li>The model correctly predicted 99% of the cases.</li>
            </ul>
        </li>
        <li><strong>Precision for Healthy Loans (Label 0):</strong> 1.00
            <ul>
                <li>The model accurately identified all but a few healthy loans.</li>
            </ul>
        </li>
        <li><strong>Recall for Healthy Loans (Label 0):</strong> 0.99
            <ul>
                <li>The model captured 99% of the actual healthy loans.</li>
            </ul>
        </li>
        <li><strong>Precision for High-Risk Loans (Label 1):</strong> 0.85
            <ul>
                <li>The model had some false positives, misclassifying a few healthy loans as high-risk.</li>
            </ul>
        </li>
        <li><strong>Recall for High-Risk Loans (Label 1):</strong> 0.91
            <ul>
                <li>The model identified 91% of the actual high-risk loans.</li>
            </ul>
        </li>
    </ul>
    
   <h1>Summary</h1>
    <p>The logistic regression model demonstrates excellent performance overall, with a high accuracy rate and strong precision and recall scores. It performs exceptionally well in predicting healthy loans and reasonably well for high-risk loans.</p>
    
   <h2>Recommendation:</h2>
    <ul>
        <li><strong>Best Performing Model:</strong> The logistic regression model seems to perform best based on the provided metrics. It provides high accuracy and good recall, especially for healthy loans.</li>
        <li><strong>Performance Consideration:</strong> Given that high recall is crucial for identifying high-risk loans (to avoid missing any potentially problematic loans), the model’s performance is satisfactory, though precision could be improved.</li>
    </ul>
    
   <p><strong>Conclusion:</strong> The logistic regression model is recommended for predicting loan risk due to its high accuracy and strong performance metrics. If precision for high-risk loans is a critical requirement, additional methods or adjustments could be explored to further enhance model performance.</p>
