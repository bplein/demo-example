# demo-example
 Example of using util.sh to help script demos. util.sh is originally from the Kubernetes project early days. 

Quick way to test this: Open an Ubuntu container, install "pv" pipe viewer, and run the example:

- git clone https://github.com/bplein/demo-example.git
- cd demo-example
- docker run -v ${PWD}:/root -it ubuntu bash
- apt-get update && apt install pv
- ./example.sh