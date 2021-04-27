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
> first example
> ```
    $ python train.py --arch waterdsnetf --data_dir /opt/data/private/210421_GA_compare/ --test_data_dir /opt/data/private/210421_GA_compare/ --kind GA_CMP --test_num 1000
> ```
> second example
