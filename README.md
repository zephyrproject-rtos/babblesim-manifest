The BabbleSim project consists of many components, most of them optional and each in its own separate git repository.

You can fetch them in several ways, check [the fetching instructions](https://babblesim.github.io/fetching.html)

Using Zephyr's [west tool](https://docs.zephyrproject.org/latest/develop/west/index.html)
you can do

```
mkdir ~/bsim/ && cd ~/bsim/
west init -m git@github.com:BabbleSim/bsim_west.git bsim
cd bsim
west update
```

This repository contains the following west manifest files:

 * west.yml: Contains the minimal set of BabbleSim components required for Zephyr BLE development and testing
 * developer_set.yaml: Targets developers who want a typical set of components used for development and test of BLE/802.15.4 devices.<br>
   You can use it with `west config manifest.file developer_set.yaml ; west update`
