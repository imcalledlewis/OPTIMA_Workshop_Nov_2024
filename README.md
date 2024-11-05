
## Instructions to create enviroment for 'Omics' demo 

<details>
  <summary><b>Step 1: Open the Terminal</b></summary>
  
  1) **Open the Launcher**: Click on the blue New Launcher button seen in the top left of the notebook. (see below)
    
  ![image](https://github.com/user-attachments/assets/9515c8da-5459-42f4-82d8-1216432c8109)

  2) **Open the terminal**: Click on the Terminal Icon seen in the bottom left of the notebook. (see below)

![image](https://github.com/user-attachments/assets/13274e5d-77f1-4490-9a1a-d55ade5ead59)

 3) **Terminal Tab**: This will open up your terminal in the current working directory. (see below)

![image](https://github.com/user-attachments/assets/b354b6da-a44c-42f2-8b97-a68e679cd778)
</details>
  
<details>  
  <summary><b>Step 2: Create working Directory and copy data for analysis</b></summary>
  
  1) You need to modify your terminal configuration to ensure that mamba commands work properly in future terminal sessions by running the following command.
  
    mamba init bash

  2) You will now need to close the terminal and open a new terminal session as seen previously. Now run the following commands individually to create your working directory and copy over the data:
    
    mkdir ~/work/omics_demo

    
    cd ~/work/omics_demo

    
    cp -r ~/shared/omics_demo/* ~/work/omics_demo/

</details>

<details>  
  <summary><b>Step 3: Create the environment/b></summary>

1) **Create the environment/ OPTIMA Platform**: Once your terminal is open run the following commands individually to create the environment based on the `BCI_demo.yaml` file and add the kernel to your Jupyter notebook:

       mamba env update --file BCI_demo.yaml
     
       mamba activate BCI_demo
  
       R -e "IRkernel::installspec(name = 'BCI_demo', displayname = 'BCI_demo')"
     
</details>

<details>  
  <summary><b>Step 4: Load the kernel</b></summary>
  
1) **Change to the created kernel**: Open the Jupyter Notebook and click on the **kernel** tab this will open up a dropdown select **change kernel**. (see below)
  
  ![image](https://github.com/user-attachments/assets/a91fa0cd-3f6a-4bbf-aab6-9d937cfe5098)

2) This will bring up a popup. select the **BCI_demo** from the drop-down.

  ![image](https://github.com/user-attachments/assets/6e529941-56ec-4267-835d-81b63732aba1)

3) You should now be using the Kernel with the required libraries for the analysis. You can check this by looking in the top right corner. (see below)
<img width="149" alt="image" src="https://github.com/user-attachments/assets/ae8c9829-82a0-4139-aea7-dba1d8dd9a6f">

</details>
