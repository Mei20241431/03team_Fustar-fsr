# 03_Incremental Learning-Face Restoration Model   
## 🔧 Dependencies and Installation
Python = 3.8 (Recommend to use Anaconda or Miniconda)  
PyTorch = 2.0  
Option: NVIDIA GPU + CUDA  
Option: Linux  
## Installation
git clone https://github.com/Mei20241431/Mei20241431

### step1: Image_Preprocessing 
#install python dependencies  
cd Image_Preprocessing  
conda install mpi4py  
pip3 install -r requirements.txt 

### step2: Image Post-processing
#install python dependencies  
cd Image Post-processing  
pip install basicsr  
pip install facexlib  
pip install -r requirements.txt  
python setup.py develop  

### step3: Image_Enhancement
#install python dependencies
cd Image_Enhancement   
pip install -r requirements.txt   
python setup.py develop

## test

### step1: Image_Preprocessing
#### Enter Directory
cd Image_Preprocessing 
#### Download the pretrained model
Download the pretrained face diffusion model from [Google Drive](https://drive.google.com/file/d/1JMYAYoAQdOWvjwAdqq3fpQkpE7Z55mkT/view?usp=drive_link) to the models/restorer folder. 
#### Commands
python test_step1.py 

### step2: Image Post-processing




### step3: Image_Enhancement  
cd Image_Enhancement 
CUDA_VISIBLE_DEVICES=0 \
python ./test_step3.py --input /path/to/your/test \
--output ./results/enhanceHR --model_path ./experiments/ELAN.pth --tile_size 1200




<!--
**Mei20241431/Mei20241431** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
