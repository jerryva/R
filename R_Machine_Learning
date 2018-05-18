
library(caTools)

data("mtcars")

split<-sample.split(mtcars,SplitRatio = 0.7)

Training<-subset(mtcars,split==TRUE)

Testing<-subset(mtcars,split=FALSE)

model<-glm(vs ~ wt+disp,Training,family = "binomial")     #here we take (vs engine) against wt+displacemnet

summary(model)

data<-data.frame(wt=2.200,disp=78.7)                       #for fiat 128

data<-data.frame(wt=3.170,disp=351.0)                      #for ford pantera

probability<-predict(model,data,type="response")

probility                                                       #will give the probabilty for the 'vs engine'


