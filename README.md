# Phenotyping-exercise

Sample datasets: [http://spidey.ccbr.utoronto.ca/~okraus/DeepLoc_full_datasets.zip](http://spidey.ccbr.utoronto.ca/~okraus/DeepLoc_full_datasets.zip)
Use the architecture in "Automated analysis of high-content microscopy data with deep learning", [github link](https://github.com/okraus/DeepLoc)

- Yeast Chong set.ipynb: Repeat the work in "Automated analysis of high-content microscopy data with deep learning", use the same architecture.
- Multi-label .ipynb: Change to one hot encoding
- Novel class detection(peroxisome).ipynb: Use one hot encoding to detect novel class.
- GAN exercise-Deep.ipynb: A GAN exercise.

## Request GPU nodes at HPC:
'''
qsub -I -X -q gpu -l nodes=1:ppn=8:gtx980 -l mem=250gb
'''
Load modules:
'''
module load cuda
module load gcc
module load python/3.6.3
'''
I use Xming to forward X11 and run the jupyter notebook interactively.
