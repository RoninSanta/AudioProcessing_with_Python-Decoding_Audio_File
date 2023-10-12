# Audio Processing with Python-Decoding Audio File
The aim of this project is to use the python thinkdsp library to breakdown and decipher an encoded audio file, there are 3 exercises each with varying  levels of complexity.
- A encoded Audio file will be provided and the goal is to retrieve the hidden message buried at each complex layer

### Excercise 3.1 - Hidden text msg among audio file
A hidden text message is buried among the audio file, and a decoy music is used to mask the original message. Here are the steps to retieve the message:
- Convert the audio file into a byte array
- Use `LSB` method and get the lowest bit of the audio frame
- Convert the extracted bytes into a string text

### Excercise 3.2 - Secret passcode 
A secret audio message is recorded at a lower frequency than humans are able to hear. The message is also split across 3 audio files `sound2.wav`, `sound3.wav` and `sound4.wav` for added secrecy.

The method in solving this is quite straight forward:
- First combine the 3 audio files into one single file, lets call it `sound5.wav` and read from that
- The file will under go a high-pass filter to remove all sounds above a certain freq
- Then i will use demodulation to tune the sound into something recognizable


### Excercise 3.3 - Encode Message
Now I have to use the method I have learnt above and encode my own secert message using the techniques as an example.
