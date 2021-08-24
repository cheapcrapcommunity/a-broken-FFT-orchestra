![Screenshot 2021-08-24 at 1 43 08 PM](https://user-images.githubusercontent.com/76624368/130618308-da747eaa-490a-43a3-ae41-cbdd70ed4294.png)
# a-broken-FFT-orchestra

I want to create piece ‘played’ by a broken FFT orchestra with this project. 


First, I try to work with amplitude and phase directly by writing the amp values to a buffer and then breeding them back to reconstruct the FFT. Then I feed the sound into six delaylines which have different but very close phasor frequency as the main part of the inharmonic melody. 
  
 ![image](https://user-images.githubusercontent.com/76624368/130617546-2ecfe3ac-6c6b-4022-98d0-8b205ccd65b5.png)

Meanwhile, four of them are controlled by two random frequency generator, one gives integer between 7 to 9 and one between -900 to 900. Those two are going to make the melody glitch at some point of the track.

 
 ![image](https://user-images.githubusercontent.com/76624368/130617580-89c87bee-01a8-46cd-954d-0bea7d2fc605.png)
Sketch of track structure

![image](https://user-images.githubusercontent.com/76624368/130617619-f3f3d6b1-79ef-4055-a932-bb800ecf0ead.png)


Also, I feed the signal and turn it on and off immediately to create some micro beats. They are controlled by a 120 bpm sequencer. Another sequencer is 640 bpm, also receiving the original signal but it doesn’t turn off immediately, it’s like extending and delaying the microbeats.

Because there’s a tempo router controls  the tempo of writing the sample value. So the 4 mins track is symmetrical in structure but runs bpm 120, 640, 120, 640 in turn. 

