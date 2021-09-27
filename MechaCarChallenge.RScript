#Deliverable 1

#Use the library() function to load the dplyr package.
library(dplyr)

#Import and read in the MechaCar_mpg.csv file as a dataframe.
MechaCar_mpg <- read.csv(file='MechaCar_mpg.csv', check.names=F, stringsAsFactors = F)


#Perform linear regression using the lm() function.
MechaCar_lm <- lm(formula = mpg ~ vehicle_length + vehicle_weight + spoiler_angle + ground_clearance + AWD, data=MechaCar_mpg)

#Using the summary() function, determine the p-value and the r-squared value for the linear regression model.
summary(MechaCar_lm)

#Deliverable 2
#In your MechaCarChallenge.RScript, import and read in the Suspension_Coil.csv file as a table.
suspension_coil <- read.csv(file='Suspension_Coil.csv', check.names=F, stringsAsFactors = F)

(suspension_coil["Manufacturing_Lot"])
#Write an RScript that creates a total_summary dataframe using the summarize() function to get the mean, median, variance, and standard deviation of the suspension coil’s PSI column.
total_summary <- suspension_coil %>% summarize(Mean=mean(PSI), Median=median(PSI), Variance=var(PSI),SD=sd(PSI), .groups = 'keep') 
total_summary

#Write an RScript that creates a lot_summary dataframe using the group_by() and the summarize() functions to group each manufacturing lot by #the mean, median, variance, and standard deviation of the suspension coil's PSI column
lot_summary <- suspension_coil %>% group_by(Manufacturing_Lot) %>% summarize(Mean=mean(PSI),Median=median(PSI),Variance=var(PSI),SD=sd(PSI), .groups = 'keep') #create lot summary table
lot_summary

#Deliverable 3
#write an RScript using the t.test() function to determine if the PSI across all manufacturing lots is statistically different from the population mean of 1,500 pounds per square inch.#t-test for overall data set
overall = t.test(x=suspension_coil$PSI, mu=1500)
overall


# Next, write three more RScripts in your MechaCarChallenge.RScript using the t.test() function and its subset() argument to determine if the PSI for each manufacturing lot is statistically different from the population mean of 1,500 pounds per square inch.
lot1 = t.test(subset(suspension_coil, Manufacturing_Lot == "Lot1")$PSI, mu = 1500)
lot1


lot2 = t.test(subset(suspension_coil, Manufacturing_Lot == "Lot2")$PSI, mu = 1500)
lot2

lot3 = t.test(subset(suspension_coil, Manufacturing_Lot == "Lot3")$PSI, mu = 1500)
lot3
