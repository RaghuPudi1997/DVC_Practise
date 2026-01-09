**This repository demonstrates Data Version Control (DVC) basics and how data versioning works in an MLOps workflow.**
1. First I took a Sample Data Set (Wine Prediction Model) a sample .csv file for practise
2. # Next I have created the Python virtual environmnet using the Anaconda and activated the virtual Environment
   conda create -p venvw python==3.12
3. # Next I have installed the dvc for the Google cloud Storage
   python -m pip install dvc_gs
4. # Now initialise and add the dataset file so it creates .dvc file which includes the checksum of the dataset
   dvc init
   dvc add *****.scv
5. # Create the bucket in the Google Cloud Platform and assign the necessary permissions so that you can push the dataset to the cloud storage using dvc push
   <img width="754" height="227" alt="image" src="https://github.com/user-attachments/assets/9d8ca142-ee2e-4e08-99ff-deb58f641e89" />


* The main understanding point is we are storing the pointer to the dataset in git and the actual dataset which can range from GB's to TB's in the remote GCP Cloud Storage**
  So whenever someone wants to check currently what is the latest version we can go to ****.dvc to see the checksum and to know where it is located they can go to .dvc/config folder*
