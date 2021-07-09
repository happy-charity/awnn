# awnn
Implementing neural networks on maix-ii dock based on Allwinner v831 SoC. (not completed yet)


To run neural network on Allwinner, whether it's written on tensorflow, pytorch, keras or any other framework, neural network needs conversion to awnn format, e.g. pytorch -> onnx -> ncnn -> awnn. Here, conversion of pytorch -> awnn is explaned. 

When conversion completed, you get param and bin files. This is similar to weights and config files in yolo. Bin file is not readable, because it is binary file as obvious, but from param file you can get information about the neural networks' layers. This link shows explains structure of param file https://github.com/Tencent/ncnn/wiki/param-and-model-file-structure. But reading this structure from param file is tough. So, you can upload param file to https://netron.app/ and get graphical representation of neural network layers. From the graph, you can find output layer for further usage.



image annotations and labeling tools --->>  https://datascience.stackexchange.com/questions/14039/tool-to-label-images-for-classification
                                            https://www.cloudfactory.com/image-annotation-guide
