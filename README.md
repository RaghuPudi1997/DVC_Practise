**This repository demonstrates Data Version Control (DVC) basics and how data versioning works in an MLOps workflow.**
1. First I took a Sample Data Set (Wine Prediction Model) a sample .csv file for practise
2. # Next I have created the Python virtual environmnet using the Anaconda and activated the virtual Environment
   conda create -p venvw python==3.12
3. # Next I have installed the dvc for the Google cloud Storage
   python -m pip install dvc_gs
4. # Now initialise and add the dataset file so it creates .dvc file which includes the checksum of the dataset
   dvc init
   dvc add *****.scv
5. # Create the bucket in the Google Cloud Platform and assign the necessary permissions so that you can push the dataset to the cloud storage using
   dvc push
   <img width="754" height="227" alt="image" src="https://github.com/user-attachments/assets/9d8ca142-ee2e-4e08-99ff-deb58f641e89" />
   

