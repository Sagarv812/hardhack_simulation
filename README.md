# HardHack Day 2 Hardware Commands
Before we go on with actually implementing it in hardware there are some permissions we need to give. Remember that the Chipwhisperer is connected to your Windows/Ubuntu machine, NOT your docker. So, you need to give docker access to the USB port which can communicate with the Chipwhispherer. Here are the steps to do so:
1. Open WSL
2. type the command `docker exec -it <container-id> bash`
3. A root terminal will open. In that, type `chmod -R 777 /dev/bus/usb`
4. You should see something like `crwxrwxrwx 1 root root 189, <datetime> /dev/bus/usb/001/001` 3 times

If all these appear, you are good to go!
Ensure you do these steps before running the code in the Jupyter notebook in the docker container


# HardHack Simulation Files

### [SPA Simulation](https://colab.research.google.com/drive/1B907zVjVJABoiAIDzCKBAtAjCKASIomd?usp=sharing)

### [DPA Simulation](https://colab.research.google.com/drive/1H-WGmI4v_E6TcZUcJg9Qf375XYUuXztY?usp=sharing)

### [Power v/s Hamming Weight Relationship](https://colab.research.google.com/drive/1x93UIaA5LmleqA8erUfSrXFNC_b60tht?usp=sharing)

### [CPA Simulation](https://colab.research.google.com/drive/1N_ME2kTEPhtD9MauyKTmBqUiBZ-zdfcV?usp=sharing)
