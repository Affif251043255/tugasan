# R code for Individuals Control Chart (PartLength)
library(tidyverse)
library(qcc)
library(plotly)
library(htmlwidgets)

machine1_data <- X002..2. %>% filter(Machine == 1, Temperature == 303, Pressure == 100)
i_chart_partlength <- qcc(machine1_data$PartLength, type="xbar.one", nsigmas = 3, plot = FALSE)

plot_data <- data.frame(
  sample = 1:length(i_chart_partlength$statistics),
  val = i_chart_partlength$statistics,
  UCL = i_chart_partlength$limits[1,2],
  LCL = i_chart_partlength$limits[1,1],
  CL = i_chart_partlength$center
)

p <- plot_ly(plot_data, x = ~sample, y = ~val, type = 'scatter', mode = 'lines+markers')
htmlwidgets::saveWidget(as_widget(p), file = "media/plots/partlength_xbar_m1_t303_p100.html", selfcontained = TRUE)
