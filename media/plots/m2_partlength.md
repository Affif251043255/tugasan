# R Code for Machine 2 PartLength
library(qcc)
m_data <- X002_data %>% filter(Machine == 2, Temperature == 338, Pressure == 200)
qcc(m_data$PartLength, type='xbar.one', nsigmas=3)
