# CSE534-FinalProject
## Step1
Download datasets:
scripts/download_mpiigaze_dataset.sh
## Step2
Preprocess datasets:
python3 tools/preprocess_mpiigaze.py --dataset datasets/MPIIGaze -o datasets/
## Step3
Train
python3 train.py --config configs/mpiigaze/lenet_train.yaml
## Step4
Evaluate
python3 evaluate.py --config configs/mpiigaze/lenet_eval.yaml

## Note:
In the config file, there are many parameters can be changed.
If you want to train all datasets about 15 persons, use scripts/run_all_mpiigaze_lenet.sh.
