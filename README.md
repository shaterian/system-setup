# system-setup
# Remote server 
Steps to have access to jupyterlab on a remote server :
1. ssh and cast the localhost of the serevre on localhost of your machine  
  ssh -L 8080:localhost:8080 serever_ip
2. On the base environment install conda-nb  
 conda install -c conda-forge nb_conda_kernels
3. Install jupyterlab on the environment    
conda install -c conda-forge jupyterlab
4. install ipykernel on the environment   
 conda install ipykernel  
Note : If you have installed nb_conda_kernels, and want to create a new conda environment and have it accessible   right away then:    
conda create -n new_env_name ipykernel  
5. To open upyterlab  
jupyter-lab --no-browser --port 8080     
6. To have updated modules automatically be loaded in a jupyter-notebook add the following command at the start of your notebook    
 %load_ext autoreload  
%autoreload 2  


$ conda activate cenv           # . ./cenv/bin/activate in case of virtualenv
(cenv)$ conda install ipykernel
(cenv)$ ipython kernel install --user --name=<any_name_for_kernel>
(cenv)$ conda deactivate
