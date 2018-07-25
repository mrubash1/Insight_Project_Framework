# Insight_Project_Framework
Framework for machine learning projects at Insight Data Science
![Pipeline](https://github.com/mrubash1/Insight_Project_Framework/blob/master/static/example-data-pipeline.png)
Motivation for this project format:
- **src** : Put all source code for production within structured directory
- **tests** : Put all source code for testing in an easy to find location
- **configs** : Enable modification of all preset variables within single directory (consisting of one or many config files for separate tasks)
- **data** : Include example a small amount of data in the Github repository so tests can be run to validate installation
- **build**: Include scripts that automate building of a standalone environment


## Requisites
- List all packages and software needed to build the environment
- This could include cloud command line tools (i.e. gsutil), package managers (i.e. conda), etc.
```
- A
- B
- C
```

## Build Environment
- Include instructions and/or run scripts in the build subfolder
- For how to build a standalone environment to run the code in the repository
- This can be for a local environment, or a cloud environment using CLI tools from a cloud provider (i.e. gsutil from Google Cloud Platform)
- If using build scripts, these can be either shell scripts or python setup.py files
```
# Step 1
# Step 2
```

## Configs
- We recommond using either .yaml or .txt for your config files, not .json
- **DO NOT STORE CREDENTIALS IN THE CONFIG DIRECTORY!!**
- If credentials are needed, use environment variables or HashiCorp's [Vault](https://www.vaultproject.io/)


## Test
- Include instructions for how to run all tests after the software is installed
```
# Step 1
# Step 2
```
_Verify results match_
```
# Example test results
```

## Run Inference
- Include instructions on how to run inference
- i.e. image classification on a single image for a CNN deep learning project
```
# Step 1
# Step 2
```

## Build Model
- Include instructions of how to build the model
- This can be done either locally or on the cloud
```
# Step 1
# Step 2
```

## Serve Model
- Include instructions of how to set up a REST or RPC endpoint 
- This is for running remote inference via a custom model
```
# Step 1
# Step 2
```

## Analysis
- Include some form of EDA (exploratory data analysis)
- And/or include benchmarking of the model and results
```
# Step 1
# Step 2
```
