# ACE---Vizdetect
Problem Statement
What is the problem?
Organizations, especially businesses and financial institutions, face challenges in detecting anomalies such as fraudulent transactions, operational errors, 
or irregularities in their data. Existing manual or semi-automated methods are inefficient, time-consuming, and prone to errors.

Why does it matter?
Undetected anomalies can lead to significant financial losses, compromised data integrity, and missed opportunities to prevent fraud or errors. 
This directly impacts decision-making, operational efficiency, and trust in the organization's data systems.

Who is affected?
Businesses, financial institutions, analysts, and decision-makers who rely on transactional data for operations are most affected. 
Small-to-medium enterprises (SMEs) often lack the tools or expertise to analyze large datasets efficiently, leaving them vulnerable to data anomalies and fraudulent activity

Solution Overview (K.I.S.S – Keep It Short and Simple)
What is your solution?
The One-Click Anomaly Detection System is a user-friendly tool that leverages machine learning to quickly and accurately identify anomalies in transactional data.

How does it solve the problem?
By allowing users to upload a CSV file with transactional data, the system automatically analyzes and detects irregularities using the Isolation Forest algorithm. It highlights anomalies and presents results visually, eliminating manual effort, saving time, and ensuring accuracy.

What makes it special?

One-Click Simplicity: No technical expertise is required. Just upload your data.
Speed & Accuracy: Detects anomalies in minutes with high precision.
User-Friendly Interface: Intuitive visualization of results for easy understanding.
Scalable: Handles large datasets (up to 200MB), making it suitable for SMEs and enterprises alike.



Technical Implementation
Tools and Frameworks:

Streamlit: User-friendly web interface for data upload and visualization.
Python Libraries: pandas, scikit-learn, matplotlib for data processing, ML, and visualization.
Isolation Forest Algorithm: Machine learning model to detect anomalies based on feature scaling.
ngrok: Tunnels to host and test the app online for easy sharing.
Workflow:


The link sometimes doesn't connect to the server , we recommend to test it in google colab 

Input: Transactional data with Time and Amount features.
Preprocessing: Standardizes data using StandardScaler.
Detection: Trains Isolation Forest to flag anomalies (contamination rate: 1%).
Output: Classifies data as "Normal" or "Anomaly," and visualizes the results.
Deployment: Runs seamlessly via Streamlit, and can be accessed globally through an ngrok tunnel.

