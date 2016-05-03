# NSL-KDD-Dataset

***Note
-------
I couldn't find the NSL-KDD dataset anywhere except via the Wayback Machine. This is just a backup. The data was found via  https://web.archive.org/web/20150205070216/http://nsl.cs.unb.ca/NSL-KDD/


Abstract
--------
NSL-KDD is a data set suggested to solve some of the inherent problems of the KDD'99 data set which are mentioned in [1]. Although, this new version of the KDD data set still suffers from some of the problems discussed by McHugh [2] and may not be a perfect representative of existing real networks, because of the lack of public data sets for network-based IDSs, we believe it still can be applied as an effective benchmark data set to help researchers compare different intrusion detection methods. Furthermore, the number of records in the NSL-KDD train and test sets are reasonable. This advantage makes it affordable to run the experiments on the complete set without the need to randomly select a small portion. Consequently, evaluation results of different research work will be consistent and comparable.

Data Files
----------

**KDDTrain+.ARFF** - The full NSL-KDD train set with binary labels in ARFF format

**KDDTrain+.TXT** - The full NSL-KDD train set including attack-type labels and difficulty level in CSV format

**KDDTrain+_20Percent.ARFF** - A 20% subset of the KDDTrain+.arff file

**KDDTrain+_20Percent.TXT** - A 20% subset of the KDDTrain+.txt file

**KDDTest+.ARFF** - The full NSL-KDD test set with binary labels in ARFF format

**KDDTest+.TXT** - The full NSL-KDD test set including attack-type labels and difficulty level in CSV format

**KDDTest-21.ARFF** - A subset of the KDDTest+.arff file which does not include records with difficulty level of 21 out of 21

**KDDTest-21.TXT** - A subset of the KDDTest+.txt file which does not include records with difficulty level of 21 out of 21


Improvements to the KDD'99 data set
-----------------------------------
The NSL-KDD data set has the following advantages over the original KDD data set:
*	It does not include redundant records in the train set, so the classifiers will not be biased towards more frequent records.
* There is no duplicate records in the proposed test sets; therefore, the performance of the learners are not biased by the methods which have better detection rates on the frequent records.
* The number of selected records from each difficultylevel group is inversely proportional to the percentage of records in the original KDD data set. As a result, the classification rates of distinct machine learning methods vary in a wider range, which makes it more efficient to have an accurate evaluation of different learning techniques.
* The number of records in the train and test sets are reasonable, which makes it affordable to run the experiments on the complete set without the need to randomly select a small portion. Consequently, evaluation results of different research works will be consistent and comparable.


References
----------
[1] M. Tavallaee, E. Bagheri, W. Lu, and A. Ghorbani, “A Detailed Analysis of the KDD CUP 99 Data Set,” Submitted to Second IEEE Symposium on Computational Intelligence for Security and Defense Applications (CISDA), 2009. 

[2] J. McHugh, “Testing intrusion detection systems: a critique of the 1998 and 1999 darpa intrusion detection system evaluations as performed by lincoln laboratory,” ACM Transactions on Information and System Security, vol. 3, no. 4, pp. 262–294, 2000.
