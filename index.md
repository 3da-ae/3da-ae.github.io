<p align="justify">We present a method enabling the scaling of NeRFs to learn a large number of semantically-similar scenes. We combine two techniques to improve the required training time and memory cost per scene. First, we learn a 3D-aware latent space in which we train Tri-Planes scene representations, hence reducing the resolution at which scenes are learned. Moreover, we present a way to share common information across scene representations, hence allowing for a reduction of model complexity to learn a particular scene. 
Our method reduces effective per-scene memory costs by 44% and per-scene time costs by 86% when training 1000 scenes.</p>

## Method
![Figure](assets/css/schema.svg)

We learn a 3D-aware latent space by regularizing its training with 3D constraints. To this end, we jointly train an encoder, a decoder and N scenes lying in this latent space. For each scene s, we learn a Tri-Planes representation T<sub>s</sub>, built from the concatenation of local Tri-Planes T<sub>s</sub><sup>mic</sup> and global Tri-Planes T<sub>s</sub><sup>mac</sup>. T<sub>s</sub><sup>mic</sup> is retrieved via a one-hot vector e<sub>s</sub> from a set of scene-specific planes stored in memory. T<sub>s</sub><sup>mac</sup> is computed from a summation of M globally shared Tri-Planes, weighted with weights W<sub>s</sub>.

## Learning scenes with 3Da-AE

After training a 3D-aware autoencoder, we utilize it to train Tri-Plane scene representations in its latent space.

### Comparison of Latent Tri-Planes and Tri-Planes (RGB)
<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Ours-Decode-pre-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        Our method
    </div>
</center>

<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/RGB-Triplanes.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        Tri-Planes (RGB)
    </div>
</center>

### Comparison of Latent Tri-Planes: 3Da-AE vs baseline AE
<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Ours-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        3Da-AE (ours)
    </div>
</center>

<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Vanilla-VAE-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        Baseline AE
    </div>
</center>


## Citation
```
@article{,
  title={},
  author={},
  journal={},
  year={}
}
```
