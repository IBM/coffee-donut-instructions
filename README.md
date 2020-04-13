# Build and Deploy an image classifier on IBM Cloud
## This hands-on lab builds a neural network to predict an input image as that of coffee, donut or a mug.

### 1. Search for Watson Studio service on IBM Cloud
![](images/create-watson-studio.png)

### 2. Create a Watson Studio instance
![](images/create-watson-studio-instance.png)

### 3. Click on `Getting Started` to launch Watson Studio
![](images/launch-watson-studio.png)

### 4. Start creating a `New Project` inside Watson Studio
![](images/start-new-project.png)

### 5. Create a project from a sample or file
![](images/create-from-sample.png)

### 6. Create new storage service
![](images/create-new-storage-service.png)

### 7. You can leave the defaults and click on `Create`
![](images/create-new-storage-service-defaults.png)

### 8. Upload the sample file to create the new project. You can find the sample zip file under [assets/coffee-donut.zip](assets/coffee-donut.zip).
![](images/upload.sample.png)

### 9. Finish uploading file and create new project
![](images/finish-creating-project.png)

![](images/project-in-process.png)

### 10. Once the project has finished, view project to see details
![](images/viewproject.png)

### 11. Open `Assets` section. This is where you will find the data and notebooks
![](images/assets.png)

### 12. Scroll down to `Notebooks` and open the `Train a sample classifier` notebook
![](images/open-notebook.png)

### 13. If your note is in read-only mode, use the pencil button to edit the notebook
![](images/edit-notebook.png)

### 14. This will instantiate a new runtime for you to run the notebook
![](images/notebook-runtime.png)

### 15. You can now run the cells to create the neural network!
![](images/run-notebook.png)


## Additional clarifications for the notebook

### 1. Adding credentials to the notebook
![](images/notebook-cos-credentials-insert.png)

### 2. Using credentials in the notebook. Make sure you change the variable name to what was assigned in the last step when you added credentials to the notebook
![](images/notebook-cos-credentials-variable.png)