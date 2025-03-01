# mean-avg
import csv
from statistics import mean
with open("new 1.csv") as fcsv:
    reader = csv.reader(fcsv)
    for row in reader:
        #print(row)
        name = row[0]
        thisgrade = list()
        for grade in row[1:]:
            thisgrade.append(int(grade)) 
        print("average of %s is %f" % (name,mean(thisgrade)))
