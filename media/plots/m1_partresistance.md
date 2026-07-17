# R Code for Machine 1 PartResistance
library(qcc)
m_data <- X002_data %>% filter(Machine == 1, Temperature == 303, Pressure == 100)
qcc(m_data$PartResistance, type='xbar.one', nsigmas=3)
