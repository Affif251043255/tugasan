# R Code for Machine 3 PartResistance
library(qcc)
m_data <- X002_data %>% filter(Machine == 3, Temperature == 373, Pressure == 300)
qcc(m_data$PartResistance, type='xbar.one', nsigmas=3)
