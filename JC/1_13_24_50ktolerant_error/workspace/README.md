During gen 472, got the following error:

Pulled b'\r\n' from MCU (sample 2/2)
Length of buffer: 2
Buffer entry 0: b'51331'
Buffer entry 1: b''
Traceback (most recent call last):
  File "/home/allyn/BitstreamEvolution/src/evolve.py", line 87, in <module>
    run()
  File "/home/allyn/BitstreamEvolution/src/evolve.py", line 77, in run
    evolution.evolve(
  File "/home/allyn/BitstreamEvolution/src/Evolution.py", line 66, in evolve
    population.evolve()
  File "/home/allyn/BitstreamEvolution/src/CircuitPopulation.py", line 450, in evolve
    fitness = circuit.get_fitness() if is_multi_pass else self.__eval_ckt(circuit)
  File "/home/allyn/BitstreamEvolution/src/CircuitPopulation.py", line 393, in __eval_ckt
    fitness = circuit.evaluate_pulse_count(record_data = record_data)
  File "/home/allyn/BitstreamEvolution/src/Circuit.py", line 325, in evaluate_pulse_count
    self.__microcontroller.simple_measure_pulses(self, self.__config.get_num_samples())
  File "/home/allyn/BitstreamEvolution/src/Microcontroller.py", line 105, in simple_measure_pulses
    buf[i] = int(buf[i])
ValueError: invalid literal for int() with base 10: b''

Since this was so close to the end of the experiment, I saved these results anyways

