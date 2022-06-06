# CrossSim Models
This repository contains pre-trained Keras model files for [CrossSim](https://github.com/sandialabs/cross-sim). This is not a self-executing repository. Please see the main [CrossSim repository](https://github.com/sandialabs/cross-sim) for more information about the tool.

The following pre-trained models are available in this repository for use with CrossSim Inference:
* MNIST:
	* Two shallow CNNs with different numbers of channels, trained by CrossSim's developers
* CIFAR-10: all models were trained by CrossSim's developers
    * Four ResNets of different depths, following the topology specified in the [original ResNet paper](https://arxiv.org/abs/1512.03385): ResNet14, ResNet20, ResNet32, ResNet56
    * A shallow CNN that uses bounded ReLU (cifar10_cnn_brelu)
    * A sequential CNN with binary weights and activations using the [Larq package](https://docs.larq.dev/larq/)
    * A sequential CNN with binary activations using the [Whetstone package](https://github.com/SNL-NERL/Whetstone)
* CIFAR-100:
	* A ResNet56 network, trained by CrossSim's developers
* ImageNet: all models were obtained from external sources
	* ResNet50, InceptionV3, MobileNetV1, and MobileNetV2 from [keras.applications](https://keras.io/api/applications/)
	* ResNet50v1.5 and MobileNetV1 quantized (int8) from the benchmark suite in [MLPerf Inference](https://github.com/mlcommons/inference/tree/master/vision/classification_and_detection)
	* ResNet50v1.5 quantized (int4) submitted by [Nvidia for MLPerf Inference](https://github.com/mlperf/inference_results_v0.5/tree/master/open/NVIDIA)