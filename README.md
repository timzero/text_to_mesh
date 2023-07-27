# Text to Mesh

The included notebook takes a text prompt and generates a 3D mesh. The steps to do so are as follows:

1. Generate image from text using __[Stable Diffusion pipeline](https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/text2img)__ 
2. Generate depth map using  __[DPTForDepthEstimation](https://huggingface.co/docs/transformers/main/en/model_doc/dpt#transformers.DPTForDepthEstimation)__
3. Convert depth map + image to rgbd image -> point cloud -> mesh using __[Open3D library](http://www.open3d.org/)__

### Prompt
`interior of a mountain chalet by frank lloyd wright`

### Image
![interior of a mountain chalet by frank lloyd wright](images/interior_of_a_mountain_chalet_by_frank_lloyd_wright-1690402022.png)

### Mesh
[interior_of_a_mountain_chalet_by_frank_lloyd_wright-1690431419.webm](https://github.com/timzero/text_to_mesh/assets/277352/657fe2be-d338-4f0a-b1ae-21353558ff9a)
