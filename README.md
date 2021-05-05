# Steganography

## What is Steganography?
> **Steganography** is the process of hiding a secret message within a larger one in such a way that someone can not know the presence or contents of the hidden message.
The purpose of Steganography is to maintain secret communication between two parties.

### Steganography vs cryptography
<table><td></td><td><span><strong><span>STEGANOGRAPHY</span></strong></span></td><td><span><strong><span>CRYPTOGRAPHY</span></strong></span></td></tr><tr><td><span><strong><span>Definition</span></strong></span></td><td><span>It is a technique to hide the existence of communication</span></td><td><span>It’s a technique to convert data into&nbsp;an incomprehensible form</span></td></tr><tr><td><span><strong><span>Purpose</span></strong></span></td><td><span>Keep communication secure</span></td><td><span>Provide data protection</span></td></tr><tr><td><span><strong><span>Data Visibility</span></strong></span></td><td><span>Never</span></td><td><span>Always</span></td></tr><tr><td><span><strong><span>Data Structure</span></strong></span></td><td><span>Doesn’t alter the overall structure of data</span></td><td ><span>Alters the overall structure of data</span></td></tr><tr><td ><span><strong><span>Key</span></strong></span></td><td><span>Optional, but offers more security if used</span></td><td><span>Necessary requirement</span></td></tr><tr><td><span><strong><span>Failure</span></strong></span></td><td><span>Once the presence of a secret message is discovered, anyone can use the secret data</span></td><td><span>If you possess the decryption key, then you can figure out original message from the ciphertext</span></td></tr></tbody></table>

 
### Advantage of using Steganography over Cryptography?
1. Used besides cryptography to add more protective layers to the hidden data.
2. The intended secret message does not attract attention to itself as the subject of scrutiny.

## Types of Steganography
Depending on the nature of the cover object(actual object in which secret data is embedded), steganography can be divided into five types:
1. Text Steganography
2. Image Steganography
3. Video Steganography
4. Audio Steganography
5. Network Steganography

![Types of Steganography!](/images/1_types.png "Types of Steganography")

## Basic Steganographic Model
![Steganographic Model!](/images/2_model.png "Steganographic Model")

1. The **original** image file(X) and **secret** message (M) needs to be hidden are fed into a steganographic encoder as input. 
2. Steganographic Encoder function, f(X,M,K) embeds the secret message into a cover image file by using techniques like least significant bit encoding.
3. The resulting stego image looks very similar to your cover image file, with no visible changes. This completes encoding. 
4. To retrieve the secret message, stego object is fed into Steganographic Decoder.

