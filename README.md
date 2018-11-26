# Assignment4.4
#Use the package RcmdrPlugin.IPSUR. data(RcmdrTestDrive) and perform the below operations: #a. Calculate the average salary by gender and smoking status. #b. Which gender has the highest mean salary? #c. Report the highest mean salary. #d. Compare the spreads for the genders by calculating the standard deviation of salary by gender.

x <- tapply (salary, list(gender = gender), mean) by(salary, gender, mean, na.rm = true) Ans 1 b -> Male colMax(dat) Ans 1 c -> mean(salary[gender == male]) x[which(x == max(x))] Ans 4 d -> x <- tapply (salary, list(gender = gender), sd) by(salary, gender, sd, na.rm = true)
