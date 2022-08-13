# Digital-Watermaring-using-LSB
Invisible Digital Image Watermarking in spatial domain using LSB bit manipulation


Invisible Digital Image Watermarking in
spatial domain using LSB bit manipulation
 Divyansh Nirman (2019244)

Mentor:
Dr. Durgesh Singh

Abstract





Information technology has eased the duplication, manipulation and distribution of
digital data in recent times which has resulted in the demand for safe ownership of
digital images.
A very crucial concern for the content owners and distributors is copyright
protection and content authentication.
The solution to these problems is Digital Watermarking. The watermarking is the
process of embedding a signal in to other signal robustly and invisibly at the same
time.

Index of Contents

Introduction​
Why watermarking?
Types of watermarking​
Applications of Watermarking​
Spatial watermarking​
Spatial Domain Techniques​
Advantages of Using LSB
Watermarking algorithm
Advantages and Disadvantages
Conclusion​
References

What is watermarking?




Watermarking is the process of superimposing a logo or
piece of text atop a document or image file, and it’s an
important process when it comes to both the copyright
protection and marketing of digital works.
While the watermarking process is mostly digital these
days, the term “watermarking” itself dates back
centuries. Traditionally, a watermark was only visible
when the paper was held up to the light or when it was
wet, and the process of watermarking paper occurred
while the paper was wet—hence the term we still use
today.

Block diagram of watermarking system

Why watermarking is used?




There are a couple of key reasons why you might need to watermark a document
or image. On one end, watermarking helps protect the copyright of your work and
ensures that it cannot be reused or altered without your permission. This means
that people can still preview your work before purchasing it, without the risk of
them stealing it.
In other cases, a digital watermark may act as a stamp, to indicate the status of a
document, with terms like “VOID,” “COPY,” or “SAMPLE.” This ensures that
important documents are never mishandled, helping you keep your work organized
as you take it from draft to finalization

Types of watermarking


Visible Watermarks: These watermarks are visible.



Invisible Watermarks: These watermarks are embedded in the media and use steganography
techniques. They are not visible by naked eyes.



Public Watermarks: These can be understood and modified by anyone using certain algorithms.
These are not secure.



Fragile Watermarks: These watermarks are destroyed by data manipulation. There must be a
system which can detect all changes in the data if fragile watermarks are to be used.

Application of watermarking












Copyright protection
Content identification and management
Digital forensic
Military
Broadcast monitoring
Media file archiving
Covert communication
Remote education
Smart healthcare
Fingerprinting
Securing E-Voting and licenses

Spatial Domain Digital Watermarking






Spatial Domain Digital Watermarking is a technique for the insertion of
watermarked information (side information defined by the owner) into the source
(cover) image/video in the spatial domain.
The most common algorithm for spatial domain watermarking is Least Significant
Bit Modification. This method changes the least significant bits (LSB) of chosen
pixels in the image. It is possible to use more LSB bits of the container image in a
similar way.
The watermark object may also be embedded many times within the container
image. Even if most of the watermarks are lost due to attacks, a single surviving
one is enough.

Advantages of Using LSB




LSB is the Least Significant Bit, that means the last bit in binary representation
which is 20.
So upon changing the LSB of the image wo be watermarked, we will be changing
the value of its color at most by one.
This small change is not visible to a naked eye hence our image gets watermarked
by another image with the pixels on LSB.

Watermarking Algorithm

Original Image

Watermark Image

Comparing watermarking on different bits

Watermarking on last bit (LSB)

Watermarking on 2nd last bit

Watermarking on 3rd last bit

Contd.





Upon comparison, we can see that the watermark becomes visible as we move
towards the Most Significant Bit.
So to hide image from naked eye, we should be changing the LSB.
The algorithm is pretty simple, we convert the original image to grayscale and
binarize the watermark so as to hide it easily in the image.
Then for every pixel we check for the binary of watermark and replace it in the
original image array.

Extracting watermarking using LSB
substitution
Extracting Algorithm:
1. Iterate over all the pixels in watermarked image.
2. Store in the array the LSB of that pixel, if LSB is 1 store 255, else
store 0.
3. Resize the flatten array to the size of original image that was
hidden.
4. Then display the image from the resized array and check if it was
same as the earlier.

Extracted Image

Advantages





Simple to implement
Decryption algorithm not required. So a person unknown to cryptography can
decrypt the message.
We can send cipher image through FAX or E-MAIL.
Lower computational cost since the secret message is recognized only by human
eyes and not cryptographically computed.

Disadvantages





The contrast of the reconstructed image is not maintained.
Perfect alignment of the transparencies is troublesome.
Due to pixel expansion the width of the decoded image is twice that of the original
image which leads to loss of information due to a change in aspect ratio.
Additional processing is required for coloured images.

Conclusion
The classification and methods of image watermarking and evaluates LSB based digital
watermarking scheme. After we have embedded the secret data in the first bit i.e. LSB in
the image we got Watermarked Image without noticeable distortion on it.
However when we embed the data in the consequent bits i.e. second towards last MSB
bit, the image start distorted.

References



https://link.springer.com/article/10.1007/s11042-017-5222-8
https://experience.dropbox.com/resources/what-is-watermarking



https://www.ijsr.net/archive/v4i4/29031501.pdf



https://towardsdatascience.com/hiding-data-in-an-image-image-steganography-usi



ng-python-e491b68b1372
Neha Jadhav, S. K. (2015). Digital Watermarking Using Least Significant Bit
Algorithm. International Journal of Emerging Technologies and Engineering (IJETE) ,
43-46.

Thank
You!
