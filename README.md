# Steganography

## What is Steganography?
> **Steganography** is the process of hiding a secret message within a larger one in such a way that someone can not know the presence or contents of the hidden message.
The purpose of Steganography is to maintain secret communication between two parties.

### Steganography vs cryptography
<table><td></td><td><span><strong><span>STEGANOGRAPHY</span></strong></span></td><td><span><strong><span>CRYPTOGRAPHY</span></strong></span></td></tr><tr><td><span><strong><span>Definition</span></strong></span></td><td><span>It is a technique to hide the existence of communication</span></td><td><span>It’s a technique to convert data into&nbsp;an incomprehensible form</span></td></tr><tr><td><span><strong><span>Purpose</span></strong></span></td><td><span>Keep communication secure</span></td><td><span>Provide data protection</span></td></tr><tr><td><span><strong><span>Data Visibility</span></strong></span></td><td><span>Never</span></td><td><span>Always</span></td></tr><tr><td><span><strong><span>Data Structure</span></strong></span></td><td><span>Doesn’t alter the overall structure of data</span></td><td ><span>Alters the overall structure of data</span></td></tr><tr><td ><span><strong><span>Key</span></strong></span></td><td><span>Optional, but offers more security if used</span></td><td><span>Necessary requirement</span></td></tr><tr><td><span><strong><span>Failure</span></strong></span></td><td><span>Once the presence of a secret message is discovered, anyone can use the secret data</span></td><td><span>If you possess the decryption key, then you can figure out original message from the ciphertext</span></td></tr></tbody></table>

 
### Advantage of using Steganography over Cryptography?
1. Used besides cryptography to add more protective layers to the hidden data.
2. The intended secret message does not attract attention to itself as the subject of scrutiny.

## Basic Steganographic Model
![Steganographic Model!](/images/2_model.png "Steganographic Model")

1. The **original** image file(X) and **secret** message (M) needs to be hidden are fed into a steganographic encoder as input. 
2. Steganographic Encoder function, f(X,M,K) embeds the secret message into a cover image file by using techniques like least significant bit encoding.
3. The resulting stego image looks very similar to your cover image file, with no visible changes. This completes encoding. 
4. To retrieve the secret message, stego object is fed into Steganographic Decoder.


## Types of Steganography
Depending on the nature of the cover object(actual object in which secret data is embedded), steganography can be divided into five types:
1. Text Steganography
2. Image Steganography
3. Video Steganography
4. Audio Steganography
5. Network Steganography

![Types of Steganography!](/images/1_types.png "Types of Steganography")


### Text Steganography
Text Steganography is hiding information inside the text files. It involves things like changing the format of existing text, changing words within a text, generating random character sequences or using context-free grammars to generate readable texts. Various techniques used to hide the data in the text are:
* Format Based Method
* Random and Statistical Generation
* Linguistic Method

### Image Steganography
Hiding the data by taking the cover object as the image is known as image steganography.  In digital steganography, images are widely used cover source because there are a huge number of bits present in the digital representation of an image. There are a lot of ways to hide information inside an image. Common approaches include:
* Least Significant Bit Insertion
* Masking and Filtering
* Redundant Pattern Encoding
* Encrypt and Scatter
* Coding and Cosine Transformation

### Audio Steganography
The secret message is embedded into an audio signal which alters the binary sequence of the corresponding audio file. Hiding secret messages in digital sound is a much more difficult process when compared to others, such as Image Steganography. Different methods of audio steganography include:
* Least Significant Bit Encoding
* Parity Encoding
* Phase Coding
* Spread Spectrum

This method hides the data in WAV, AU, and even MP3 sound files.


### Video Steganography
One can hide kind of data into digital video format. The advantage of this type is a large amount of data can be hidden inside and the fact that it is a moving stream of images and sounds. You can think of this as the combination of Image Steganography and Audio Steganography. 
Two main classes of Video Steganography include:
1. Embedding data in uncompressed raw video and compressing it later
2. Embedding data directly into the compressed data stream

## Best Tools to Perform Steganography
There are many software available that offer steganography. *Some offer normal steganography, but a few offer encryption before hiding the data.*
hese are the steganography tools which are available for free:
1. **Stegosuite** is a free steganography tool which is written in Java. With Stegosuite you can easily hide confidential information in image files.
2. **Steghide** is an open source Steganography software that lets you hide a secret file in image or audio file.
3. **Xiao Steganography** is a free software that can be used to hide data in BMP images or in WAV files.
4. **SSuite** Picsel is another free portable application to hide text inside an image file but it takes a different approach when compared to other tools.
5. **OpenPuff** is a professional steganographic tool where you can store files in image, audio, video or flash files

