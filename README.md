# tensorFlow-install-win10

conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0  
conda create --name tf python=3.9  
conda deactivate  
conda activate tf  
conda install -c conda-forge cudatoolkit=11.2 cudnn=8.1.0  
pip install --upgrade pip  
#Anything above 2.10 is not supported on the GPU on Windows Native  
pip install "tensorflow<2.11"   
python -c "import tensorflow as tf; print(tf.config.list_physical_devices('GPU'))"  
