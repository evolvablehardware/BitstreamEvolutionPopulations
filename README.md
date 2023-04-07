# BitstreamEvolutionPopulations
Experiments are stored in folders based on which FPGA they were run on

## Standard Config
population_size = 50
generations = 500
genotypic_length = 24
mutation_probability = 0.0021
crossover_probability = 0.7
elitism_fraction = 0.1
desired_freq = 10000
selection = FIT_PROP_SEL
randomize_until = NO
variance_threshold = 4
init_mode = RANDOM
pulse_func = True
simulation_mode = FULLY_INTRINSIC
diversity_measure = HAMMING_DIST
fitness_func = VARIANCE
sampling_method = MEDIAN
measurement_type = VARIANCE
num_samples = 2
random_injection = 0.15

