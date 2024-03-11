<p align="justify">We present a method enabling the scaling of NeRFs to learn a large number of semantically-similar scenes. We combine two techniques to improve the required training time and memory cost per scene. First, we learn a 3D-aware latent space in which we train Tri-Planes scene representations, hence reducing the resolution at which scenes are learned. Moreover, we present a way to share common information across scene representations, hence allowing for a reduction of model complexity to learn a particular scene. 
Our method reduces effective per-scene memory costs by 44% and per-scene time costs by 86% when training 1000 scenes.</p>

## Method
![Figure](assets/css/schema.svg)

## Renders
<center>
    <div>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Ours-Decode-pre-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Ours-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/RGB-Triplanes.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> <br>
        <video width="60%" height="60%" autoplay muted loop playsinline>
            <source src="assets/css/Vanilla-VAE-Encode.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
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
