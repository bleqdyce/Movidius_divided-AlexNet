Movidius_divided-AlexNet
====
**This material for the users of Intel Movidius. A successful example of dividing Alexnet into two part and execute on Intel Movidius.**

There are two folders and one image: <br> 
Folder 1 - "AlexNet all" is a complete network architecture. <br>
Folder 2 - "AlexNet - two part" is a network architecture which is divided into two parts. <br>
Image 1 - "run & run_part - the same result.png" is the executing results of original-AlexNet(above) and divided-AlexNet(below) <br>
run.py, run_part.py are the Movidius inference code.

**Previous condition:** You should install intel Movidius (NC SDK) and do *make examples*. It will download several network example including AlexNet.

The graph file is Movidius's model, generated by command like *mvNCCompile -w bvlc_alexnet.caffemodel -s 12 deploy_part2.prototxt -o graph_part2*
