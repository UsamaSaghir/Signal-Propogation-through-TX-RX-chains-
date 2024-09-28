The repository conatins a Matlab .m file that simulates the propogation of an 8PSK signal from a transmitter to a reciever passing through different channel Impairments.
Main stages of the implementation are:
* Generatelog2(M)×100000 random bits. where M = 8 for PSK.
* Encoding th eoriginal bit sequence with a Hamming code that maps k=4 source bits to n=7 coded bit– H(7,4),with help of the generator matrix G = (Ik |P).
  The parity array of the generator matrix reads
  p = |1 0 1|
      |1 1 1|
      |1 1 0|
      |0 1 1|
*  Use of Gray mapping to generate 100 000 8-PSK symbols from the encoded bit stream.
*  Implementation of Root-Raised Cosine transmitter filter (RRC) on generated 8-PSK symbols.
*  Addition of AWGN noise and complex chaneel impulse response on the transmitted symbols.
*  Implemtation of the reciever RRC filter.
*  Channel equilization using Least Mean Squares(LMS)algorithm-based equalizer.
*  Grey decoding and demodulation of symbols to recieved bit stream.
*  Hamming Decoding.
*  Bit-Error Rate (BER) Calculations for SNR from 0dB to 20dB. 
