# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Generalized Kernel Regularized Least Squares Use gKRLS With (In) R Software
install.packages("gKRLS")
library("gKRLS")
gKRLS = read.csv("https://raw.githubusercontent.com/timbulwidodostp/gKRLS/main/gKRLS/gKRLS.csv",sep = ";")
# Estimation Generalized Kernel Regularized Least Squares Use gKRLS With (In) R Software
# A gKRLS model without fixed effects
fit_gKRLS <- mgcv::gam(y ~ s(x1, x2, x3, bs = "gKRLS"), data = gKRLS)
summary(fit_gKRLS)
# A gKRLS model with fixed effects outside of the kernel
fit_gKRLS_FE <- mgcv::gam(y ~ state + s(x1, x2, x3, bs = "gKRLS"), data = gKRLS)
summary(fit_gKRLS_FE)
# Generalized Kernel Regularized Least Squares Use gKRLS With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished