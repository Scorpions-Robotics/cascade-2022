# Scorpions Robotics 7672

## Cascade Classifiers for FRC Rapid React Season

This repository contains the Cascade Classifiers and a huge dataset of images for the FRC Rapid React Season. We used the 1:3 ratio of pos:neg images to train our classifiers. Feel free to open an issue if you have any questions or suggestions. Have fun!

### Commands

#### **Hoop:**

``` bash
cascade-trainer -neg n -pos p -w 55 -he 12 -s 20 -t 5 --idxSize 5000 --valSize 5000 -m ALL -npt 800 -npv 946 -nn 2365 -b 0.00007
```

#### **Ball:**

``` bash
cascade-trainer -neg n -pos p -w 40 -he 40 -s 20 -t 5 --idxSize 5000 --valSize 5000 -m ALL -npt 800 -npv 992 -nn 2480 -b 0.0001
```

``cascade-trainer`` is available at <https://pypi.org/project/cascade-trainer>
For more information about parameters, run ``cascade-trainer -h``

### Footnotes

- Accuracy may vary based on your vision processing hardware and camera settings.
- We strongly recommend training your own classifiers with the provided images and custom parameters.
- If you run into any issues, please open an issue on the issues page with your log file attached.

### License

***You can use this dataset for any purpose, but please give credit to the [original repository](https://github.com/Scorpions-Robotics/cascade-2022). See the [LICENSE file](https://github.com/Scorpions-Robotics/cascade-2022/blob/master/LICENSE) for more information.***
