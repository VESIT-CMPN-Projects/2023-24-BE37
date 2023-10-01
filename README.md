# Fetal_Brain_Anomalies

**To Run the code Locally:** <br>

clone the repo locally
create virtual env 

**install dependencies**<br>
pip install django<br>
pip install django-crispy-forms<br>
pip install django-cleanup<br>
pip install django-debug-toolbar<br>
pip install celery<br>
pip install yolov5<br>

**Change Directory**<br>
cd replace_directory


**migrate**<br>
python manage.py migrate

**create super user**<br>
python manage.py createsuperuser # (it may show an error page if no 'default.png' in media folder. See note.)

Note<br>
An image with the name default.png in media folder is required for user-profile. Create media folder and add any image file with this name 'default.png'.

**run**<br>
python manage.py runserver

**login**<br>
Login at the web address 127.0.0.1:8000 using the superuser credentials.

**Create ImageSet**<br>
create an ImageSet first and then upload images into the ImageSet from ImageSet detail page.

On images list page click on detect object.

select a YoloV5 model
the YoloV5 dependencies and pre-trained model will start downloading.

# Classes Identified in the project are :

| Class                      | Images | Instances | Box(P) | R     | mAP50 | mAP50-95 | Mask(P) | R     | mAP50 | mAP50-95 |
| -------------------------- | ------ | --------- | ------ | ----- | ----- | -------- | ------- | ----- | ----- | -------- |
| all                        | 357    | 381       | 0.901  | 0.942 | 0.962 | 0.637    | 0.896   | 0.935 | 0.957 | 0.55     |
| anold chiari malformation  | 357    | 10        | 0.935  | 1     | 0.995 | 0.679    | 0.935   | 1     | 0.995 | 0.505    |
| arachnoid cyst             | 357    | 22        | 1      | 0.968 | 0.995 | 0.662    | 1       | 0.968 | 0.995 | 0.62     |
| cerebellah hypoplasia      | 357    | 32        | 0.844  | 0.845 | 0.897 | 0.633    | 0.875   | 0.876 | 0.943 | 0.583    |
| cisterna magna             | 357    | 10        | 0.789  | 1     | 0.977 | 0.599    | 0.71    | 0.9   | 0.887 | 0.479    |
| colphocephaly              | 357    | 29        | 0.802  | 0.724 | 0.842 | 0.438    | 0.802   | 0.724 | 0.842 | 0.429    |
| encephalocele              | 357    | 37        | 1      | 0.915 | 0.953 | 0.652    | 1       | 0.915 | 0.953 | 0.631    |
| holoprosencephaly          | 357    | 4         | 0.862  | 1     | 0.995 | 0.846    | 0.862   | 1     | 0.995 | 0.647    |
| hydracenphaly              | 357    | 8         | 0.91   | 1     | 0.995 | 0.765    | 0.91    | 1     | 0.995 | 0.728    |
| intracranial hemorrdge      | 357    | 18        | 1      | 0.94  | 0.972 | 0.505    | 1       | 0.94  | 0.972 | 0.545    |
| intracranial tumor          | 357    | 1         | 0.781  | 1     | 0.995 | 0.697    | 0.781   | 1     | 0.995 | 0.298    |
| mild ventriculomegaly       | 357    | 72        | 0.956  | 0.907 | 0.935 | 0.56     | 0.956   | 0.907 | 0.942 | 0.502    |
| moderate ventriculomegaly   | 357    | 71        | 0.79   | 0.956 | 0.951 | 0.646    | 0.79    | 0.956 | 0.951 | 0.599    |
| polencephaly                | 357    | 32        | 1      | 0.968 | 0.988 | 0.588    | 1       | 0.968 | 0.988 | 0.549    |



