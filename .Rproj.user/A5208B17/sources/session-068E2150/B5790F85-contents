

# assegnare il dataset all'oggetto data
data = pressure
# rinominare la variabaile dipendente in y
data$y = pressure$temperature
# rinominare la variabile indipedente in x
data$x = pressure$pressure
# maggiori dettagli sulla x
summary(data$x)

# grafico 
plot(data$y ~ data$x)

# regressione
m = lm(y ~ x, data = data)
# summary del modello
summary(m)