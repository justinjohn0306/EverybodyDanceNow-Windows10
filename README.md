# EverybodyDanceNow-Windows10

This repo is an implementation EverybodyDanceNow repo by Caroline Chan : https://github.com/carolineec/EverybodyDanceNow




Installation:


conda create -n dancenow python=3.7

conda activate dancenow


pip install torch==1.7.1+cu101 torchvision==0.8.2+cu101 torchaudio===0.7.2 -f https://download.pytorch.org/whl/torch_stable.html


pip install --user --upgrade tensorflow


pip install dominate


pip install scipy


Training Test CMD line:

python train_fullts.py --name ./model_local/ --dataroot ./dataset/train/  --checkpoints_dir ./checkpoints/ --loadSize 512 --no_instance --no_flip --tf_log --netG local --ngf 32 --num_D 3 --label_nc 6 --resize_or_crop none --save_latest_freq 100 --save_epoch_freq 1 --print_freq 10   
