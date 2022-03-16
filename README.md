# median
print("Enter values in a vector")
x<-scan()
n <- length(x)
for(i in 1:(n-1))
for(j in (i+1):n)
        if (x[i] > x[j])
        {
        temp <- x[i]
        x[i] <- x[j]
        x[j] <- temp
      }
  print(x)
  if(n%%2==0){
    med =(x[n%/%2]+x[(n%/%2)+1])/2.0
    } else 
    med =x[(n+1)%/%2]
  print(med)

