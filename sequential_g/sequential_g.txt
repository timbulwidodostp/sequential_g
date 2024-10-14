# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Perform linear exact sequential analysis for poisson andb binomial data g-estimation to estimate
# the controlled direct effect of a treatment net the effect of a mediator Use sequential_g With R Software
install.packages("DirectEffects")
library("DirectEffects")
sequential_g = read.csv("https://raw.githubusercontent.com/timbulwidodostp/sequential_g/main/sequential_g/sequential_g.csv",sep = ";")
# Estimation Perform linear exact sequential analysis for poisson andb binomial data g-estimation to estimate
# the controlled direct effect of a treatment net the effect of a mediator Use sequential_g With R Software
result_sequential_g<- women_politics ~ plow + agricultural_suitability + tropical_climate + large_animals + 
political_hierarchies + economic_complexity + rugged | years_civil_conflict + years_interstate_conflict  + 
oil_pc + european_descent + communist_dummy + polity2_2000 + serv_va_gdp2000 | centered_ln_inc + centered_ln_incsq
sequential_g <- sequential_g(result_sequential_g, sequential_g)
summary(sequential_g)
# Perform linear exact sequential analysis for poisson andb binomial data g-estimation to estimate
# the controlled direct effect of a treatment net the effect of a mediator Use sequential_g With R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished