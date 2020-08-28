# Motivation

I came across an interesting dataset while browsing through the UCI Machine Learning Datasets. It was recently released to the public on 2020-06-17, and hence was less studied by individuals. What could be more interesting than an adventure into the unknown?

# Bitcoin Heist Classification Project

End-to-end classification project, involving EDA, data cleaning, feature selection, and selection, evaluation, and deployment of classification algorithms. Achieved a score of 0.81 using the Random Forest Classifier algorithm, with:

Recall Score: 0.69
Precision Score: 0.76
F1 Score: 0.72
Accuracy Score: 0.74

Continuously searching for new features and trying new algorithms and parameters for an improved score. 

Dataset from the UCI BitcoinHeistRansomwareAddressDataset Data Set available at http://archive.ics.uci.edu/ml/datasets/BitcoinHeistRansomwareAddressDataset

Number of instances: 2916697
Number of attributes: 10

# Attribute Information

address: String. Bitcoin address.

year: Integer. Year.

day: Integer. Day of the year. 1 is the first day, 365 is the last day.
length: Integer.Length is designed to quantify mixing rounds on Bitcoin, where transactions receive and distribute similar amounts of coins in multiple rounds with newly created addresses to hide the coin origin.

weight: Float. Weight quantifies the merge behavior (i.e., the transaction has more input addresses than output addresses), where coins in multiple addresses are each passed through a succession of merging transactions and accumulated in a final address.

count: Integer. Similar to weight, the count feature is designed to quantify the merging pattern. However, the count feature represents information on the number of transactions, whereas the weight feature represents information on the amount (what percent of these transactions is output) of transactions.

looped: Integer. Loop is intended to count how many transaction i) split their coins; ii) move these coins in the network by using different paths and finally, and iii) merge them in a single address. 

neighbors: Integer. (Not explained in dataset, but assumed to be number of network neighbors involved in the transaction) 

income: Integer. Satoshi amount (1 bitcoin = 100 million satoshis).

label: Category String. Name of the ransomware family (e.g., Cryptxxx, cryptolocker etc) or white (i.e., not known to be ransomware).

# Migrated csv file using:
 git lfs migrate import --include="*.csv"

