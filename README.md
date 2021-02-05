# demo-example
 Example of using util.sh to help script demos. util.sh is originally from the Kubernetes project early days. 

 This requires pv ("pipe viewer") and works well on Linux, and breaks on macOS due to differences in some of the commands.

Store util.sh with your scripting, and at the beginging of your script, use:

 ```
 source util.sh
 ```

 example.sh is a short script demonstrating its use. 

Quick way to test this: Open an Ubuntu container, install "pv" pipe viewer, and run the example:

```
git clone https://github.com/bplein/demo-example.git
cd demo-example
docker run -v ${PWD}:/root -it ubuntu bash
apt-get update && apt install pv
./example.sh
```
