## Convolutional neural networks on various datasets(images,audio) 



### grozi-120([link](http://grozi.calit2.net/grozi.html)) with Alexnet([link](https://proceedings.neurips.cc/paper_files/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf))

I used in-vitro as a train-set and in-situ as a test set,the hyper-parameters are bit different then alexnet i used dropout rate(0.7 instead of 0.5),batch-size(64 instead of 128),learning-rate(0.0001 instead of 0.001).

Created a csv file with labels for easier loading of the images,and used torchvision.transforms for data augmentation on in-vitro,for in-situ i limited the number of images per class label to be 5 since i was getting cuda out of memory if i load the entire in-situ.














