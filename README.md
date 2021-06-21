# PC_L13_Inpainting_Audio
## Project Course 2020/2021 @POLIMI Music & Acoustic Engineering

Welcome to the project L13 of the *Project Course A.Y. 2020/2021* from *Politecnico di Milano*.

The aim of this project is to test and analyze some of the main image inpainting methods... but applied to audio!

The idea is to treat audio as image by obtaining a frequency representation (**STFT** or **MEL**).

Then corrupt this audios in different ways (corrupting **time axis** or **frequency axis**) and in progressive way, starting from a little (imperceptible) degradation.

Our evaluation consist in a confront on both the reconstructed image (metrics: **PSNR** and **SSIM**) and the reconstructed audio (metrics: **SNR** and **PESQ**).

Also, the reconstruction from audio to image can be implemented in two ways: using **original phase** or approximating it with **griffinlim** algorithm.

A brief description on the project can be found in *Project_Requirements.pdf*

Further details on the whole project on our report *L13.pdf* inside report folder.

More details about the scripts implementation on *Documentation.pdf* inside documentation folder.

##### USEFUL LINKS
- [Model Based Inpainting Method](https://scikit-image.org/docs/stable/auto_examples/filters/plot_inpaint.html)
- [Pix 2 Pix Inpainting Method](https://paperswithcode.com/paper/image-to-image-translation-with-conditional)
- [Deep Prior Inpainting Method](https://github.com/DmitryUlyanov/deep-image-prior)
- [griffinlim](https://librosa.org/doc/main/generated/librosa.griffinlim.html)
- [PESQ](https://pypi.org/project/pesq/)
- [SSIM](https://scikit-image.org/docs/dev/auto_examples/transform/plot_ssim.html)

##### HOW TO READ RESULTS
*example:* model_based_5_it_x_20_cols, means **model based** method applied for **5 iterations** each of **20 columns** of degradation (apart from the first which is of only 1 row/column), so in this example we have a total of 4x20 = 80 degradated columns.


**Column** degradation means degradating **time** axis, while **Rows** degradation refers to **frequency** axis.
