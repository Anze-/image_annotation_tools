# 2024 Tools for Image Annotation: task data preparation for Deep Learning training/finetuning
A quick lookup at 2024 image annotation tools: in 2024 one would expect to have a plethora of tools to label images for object detection/segmentation tasks, while this is somehow true, it is not immediately obvious which tool is better suited to which needs, hence this readme file.

## Large Categories, pros and cons:
 * **cloud based**: + processing power, zero setup ; - data privacy, bandwidth
 * **on premise**: + data privacy, zero bandwidth; - requires setup
   * **server side**: + can access data on your remote workstation locally
   * **client side**: + can only access data on your local machine
  
## Tested options

**repo**: complexity, cloud/premise, server/client, extra notes notes

*  **HumanSignal/labelImg**: intermediate, on premise, client side (executable)
*  **ox-vgg/via**: intermediate, on premise, client side, single html website which can be useful for local data
*  **HumanSignal/label-studio**: simple, on premise, server side, BUT sends lot of metrics and diagnostics and it's not currently possible to stop this behavoiur, requires account
* **l3p-cv/lost**: complex, on premise, server side, (good for larger multi user companies)
* **UniversalDataTool/universal-data-tool**: intermediate, can run as docker, premise, webapp, jupyter widget etc... but in practice it's not working any more
* **Hitachi-Automotive-And-Industry-Lab/semantic-segmentation-editor**: bloated and overcomplicated, outdated
* **BMW-InnovationLab/BMW-Labeltool-Lite**: intermediate, on premise, server side, the best tool to work with server-side data storage NOTE: ssh domain.com -L 8000:localhost:8000 -L frontendport:localhost:8081
* **RTIInternational/SMART**: intermediate, dockerized, but not thought to manage data on the server side
* **IDEA-Research/deepdataspace**: intermediate, client side, on premise (it's hard to find a tool thought to manage data on the server side!!!)
* **rediscovery-io/remo-python**: looks amazing, but their website is down and both the pip package and the docker installation pull from 404 resources
* **AlvaroCavalcante/auto_annotate**: ...
* **IndustryEssentials/label-free**: mainly chinese, english full manual not existing, it has an option to load data from a server ip, but it's unclear
* **jaxony/turktool**: simple, react app that can be used in many deployments fashion 
