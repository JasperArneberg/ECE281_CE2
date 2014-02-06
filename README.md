ECE281_CE2
==========

Computer Exercise 2

###### Jasper Arneberg
###### M6A ECE 281
###### Dr. Neebel

# Truth Table as Tested

| I0 | I1 | EN | Y0 | Y1 | Y2 | Y3 |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 | 0 | 0 |
| 0 | 1 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 | 1 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 |
| 1 | 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 | 1 |

# Truth Table Rearranged
This rearrangement makes it easier to see what the decoder is really doing.

| I0 | I1 | EN | Y0 | Y1 | Y2 | Y3 |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: |
| 0 | 0 | 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 0 | 0 | 0 | 0 | 0 |
| 0 | 1 | 0 | 0 | 0 | 0 | 0 |
| 1 | 1 | 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 1 | 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 0 | 1 | 0 | 0 |
| 0 | 1 | 1 | 0 | 0 | 1 | 0 |
| 1 | 1 | 1 | 0 | 0 | 0 | 1 |


# Structural Waveform Output

![alt text](https://github.com/JasperArneberg/ECE281_CE2/blob/master/structural_waveform.png?raw=true "Structural Screenshot")

# Behavioral Waveform Output

![alt text](https://github.com/JasperArneberg/ECE281_CE2/blob/master/behavioral_waveform.png?raw=true "Behavioral Screenshot")

# Analysis

Both the behavioral and structural implementations of the circuit behaved as they should during simulation. The waveforms match each other exactly, and they correspond with the truth table correctly. The reason the waveforms appear slightly different than the provided example is because the varying inputs were tested in a different sequence.

# Decoder

In this computer exercise, a 2-to-4 line single-bit decoder was constructed. A decoder retrieves encoded information, essentially doing the reverse process of an encoder. The EN input is an enable switch on the decoder itself. In the context of computer memory, encoding information takes up a lot less space. A decoder is necessary to retrieve this information back, however, in the desired form.

Documentation: http://en.wikipedia.org/wiki/Decoder
