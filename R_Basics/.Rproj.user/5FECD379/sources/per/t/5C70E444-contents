# Orgense the project folder
# data
# scripts
# results

# create folder
dir.create("data")
dir.create("scripts")
dir.create("results")

# working of R -> function(your argument/input)
print("Biotechnology")

gene_expression <- c(2.3, 4.3, 3.8, 5.2, 6.2)
# <- is the assignment operator to store values into variable

mean_result = mean(gene_expression)

# Basic Visualisation
plot(gene_expression)
hist(gene_expression)
barplot(gene_expression)

# Check the bascis stats
summary(gene_expression)

# R Datatypes
# 1. Numberic with decimal point +ve or -ve
x <- 24
class(x)

y <- 10.4
class(y)

# 2. Integer/whole number
# by default decimal and whole is classified as numeric
z = 23L
class(z)
# INteger consunes less storage than numeric data

var_1 = c(24.8, 23.6, 25.8, 22.4)
class(var_1)

# convert intger to numeric
var_2 = as.integer(var_1)
class(var_2)

# convert integer to numeric
var_3 = as.numeric(var_2)
class(var_3)

# Character/str
var_4 = c("gene1", "gene2", "gene3")
class(var_4)

var_5 = c(gene1, "gene2", "gene3")

var_6 = c("3.8", "4.4")
class(var_6)
mean(var_6)

var_7 = c(3.8, 4.4)
class(var_7)
mean(var_7)

# 4. factor ot categorical data
# either written as numeric(0, 1) or chraacter (normal, cancer)
disease_status = c("cancer", "normal", "cancer", "cancer", "normal")
class(disease_status)

# convert class into factor
disease_status = as.factor(disease_status)
class(disease_status)
disease_status

disease_status <- factor(disease_status,
                         levels = c("normal", "cancer"))
disease_status

# 5. logical datatype
age = c(23, 44, 25)

var_8 = age < 25

# import csv file
data <- read.csv(file.choose())


# Convert height into factor
data$height_fac <- as.factor(data$height)
str(data)

# Relevel factors
data$height_fac = factor(data$height,
                         levels = c("Tall", "Medium", "Short"))
str(data)
levels(data$height_fac)

# Convert gender into factor
data$gender_fac = as.factor(data$gender)
str(data)

# Convert gender factor to numeric factor
data$gender_num = ifelse(data$gender_fac == "Female", 1, 0)
str(data)

data$gender_num = as.factor(data$gender_num)
str(data)

# Save file as a csv file
write.csv(disease_status, file = "results/patient_data.csv")

# Saving the workspace
# saving the entire workspace
save.image(file = "full_workspace.RData")

# save specifiic specfiic objects
save(gene_expression, disease_status, file = "workspace.RData")

# Load workspace in R
load("workspace.RData")
load("full_workspace.Rdata")
