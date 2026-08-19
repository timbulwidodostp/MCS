# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Perform the Model Confidence Set procedure of Hansen et.al. (2011) Use MCS With (In) R Software
install.packages("MCS")
library("MCS")
# Estimation Perform the Model Confidence Set procedure of Hansen et.al. (2011) Use MCS With (In) R Software
MCS_ = read.csv("https://raw.githubusercontent.com/timbulwidodostp/MCS/main/MCS/MCS.csv",sep = ";")
MCS_Data <-  na.omit(MCS_)
MCS_Data <-  MCS_Data [complete.cases(MCS_Data), ]
MCS <- as.matrix(MCS_Data)
storage.mode(MCS) <- "numeric"
MCS = MCSprocedure(Loss = MCS, verbose = TRUE)
MCS
# Perform the Model Confidence Set procedure of Hansen et.al. (2011) Use MCS With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished