# Assignment_4.2

#Write a program to create barplots for all the categorical columns in mtcars.

barplot(mtcars$mpg)
barplot(mtcars$cyl) 
barplot(mtcars$disp) 
barplot(mtcars$hp) 
barplot(mtcars$drat) 
barplot(mtcars$wt) 
barplot(mtcars$qsec) 
barplot(mtcars$vs) 
barplot(mtcars$am) 
barplot(mtcars$gear) 
barplot(mtcars$carb)

#Create a scatterplot matrix by gear types in mtcars dataset.

library(lattice) splom(mtcars[c(1,3,5,6)], groups=gear, data=mtcars, panel=panel.superpose, key=list(title="Gear Types", columns=3, points=list(pch=super.sym$pch[1:3], col=super.sym$col[1:3]), text=list(c("1 Gear","2 Gear","3 Cylinder"))))

#Write a program to create a plot density by class variable.

Ans:
plot(density(mtcars$mpg))  
plot(density(mtcars$cyl))
plot(density(mtcars$disp))
plot(density(mtcars$hp))
plot(density(mtcars$drat))
plot(density(mtcars$qsec))
plot(density(mtcars$vs))
plot(density(mtcars$am))
plot(density(mtcars$gear))
plot(density(mtcars$carb))
