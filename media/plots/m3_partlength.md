# R Code for Machine 3 PartLength
library(qcc)
m_data <- X002_data %>% filter(Machine == 3, Temperature == 373, Pressure == 300)
qcc(m_data$PartLength, type='xbar.one', nsigmas=3)
