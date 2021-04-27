# TFR-FLDenseNet
The fully-linear DenseNet to extract pipe leak features in transient frequency response.

It learns from training data set and validates on the testing data set.

## Some cmd arguments
* --arch: the kind of network architecture to use (should be "waterdsnetf" here)
* --data_dir: the path of the training data set
* --test_data_dir: the path of the testing data set
* --test_num: scale of the testing data set
* --epoch: training epoch number
* --kind: the name of the log file recording information during running

## How to run
* Firstly you need to install all the dependencies.
* Then run in a Python console, following are some examples:
> ### First example
> ```
> $ python train.py --arch waterdsnetf --data_dir /opt/data/private/191220_LeakScale_M1/ --test_data_dir /opt/data/private/191220_LeakScale_M1/ --kind 191220_LeakScale_M1
> ```
> ### Second example (cross dataset validation)
> ```
> $ python train.py --arch waterdsnetf --data_dir /opt/data/private/200115_LeakScale_M4/ --test_data_dir /opt/data/private/200115_LeakScale_M5/ --kind _TestWith_200115_LeakScale_M2
> ```
> ### Third example (specify testing data set scale)
> ```
> $ python train.py --arch waterdsnetf --data_dir /opt/data/private/210421_GA_compare/ --test_data_dir /opt/data/private/210421_GA_compare/ --kind _GA_CMP --test_num 1000
> ```
