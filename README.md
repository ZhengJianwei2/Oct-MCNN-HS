# Oct-MCNN-HS
## Papers
* MCNN-CP: Hyperspectral Image Classification Using Mixed Convolutions and Covariance Pooling (TGARS 2021) [paper](https://ieeexplore.ieee.org/document/9103280/) and [source_code](https://github.com/ZhengJianwei2/MCNN-based_HSI_Classification/blob/master/MCNN-CP-Source-code.ipynb)
* [Oct-MCNN-HS](https://github.com/ZhengJianwei2/MCNN-based_HSI_Classification): 3D Octave and 2D Vanilla Mixed Convolutional Neural Network for Hyperspectral Image Classification With Limited Samples (Submitted)

## 1. Environment setup
This code has been tested on on a personal laptop with Intel i7-9750H 2.6-GHz processor, 32-GB RAM, and an NVIDIA GTX1650 graphic card, Python 3.6, tensorflow_gpu-1.14.0, Keras-2.2.4, CUDA 10.0, cuDNN 7.6. Please install related libraries before running this code:

    pip install -r requirements.txt

## 2. Download the datesets:
* IP:
[Indian Pines corrected](http://www.ehu.eus/ccwintco/uploads/6/67/Indian_pines_corrected.mat) and
    [Indian Pines gt](http://www.ehu.eus/ccwintco/uploads/c/c4/Indian_pines_gt.mat)
* UH:
[University of Houston 2018](https://hyperspectral.ee.uh.edu/?page_id=1075)
* UP:
[University of Pavia corrected](http://www.ehu.eus/ccwintco/uploads/e/ee/PaviaU.mat) and
    [University of Pavia gt](http://www.ehu.eus/ccwintco/uploads/5/50/PaviaU_gt.mat)
* SA:
[Salinas Scene corrected](http://www.ehu.eus/ccwintco/uploads/a/a3/Salinas_corrected.mat) and
    [Salinas Scene gt](http://www.ehu.eus/ccwintco/uploads/f/fa/Salinas_gt.mat)

and put them into data directory.

## 3. Download the models (loading models):

* [models]() code: 

and put them into models directory.

## 4. Download the pretrained_models (loading model parameters):
* IP:
[Indian Pines]() code: 
* UH:
[University of Houston]() code: 
* UP:
[University of Pavia]() code: 
* SA:
[Salinas Scene]() code: 

and put them into pretrained_models directory.

## 5. Test

    python validate.py                
	--dataset IP                       # dataset_name
	--model Oct-MCNN-HS                # model_name
	--ratio 0.99                       # test_ratio
           
The testing result will be saved in the classification_report.txt.

## 6. Cite
