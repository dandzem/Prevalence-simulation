# Prevalence-simulation
The program is used to simulate the spread of an infectious disease within a closed environment with a homogeneous and adjustable population




#Model Description
The multi-agent model will be developed using a software tool based on NetLogo, an open
platform for simulations. The model created for this project is a modified version of
“epiDEM” (Epidemiology: Understanding Disease Dynamics and Emergence through
Modeling), the introductory model in the curricular unit. The program is used to simulate the
spread of an infectious disease within a closed environment with a homogeneous and
adjustable population. The model is flexible and can be adjusted for different purposes.
The software model is intentionally simplified: the main goal is to optimize the graphic
interface and integrate it with the code of the basic epiDEM program, allowing user-friendly
interactions with model’s parameters and data visualization tools. For simplicity reasons, the
program does not include some advanced features of the epidemic: the “time of immunity”,
i.e. how much time an individual is immune after healing from the virus, and the possibility
to plot multiple mutations at once.
In order to simulate the vaccines’ intervention, the model’s environment is populated with the
vaccination centers: their number can be set up using a slider. For the limited aim of this
project, we assume that an external agent - Healthcare Authorities - oversees the number of
vaccination’s hubs.
The model defines a virtual context in which the virus is released, consisting of a
homogeneous group of people, where everyone has the same chance of interacting with any
other person within the area. The initial number of members of the virtual population, which
are treated in the model as active agents, is modifiable through a specific variable.
All the people within the model are susceptible to contagion.
Distinctive colors are used to specify the different conditions of an agent:
● Red is used for infected individuals.
● White is adopted for not infected nor vaccinated people.
● Green is applied to agents which have successfully recovered from the virus.
● Blue is selected for vaccinated individuals.
Agents are programmed to randomly wander around within the virtual environment. If they
cross one of the vaccination centers when they are not infected, they get vaccinated;
individuals who got vaccinated diminish their chances of getting infected. The probability of
getting vaccinated (an agent passes through a vaccination hub), along with all the other
parameters included in the model can be adjusted through sliders in the interface tab of the
model.
In addition, the model considers the possibility of viral mutations. There are parameters for
the probability of the virus to mutate, as well as for the chances to be infected with the
variant, both when vaccinated and when not vaccinated. Thanks to flexibility, the model can
be used with or without the application of mutations: all the relevant parameters can then be
adjusted using sliders.
In addition, at the bottom of the interface tabs there are graphs to help visualize the dynamics
and the total number of agents in different states.
The SETUP button creates individual according to the previously adjusted parameters. Once
the model has been set up, push the GO button to run the model. Each time-step can be
considered as expressed in hours.
The interface is divided in three main parts: the top-left section consists of all the adjustable
parameters, the top-right area is occupied by the environment simulator where the progress of
the simulation is shown, the bottom-left section displays three graphs which show some
statistics of the simulation’s dynamics.
Legend of the model’s interface:
1. INITIAL-VACCINATION CENTER (0-50): the number of vaccination centers in the
environment
2. INITIAL-PEOPLE (initialized to vary between 50-400): the number of individuals in
the simulation
3. INFECTION-CHANCE (10-100): disease’s probability of being spread form one
agent to another when they come in contact
4. CHANCE INFECTED IF VACCINATED (10-100): chance of the agent getting
infected while being vaccinated
5. VACCINATION-CHANCE (0-100): probability of the agent passing through
vaccination’s hub and getting vaccinated
6. RECOVERY-CHANCE (10-100): probability of an infected individual to recover
7. AVERAGE-RECOVERY-TIME (50-500): time it takes for an individual to recover on
average. This parameter is measured in ticks (hours)
8. MUTATIONS?: this switch turns on or off the presence of virus’ mutation and controls
the activation of the parameters below
9. MUTATION-CHANCE (0-100): probability of viral mutation within the environment
10. INFECTION-CHANCE IF MUTATED (0-100): probability of transmission of the
disease from one agent to another when the virus is mutated
11. CHANCE-INFECTED-IF-VACCINATED-MUTATED (0-100): probability of getting
infected with the mutation when the agent is vaccinated
12. RECOVERY-CHANCE-MUTATED (0-100): probability of recovering while being
infected with the virus’ mutation
13. RECOVERY-TIME-MUTATED (0-500): average recovery time for the mutation’s
infection, measured in ticks
14. Graph that shows the cumulative states of all the agents - differentiated by color -
over time.
15. Graph that shows the infection and recovery rates - differentiated by color - over time
16. Graph that shows the number of agents in every state at every given moment during
the simulation
Further improvements of the model can be easily introduced by adding new variables, with
the goal of providing a more comprehensive tool to simulate and analyze the expected
effectiveness of possible public health policies, such as non-pharmaceutical interventions or
vaccination policies.
