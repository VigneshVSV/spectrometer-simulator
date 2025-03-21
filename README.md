# Spectrometer Simulator

An example/simulator device for spectrometer, used for illutration of web APIs.

For a web GUI, visit [here](https://thing-control-panel.hololinked.dev/#https://examples.hololinked.dev/simulations/spectrometer/resources/wot-td)
and for server only visit [here](https://examples.hololinked.dev/simulations/spectrometer/resources/wot-td).

Docker image is available, just do: <br />
`docker pull ghcr.io/vigneshvsv/spectrometer-simulator:main` <br />
for the latest image.

![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/VigneshVSV/spectrometer-simulator/docker-publish.yml?label=Build%20Docker%20Image)


Following environment variables are necessary in a docker container:
- `hostname` - hostname of the server
- `ssl_used` - optional, pythonic evaluated as a boolean (satisfies if condition for any type) if your server has SSL setup 

These variables are necessary for the forms to be correctly generated in a [Thing Description](https://www.w3.org/TR/wot-thing-description11/) otherwise the device will still work, but the forms will be wrong. These environment variables are not necessary if you are running the server outside docker. 



### To run

`pip install numpy hololinked`

Go to spectrometer.py and run the script. 
