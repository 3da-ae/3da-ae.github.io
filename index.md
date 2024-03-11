<p align="justify">We present a method enabling the scaling of NeRFs to learn a large number of semantically-similar scenes. We combine two techniques to improve the required training time and memory cost per scene. First, we learn a 3D-aware latent space in which we train Tri-Planes scene representations, hence reducing the resolution at which scenes are learned. Moreover, we present a way to share common information across scene representations, hence allowing for a reduction of model complexity to learn a particular scene. 
Our method reduces effective per-scene memory costs by 44% and per-scene time costs by 86% when training 1000 scenes.</p>

## Method
![Figure](assets/css/schema.svg)

We learn a 3D-aware latent space by regularizing its training with 3D constraints. To this end, we jointly train an encoder, a decoder and N scenes lying in this latent space. For each scene s, we learn a Tri-Planes representation T_s, built from the concatenation of local Tri-Planes T_s^{mic} and global Tri-Planes T_s^{mac}. T_s^{mic} is retrieved via a one-hot vector e_s from a set of scene-specific planes stored in memory. T_s^{mac} is computed from a summation of M globally shared Tri-Planes, weighted with weights W_s.

## Renders

### Visual comparison of renderings of our method and vanilla Tri-Planes trained in the image space.
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

### Visual comparison when training Tri-Planes on latent images coming from our 3Da-AE and the vanilla VAE.
<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Ours-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        Our method (Encode-Scene only)
    </div>
</center>

<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Vanilla-VAE-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        Vanilla VAE (Encode-Scene only)
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
