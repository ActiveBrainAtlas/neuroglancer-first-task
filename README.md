# Neuroglancer-first-task

There are three brains named "MD585", "MD589", and "MD594".

For each of the three brains, we have a brain image stack (in Neuroglancer's tiled format), and we have a numpy volume. All of these files are stored on AWS S3.

## Data Storage

All files are stored in the bucket `neuroglancer-data` on AWS S3.

### Volume Files

- Since each volume is a single numpy file, we will provide links to each:
  - [MD585 volume](https://neuroglancer-data.s3-us-west-1.amazonaws.com/Neuroglancer_Volumes/Matrix/MD585/human_annotation/combined_volume/brainstem_xy5um_z20um/color_1_thickness_1_offset_0/volume_colored.npy)
  - [MD589 volume](https://neuroglancer-data.s3-us-west-1.amazonaws.com/Neuroglancer_Volumes/Matrix/MD589/human_annotation/combined_volume/brainstem_xy5um_z20um/color_1_thickness_1_offset_0/volume_colored.npy)
  - [MD594 volume](https://neuroglancer-data.s3-us-west-1.amazonaws.com/Neuroglancer_Volumes/Matrix/MD594/human_annotation/combined_volume/brainstem_xy5um_z20um/color_1_thickness_1_offset_0/volume_colored.npy)

### Image Files

Image files for each brain stack are stored in S3 in a folder. The filepath uses the following convention: `s3://neuroglancer-data/Neuroglancer_Images/Precomputed/<brain-name>/<brain-name>_prep2_raw_grayJpeg_precomputed`. Replace `<brain-name>` with one of the three brain names given above to get the proper filepath.
