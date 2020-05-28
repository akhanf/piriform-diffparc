# piriform-diffparc
Diffusion parcellation of piriform cortex snakemake workflow

## Required Inputs:
* custom template image (can be multi-chan)
* target images (can be multi-chan)
* seed segs in template space 
* freesurfer output for generating target segs
* pre-processed DWI output (e.g. dwi/bvec/bval/grad_dev) in target native space (e.g. T1w space)
* pre-processed bedpostx (e.g. merged_...)

## Steps
* prepping seed/target segs
* probtrack --OR-- mrtrix3 tracking
* generating seed-based connectivity maps
* group-wise clustering
* indiv results

