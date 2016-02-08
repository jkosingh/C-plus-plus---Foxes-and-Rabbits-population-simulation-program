# C++-Foxes-and-Rabbits-population-simulation-program

Populations of predators and their prey that are isolated tend to achieve an equilibrium over time. The pattern tends to be a cyclic increase and decrease in the populations. When the number of predators is low, the number of prey grow. As the prey increase the predators manage to catch more of them. The predators are now healthier and can raise their young with fewer dying out, so the number of predators increases. Now since there are more predators, they will start to reduce the number of prey. When the number of prey decreases too far, the predators won't be able to catch enough of them and the predators will start to die of starvation. That's the cycle. 


    For Rabbit Populations :
    If no foxes are present the new rabbit population is calculated from the previous population by the following equation:

    PRn = PR(n-1) + BR * PR(n-1)

    where :
        PRn is the new rabbit population after time period n
        PR(n-1) is the beginning rabbit population at the time period n-1
        BR is the birth rate for rabbits 
    Under these conditions the rabbit population would continually increase.

    For Fox Populations :
    If no hunters are present the new fox population is calculated from the previous population by the following equation:

    PFn = PF(n-1) - DF * PF(n-1)

    where:
        PFn is the new fox population after time period n
        PF(n-1) is the beginning fox population at the time period n-1
        DF is the death rate for foxes 
    Under these conditions the fox population will decrease.

    For Both Foxes and Rabbits Coexisting :
    When foxes can eat rabbits the population equations have another term to describe the interaction between the two.
    The population of rabbits is the same as above with a loss of population due to foxes :

    PRn = PR(n-1) + BR * PR(n-1) - I * PR(n-1) * PF(n-1)

    where :
        I is the interaction constant between the foxes and the rabbits. The population of foxes is increased with the addition of the interaction term :

    PFn = PF(n-1) - DF * PF(n-1) + I * PF(n-1) * PR(n-1)
    Now the population of rabbits is decreased by the foxes with the greater number of foxes causing a greater decrease in the rabbit population. This means that the rabbit population is eventually going to decrease and the resulting fox population will also decease. As a result a cyclic increase and decrease in the populations are set up. This is what is observed in the simulation. 
