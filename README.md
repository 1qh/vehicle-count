# Vehicle Count using StrongSORT and YOLOv5

How to run our code
```
git clone https://github.com/1qh/vehicle-count
cd vehicle-count
pip install https://github.com/KaiyangZhou/deep-person-reid/archive/master.zip
pip install -r requirements.txt
```

### Track and count object

```
python count1lane.py \
    --yolo-weights weights/trained_v5.pt \
    --strong-sort-weights weights/osnet_x0_25_msmt17.pt \
    --source video/one-lane.mp4 \
    --save-vid
```

```
python count2lane.py \
    --yolo-weights weights/trained_v5.pt \
    --strong-sort-weights weights/osnet_x0_25_msmt17.pt \
    --source video/two-lane.mp4 \
    --save-vid
```
For video sample: https://drive.google.com/drive/folders/146iVxlrW0Y3IcV3OpQdEUMJc4k-Gd_vh?usp=sharing
