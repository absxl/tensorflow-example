# tensorflow-example
basic tensorflow examples of doing binary classification
will show auc result for each epoch
It can deal with both dense or sparse input(like 3:2.5 1234:6.7)

#binary classification of dense input data using logistic regression 
python ./binary_classification.py  --train ./data/feature.normed.rand.12000.0_2.txt --test ./data/feature.normed.rand.12000.1_2.txt 
python ./binary_classification.py  --train ./data/feature.normed.rand.12000.0_2.txt --test ./data/feature.normed.rand.12000.1_2.txt  --method mlp

#binary classification of sparse input data using logistic regression 
python ./binary_classification.py  --train ./data/feature.trate.0_2.normed.txt --test ./data/feature.trate.1_2.normed.txt  
python ./binary_classification.py  --train ./data/feature.trate.0_2.normed.txt --test ./data/feature.trate.1_2.normed.txt --method mlp

python ./binary_classification.py --tr corpus/feature.trate.0_2.normed.txt --te corpus/feature.trate.1_2.normed.txt --batch_size 200 --method mlp --num_epochs 1000

... loading dataset: corpus/feature.trate.0_2.normed.txt

0

10000

20000

30000

40000

50000

60000

70000

finish loading train set corpus/feature.trate.0_2.normed.txt

... loading dataset: corpus/feature.trate.1_2.normed.txt

0

10000

finish loading test set corpus/feature.trate.1_2.normed.txt

num_features: 4762348

trainSet size: 70968

testSet size: 17742

batch_size: 200 learning_rate: 0.001 num_epochs: 1000

I tensorflow/core/common_runtime/local_device.cc:25] Local device intra op parallelism threads: 24

I tensorflow/core/common_runtime/local_session.cc:45] Local session inter op parallelism threads: 24

I tensorflow/core/common_runtime/local_device.cc:25] Local device intra op parallelism threads: 24

I tensorflow/core/common_runtime/local_session.cc:45] Local session inter op parallelism threads: 24

0 auc: 0.503701159392 cost: 0.69074464019

1 auc: 0.574863035489 cost: 0.600787888115

2 auc: 0.615858601208 cost: 0.60036152958

3 auc: 0.641573172518 cost: 0.599917832685

4 auc: 0.657326531323 cost: 0.599433459447

5 auc: 0.666575623414 cost: 0.598856064529

6 auc: 0.671990014639 cost: 0.598072590816

7 auc: 0.675956442936 cost: 0.596850153855

8 auc: 0.681129512174 cost: 0.594744671454

9 auc: 0.689568680575 cost: 0.591011970184

10 auc: 0.70265083004 cost: 0.584730529957

11 auc: 0.720751242654 cost: 0.575319047846

12 auc: 0.740525668112 cost: 0.563041782476

13 auc: 0.756397606412 cost: 0.548790696159

14 auc: 0.76745782664 cost: 0.533633556673

15 auc: 0.776115284883 cost: 0.518648754985

16 auc: 0.783683301767 cost: 0.504702218341

17 auc: 0.79058754946 cost: 0.492255532423

18 auc: 0.796831772334 cost: 0.481419827863

19 auc: 0.802349672543 cost: 0.472143309749

20 auc: 0.807102186144 cost: 0.464346827091

21 auc: 0.811092646634 cost: 0.457953127862

22 auc: 0.814318813594 cost: 0.452874061637

23 auc: 0.816884839449 cost: 0.449003176388

24 auc: 0.818881302313 cost: 0.446225956373
