{% assign imagesample = site.data[site.metadata] | where_exp: 'item','item.format contains "image"' | first %}
{% capture imagesampleid %}{{imagesample.objectid | default: ("https://raw.githubusercontent.com/ARVEVS/sitiopostales/main/objects/C2-G2-001-a.jpg")![image](https://user-images.githubusercontent.com/130485533/236248577-cb435adc-e97a-44ab-ad2f-a5a82a6eae40.png)
"}}{% endcapture %}
{% assign pdfsample = site.data[site.metadata] | where_exp: 'item','item.format contains "pdf"' | first %}
{% capture pdfsampleid %}{{pdfsample.objectid | default: "https://digital.lib.uidaho.edu/utils/getfile/collection/ui_ep/id/21768/filename/uiext21768.pdf"}}{% endcapture %}
{% assign videosample = site.data[site.metadata] | where_exp: 'item','item.format contains "video"' | first %}
{% capture videosampleid %}{{videosample.objectid | default: "https://cdil.lib.uidaho.edu/storying-extinction/objects/trailcams/videos/ballcreek-cedarrub-birdonpath.mp4"}}{% endcapture %}
{% assign audiosample = site.data[site.metadata] | where_exp: 'item','item.format contains "audio"' | first %}
{% capture audiosampleid %}{{audiosample.objectid | default: "https://www.lib.uidaho.edu/digital/mp3s/Clouds.mp3"}}{% endcapture %}

## Sobre nuestra página

El objetivo del proyecto es conservar las postales y ponerlas a disposición de entusiastas de la historia, investigadores, profesores y estudiantes en formato digital. Los usuarios pueden buscar, navegar, ordenar y seleccionar temas, lugares y edificios destacables de las ciudades europeas a inicios del siglo XX.El proyecto contiene alrededor de un centenar de postales digitalizadas con información sobre su procedencia, ubicación geográfica, temas, descripción, fecha (cuando fue posible) y metadatos como color, medidas y tipo de archivo (application/pdf). El proceso incluyó la digitalización de las postales, la identificación de su ubicación geográfica, el ordenamiento y clasificación en carpetas, y enriquecimiento con datos y metadatos. Finalmente, se utilizaron estas postales para poblar el Collection Builder. El repositorio forma parte del Curso de Humanidades Digitales de la Ibero en primavera 2023.

Si desea colaborar, puede ponerse en contacto a través del siguiente enlace: https://arvevs.github.io/sitiopostales/ 

{% include feature/image.html objectid=imagesampleid width="75" %}
