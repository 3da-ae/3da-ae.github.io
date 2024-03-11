<p align="justify">Modeling large scenes from unconstrained images has proven to be a major challenge in computer vision. Existing methods tackling in-the-wild scene modeling operate in closed-world settings, where no conditioning on priors acquired from real-world images is present. We propose RefinedFields, which is, to the best of our knowledge, the first method leveraging pre-trained models to improve in-the-wild scene modeling. We employ pre-trained networks to refine K-Planes representations via optimization guidance using an alternating training procedure.
We carry out extensive experiments and verify the merit of our method on synthetic data and real tourism photo collections. RefinedFields enhances rendered scenes with richer details and outperforms previous work on the task of novel view synthesis in the wild.</p>

## Method
![Figure](assets/css/schema.svg)

We learn a scene through two alternating stages.
_Scene fitting_ optimizes our K-Planes representation to reproduce the images in the training set, as traditionally done in neural rendering techniques.
_Scene refining_ finetunes a pre-trained prior and infers a new _refined_ K-Planes representation, which will subsequently be corrected by scene fitting.

## In-the-wild Renders
<center>
    <div>
<!--         <video width="30%" height="30%" autoplay muted loop playsinline>
            <source src="assets/css/brandenburg.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video> -->
        <video width="30%" height="30%" autoplay muted loop playsinline>
            <source src="assets/css/sacre.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="30%" height="30%" autoplay muted loop playsinline>
            <source src="assets/css/trevi.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
    </div>
</center>

## Synthetic Renders
<center>
    <div>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/chair.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/drums.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/ficus.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/hotdog.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
    </div>
    <div>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/lego.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/materials.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/mic.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
        <video width="23%" height="23%" autoplay muted loop playsinline>
            <source src="assets/css/ship.mp4" type="video/mp4" style="display: inline-block;">
            Your browser does not support the video tag.
        </video>
    </div>
</center>

## Citation
```
@article{kassab2023refinedfields,
  title={RefinedFields: Radiance Fields Refinement for Unconstrained Scenes},
  author={Kassab, Karim and Schnepf, Antoine and Franceschi, Jean-Yves and Caraffa, Laurent and Mary, Jeremie and Gouet-Brunet, Val{\'e}rie},
  journal={arXiv preprint arXiv:2312.00639},
  year={2023}
}
```
