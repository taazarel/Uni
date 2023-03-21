#kapitel 
# §8.1 Hypothesis testing
## 8.1.1 Hypothesis
A statement about the world that can be rejected or accepted. Gives a true or false answer.
## 8.1.2 Type I, and Type II errors
A type I error is... :: When a true hypothesis is rejected. <!--SR:!2023-05-14,54,290-->
A type II error is... :: When a false hypothesis is accepted. <!--SR:!2023-05-13,53,290-->
## 8.1.3 Significance
Significance is... :: The possibility of getting a type I error. <!--SR:!2023-04-12,22,270-->
To find the significance of a hypothesis we... :: make a cutoff point of acceptance on our model, and integrate the area outside the cut-off point. This number is denoted $\alpha$ and describes the significance. <!--SR:!2023-05-15,55,290-->

## 8.1.4 Power
Power is defined as... :: $1-\beta$. And we wish for this number to be large.  <!--SR:!2023-05-12,52,290-->
In power $\beta$ is... :: the integral of the probability distribution for getting a type II error. Ergo the integral of everything outside the "reject region".[^1] <!--SR:!2023-05-11,51,290-->

# §8.2 Interpreting Expiriments
## §8.2.1 The null hypothesis
If you wish to prove something by hypothesis you must... :: make a hypothesis that states there is no connection, then disprove it. This is denoted by $H_0$ and is called a null hypothesis. <!--SR:!2023-05-16,56,290-->

# §8.3 Goodness of Fit


[^1]: Notice that $\alpha$ and $\beta$ are entwined. We wish for both power to be large and significance to be small, but cannot have both. Therefore we must adjust as deemed necessary.