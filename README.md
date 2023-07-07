# system-setup
# Remote server 
Steps to have access to jupyterlab on a remote server :
1. ssh and cast the localhost of the serevre on localhost of your machine
 ssh -L 8080:localhost:8080 serever_ip
2. On the base environment install conda-nb
 conda install -c conda-forge nb_conda_kernels
3. on the environment install ipykernel
 conda install ipykernel
Note : If you have installed nb_conda_kernels, and want to create a new conda environment and have it accessible right away then
4. conda create -n new_env_name ipykernel





%load_ext autoreload
%autoreload 2
