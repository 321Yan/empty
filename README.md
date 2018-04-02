# project
r-scrpit under home /yan123

### upload folder to vm from local google cloud SDK
gcloud compute scp --recurse "D:/sfu/kaggle/dog/" rstudio:\
(caution: be aware of different usernames for a single vm)

### upload a single file
gcloud compute scp "D:/sfu/kaggle/dog/labels.csv" rstudio:\
upper right coner of SSH (slower)

### download file form VM
gcloud compute scp [INSTANCE_NAME]:[REMOTE_FILE_PATH] [LOCAL_FILE_PATH]

### save a model
save_model_hdf5(model, 'my_model.h5') \
model <- load_model_hdf5('my_model.h5')
