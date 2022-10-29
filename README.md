# Semantic-segmentation
# Project Memebers: Anosh Abraham & Syed Alam

# install nni
! pip install nni # install nni

# Save file under download (ngrok)
! wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-amd64.zip

# unzip it
! unzip ngrok-stable-linux-amd64.zip

# make new directory
! mkdir -p nni_repo

# clone repo
! git clone https://github.com/microsoft/nni.git nni_repo/nni # clone NNI's offical repo to get examples

# Create an account https://dashboard.ngrok.com/get-started/setup
# Find ngrok authtoken 
! ./ngrok authtoken 2GjVnxjnDv5z3VXi5gMnrdVrbt1_2QJn9uCqErV2GtjMzb51v

! ./ngrok authtoken 2GmXbo1RU70RG8uDduyxjPyubu7_2wXQjd73hQierhViGJZXN

# create a new experiment with the default port: 5000, using the configuration specified in config file
! nnictl create --config nni_repo/nni/examples/trials/mnist-pytorch/config.yml --port 5000 & get_ipython().system_raw('./ngrok http 5000 &')

# Output the data from server in silent mode
! curl -s http://localhost:4040/api/tunnels 

# Make new directory satSegFiles
# Change directory into satSegFiles & download data from github '228_semantic_segmentation_of_aerial_imagery_using_unet'
!mkdir satSegFiles

!cd /content/satSegFiles && wget https://raw.githubusercontent.com/bnsreenu/python_for_microscopists/master/228_semantic_segmentation_of_aerial_imagery_using_unet/228_training_aerial_imagery.py

!cd /content/satSegFiles && wget https://raw.githubusercontent.com/bnsreenu/python_for_microscopists/master/228_semantic_segmentation_of_aerial_imagery_using_unet/simple_multi_unet_model.py


![image](https://user-images.githubusercontent.com/91106087/198853736-7556698b-92fb-40cf-9936-d412156c8839.png)
