# Adding network \(IP\) cameras

Bluecherry supports several different ways to add network \(IP\) cameras.

_Most_ newer IP cameras support ONVIF detection, allowing us to scan your local network and automatically add them to your setup. If a camera isn’t detected you can try adding the camera by make / model as listed below. You will need to know the IP address, login and password for the IP camera.

{% hint style="info" %}
Always make sure your IP cameras are set to a static IP. If the IP camera is setup with dynamic \(DHCP\) and the IP address changes Bluecherry will not be able to connect to the IP camera.
{% endhint %}

### Adding network \(IP\) cameras via auto detection \(ONVIF - Version 3 and newer\)

Select ‘Discover IP Cameras’![\_images/add-camera.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/add-camera.png)

ONVIF supported IP cameras will be listed below. We will attempt to add the camera using default administrator passwords.

Select the camera\(s\) you wish to add then click ‘Add selected cameras’![\_images/onvif-list.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/onvif-list.png)

### Adding network \(IP\) cameras by make / model

**Select Devices from the menu**

Select ‘Add cameras’![\_images/add-camera.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/add-camera.png) ![\_images/model-list.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/model-list.png)

Tip

With the exception of cheaper \(rebranded / eBay\) cameras most manufacturers have the same RTSP path for all models. If the exact model is not shown try another model that is close.

**Devices -&gt; Add an IP cameras**![\_images/ipcamera-manual-add.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/ipcamera-manual-add.png)

The camera name is shared throughout Bluecherry, you can change this later if you decide. Add the host or IP address \(IP address is preferred\), username and password then click ‘Add camera’

Verify your camera is connected by clicking on ‘Logs’ on the left menu and look for lines similiar to:

> bc-server\[241\]: I\(2/1\(IP ADDRESS\)\): Stream started: Video: h264 \(High\), yuv420p\(tv, bt709, progressive\), 1920x1080 \[SAR 1:1 DAR 16:9\], 1/90000\(s\) 1001/60000\(c\)

If you see an error regarding ‘404’ it means the RTSP path is incorrect.

### Adding network \(IP\) cameras as generic \(RTSP / MJPEG\)

**If the previous two steps fail, you can add the camera as a ‘generic’ IP camera. You will need to know the RTSP URL \(a Google search for the model and ‘RTSP path’ will usually provide you this information\). You will also need to know the IP address, login and password for the IP camera.**![\_images/add-generic.png](https://bluecherry-apps.readthedocs.io/en/latest/_images/add-generic.png)

The camera name is shared throughout Bluecherry, you can change this later if you decide. Add the host or IP address \(IP address is preferred\), username and password then click ‘Add camera’

Verify your camera is connected by clicking on ‘Logs’ on the left menu and look for lines similiar to:

> bc-server\[241\]: I\(2/1\(IP ADDRESS\)\): Stream started: Video: h264 \(High\), yuv420p\(tv, bt709, progressive\), 1920x1080 \[SAR 1:1 DAR 16:9\], 1/90000\(s\) 1001/60000\(c\)

{% hint style="warning" %}
If you see an error regarding ‘404’ it means the RTSP path is incorrect.
{% endhint %}

