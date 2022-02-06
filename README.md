## fod

### Resize images - 
- `find . -maxdepth 1 -iname "*.jpg" | xargs -L1 -I{} convert -resize 300x300 "{}" resized_images/"{}"`

### Train notebook - 
- https://colab.research.google.com/drive/1S4Ft9ZBzyxmZK1sVziewcvoU3bKDnswW?authuser=1#scrollTo=0tuLaFggpb-X

### Generate train set - 
- `python models/research/convert_tf.py ~/personal/sk/resized_images ~/personal/sk/new_nut_tagged "NUT1"`

### Run prediction - 
- `python3 webcam_predict.py ~/personal/sk/fod/fine_tuned_model`
