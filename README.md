# Tabor SE5082

2019/08/10

This code is for generating an arbitrary pulse sequence and load it to Tabor SE5082 for microwave control for Rydberg experiment.
(I can't find the code with block subvi somewhere else.)


## Type definition
variables: input variables from main GUI (lab counter timer control) \
sequence_variables: select type of sequence, number of repetition, and delay time\
waveform_variablese_new: detail frequency, phase, amplitude, and time duration of microwave pulse in each segment\

## subVI
test_GUI_with_seq: simulate main experimental control GUI interface\
Init_timestep_new: generate number of step required for each segment\
sine: generate sine pulse according to the input frequency, initial phase, amplitude, and sampling rate\
SE5082_xxx: SCPI command for the SE5082\

