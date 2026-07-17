# R Code for Machine 1 PartLength
library(qcc)
m_data <- X002_data %>% filter(Machine == 1, Temperature == 303, Pressure == 100)
qcc(m_data$PartLength, type='xbar.one', nsigmas=3)
