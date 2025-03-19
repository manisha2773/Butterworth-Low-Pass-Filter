# Butterworth-Low-Pass-Filter

The code applies a Butterworth Low-Pass Filter (BLPF) to an image in the frequency domain to remove high-frequency details such as noise and sharp edges while preserving smooth variations. It first converts the image from the spatial domain (pixel values) to the frequency domain using the Fast Fourier Transform (FFT). This transformation represents the image in terms of its frequency components, where low frequencies correspond to smooth regions and high frequencies represent fine details.

A Butterworth low-pass filter is then created, which gradually attenuates high frequencies instead of cutting them off abruptly. This ensures a smooth transition between preserved and removed frequencies, reducing artifacts like ringing. The filter is applied by multiplying it with the transformed image, effectively suppressing unwanted high-frequency components. Finally, the Inverse Fourier Transform (IFFT) is used to convert the filtered frequency data back into the spatial domain, producing a blurred version of the original image.

This method is commonly used in image processing for noise reduction, edge smoothing, and preprocessing before further analysis. Compared to other low-pass filters, the Butterworth filter provides a more natural blurring effect without introducing sharp distortions, making it useful in applications like medical imaging and pattern recognition.






