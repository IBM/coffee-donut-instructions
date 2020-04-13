# Build and Deploy an image classifier on IBM Cloud
This hands-on lab builds a neural network to predict an input image as that of coffee, donut or a mug.

The workshop provides you with all the data and assets you need to create the classifier on IBM Cloud. To get started, you can close this github repo or simply download the sample file under [assets/coffee-donut.zip](assets/coffee-donut.zip). You do not need to unzip the file, but simply upload it to Watson Studio as explained in the steps below. The zip file contains the following assets

```
assets
├── data_asset
│   ├── Coffee\ Bag\ 2.jpg
│   ├── Coffee.jpg
│   ├── Donut.jpg
│   ├── Mug.jpg
│   └── coffee-donuts-segregated.zip
└── notebook
    └── notebook:Train_a_simple_classifier_dam9_4_n1.ipynb
```
- data_asset/coffee-donuts-segregated.zip - this is your training data 
- data_asset/*.jpg - test images used to predict with the model
- Train_a_simple_classifier_dam9_4_n1.ipynb - this is the sample notebook that is used to train your image classifier.


## Prerequisites
1. This workshop assumes you have an IBM Cloud account. Please ask the workshop facilitator for the URL to sign up. If you don't have a unique URL, you can [register here](https://ibm.biz/Bdq2TN) - https://ibm.biz/Bdq2TN. 
2. Download [assets/coffee-donut.zip](assets/coffee-donut.zip) file that will be used as a template in this workshop.

## Technologies Used
1. [IBM Watson Studio](https://www.ibm.com/cloud/watson-studio) - helps data scientists and analysts prepare data and build models at scale 
2. [IBM Cloud Object Store](https://www.ibm.com/cloud/object-storage) - stores large volumes of unstructured data while still ensuring scalability, security, availability, reliability, manageability, and flexibility.
3. [Jupyter Notebooks](https://developer.ibm.com/clouddataservices/docs/ibm-data-science-experience/notebooks/) - provides a collaborative environment and runtimes that enables Python, Scala, and R notebooks

## Steps

1. Search for Watson Studio service on IBM Cloud in the Catalog or using the search bar as shown here
   
    ![](images/create-watson-studio.png)

1. Create a Watson Studio instance
   
    ![](images/create-watson-studio-instance.png)

1. Click on `Get Started` to launch Watson Studio

    ![](images/launch-watson-studio.png)

1. Start creating a `New Project` inside Watson Studio

    ![](images/start-new-project.png)

1. Create a project from a sample or file

    ![](images/create-from-sample.png)

1. Create a new storage service
    
    ![](images/create-new-storage-service.png)

1. You can leave the defaults and click on `Create`

    ![](images/create-new-storage-service-defaults.png)

1. Upload the sample file to create the new project. You can find the sample zip file under [assets/coffee-donut.zip](assets/coffee-donut.zip)
    
    ![](images/upload.sample.png)

1. Finish uploading file and create a new project
    
    ![](images/finish-creating-project.png)

    ![](images/project-in-process.png)

1.  Once the project has been created, view project to see details
    
    ![](images/viewproject.png)

1.  Open `Assets` tab. This is where you will find the data and notebooks
    
    ![](images/assets.png)

1.  Scroll down to `Notebooks` and open the `Train a sample classifier` notebook
    
    ![](images/open-notebook.png)

1.  If your notebook is in read-only mode, use the pencil button to edit the notebook
    
    ![](images/edit-notebook.png)

1.  This will instantiate a new runtime for you to run the notebook
    
    ![](images/notebook-runtime.png)

1.  You can now run the cells to create the neural network!
    
    ![](images/run-notebook.png)


## Additional clarifications for the notebook

1. In order to use the data from the cloud object store in the notebook, use the `0100` data tab on the right side as show in the image below. You can use `insert credentials` link from the `coffee-donuts-segregated.zip` asset. This will insert some code in the notebook that provide you access to the credentials as a dictionary.
    
    ![](images/notebook-cos-credentials-insert.png)
    

2. The credentials generated in the cell above will be stored in  a variable with a name like `credentials_number`. Assign it to `credentials` variable in the next cell. This `credentials` variable will be used in the rest of the notebook.

    ![](images/notebook-cos-credentials-variable.png)