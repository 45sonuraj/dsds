2. consider a showroom of elecronic products, where there are various salesmen. Each salesman is given a commissoion of 5% , depending on the sales made per month. In case the salw done is less than 50000,then the salesman is not given any commission. Write a function to claculate toatal sales of a salesman in a month, commisssion. and remarks for the salesman. Sales done by each salesman per week is to ve provided as input. Use tuples / list to store data of slaesmen.
Assigh remarks accordigng to the following criteria:
Excellent : Sales >=80000
Good: Sales>=60000 and <80000
Average: Sales<=40000 and <60000
Work Hard: Sales < 40000


def mister(tup):
    commison=0
    sum=tup[1]+tup[2]+tup[3]+tup[3]
    if(sum>=50000):
        commison=sum*0.05
    if(sum>=80000):review="Excellent"
    elif(sum<80000 and sum >=60000):review="Good"
    elif(sum<60000 and sum>=40000):review="Average"
    else: review="Work Hard"
    lst=[commison, review]
    return lst

data=[]
print("Enter the weekly data of salesman continuely :")
for x in range (0,4):
    week=int(input())
    data.append(week)

print(" Commison : ", mister(data)[0])
print("Review : ", mister(data)[1])
    
    
