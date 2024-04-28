7 day sensivity  
-----
![1_sensitivity.png](plots/1_sensitivity.png)
![2_sensitivity_temp_humidity.png](plots/2_sensitivity_temp_humidity.png)
![3_sensitivity_avg_temp_humidity.png](plots/3_sensitivity_avg_temp_humidity.png)
![4_sensitivity_std_temp_humidity.png](plots/4_sensitivity_std_temp_humidity.png)
![5_change_over_time.png](plots/5_change_over_time.png)
-----
#### [TOP-LEVEL PARAMETERS]  
| Param | Value |  
|---|---|  
simulation_mode | INTRINSIC_SENSITIVITY  
#### [FITNESS PARAMETERS]  
| Param | Value |  
|---|---|  
fitness_func | PULSE_COUNT  
desired_freq | 30000  
combined_mode | MULT  
pulse_weight | 2  
var_weight | 0  
num_samples | 1  
num_passes | 1  
#### [FITNESS SENSITIVITY PARAMETERS]  
| Param | Value |  
|---|---|  
test_circuit | data/sensitvity_seeds/4_20_24_30k.asc  
sensitivity_trials | IGNORE  
sensitivity_time | 007:00:00:00  
reading_temp_humidity | true  
environment_usb_path | /dev/ttyUSB0  
#### [LOGGING PARAMETERS]  
| Param | Value |  
|---|---|  
log_level | 4  
save_log | true  
save_plots | true  
backup_workspace | true  
log_file | ./workspace/log  
plots_dir | ./workspace/plots  
output_dir | ./prev_workspaces  
asc_dir | ./workspace/experiment_asc  
bin_dir | ./workspace/experiment_bin  
data_dir | ./workspace/experiment_data  
analysis | ./workspace/analysis  
best_file | ./workspace/best.asc  
src_populations_dir | ./workspace/source_populations  
monitor_file | /home/ubuntu/BitstreamEvolution/data/monitor  
generations_dir | ./workspace/generations  
datetime_format | %%m/%%d/%%Y - %%H:%%M:%%S  
show_ovr_best | true  
#### [SYSTEM PARAMETERS]  
| Param | Value |  
|---|---|  
fpga | i:0x0403:0x6010:0  
usb_path | /dev/ttyUSB1  
auto_upload_to_arduino | false  
#### [HARDWARE PARAMETERS]  
| Param | Value |  
|---|---|  
routing | MOORE  
mcu_read_timeout | 1.5  
serial_baud | 115200  
accessed_columns | 14,15,24,25,40,41  
configurable_io | false  
input_pins | 45,47,48  
output_pins | 44  
#### [GA PARAMETERS]  
| Param | Value |  
|---|---|  
population_size | 50  
mutation_probability | 0.0021  
crossover_probability | 0.7  
elitism_fraction | 0.1  
selection | FIT_PROP_SEL  
diversity_measure | HAMMING_DIST  
random_injection | 0.0  
#### [INITIALIZATION PARAMETERS]  
| Param | Value |  
|---|---|  
init_mode | CLONE_SEED_MUTATE  
randomize_until | NO  
randomize_threshold | 4  
; Note: Randomization goes through the population. Therefore, if doing MUTATE with CLONE_SEED and pop size | 50, for example,  
randomize_mode | RANDOM  
#### [STOPPING CONDITION PARAMETERS]  
| Param | Value |  
|---|---|  
generations | 500  
target_fitness | IGNORE  
#### [TRANSFERABILITY PARAMETERS]  
| Param | Value |  
|---|---|  
transfer_interval | IGNORE  
fpga2 | i:0x0403:0x6010:0  
