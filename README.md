
## Introduction
Source codes and documentation for November 2024 OPTIMA workshop:

### Environment Creation
**Download the `BCI_demo.yaml` file**: Ensure this file is in your working directory. It should contain the specifications for your environment, including the required packages.

  1) **Open the terminal**: Click on the blue New Launcer button seen in the top left of the notebook. (see below)
    
  ![image](https://github.com/user-attachments/assets/9515c8da-5459-42f4-82d8-1216432c8109)

  - **Open the terminal**: Click on the Terminal Icon seen in the bottom left of the notebook. (see below)

![image](https://github.com/user-attachments/assets/13274e5d-77f1-4490-9a1a-d55ade5ead59)

 - **Open the terminal**: This will open up your terminal in the current working directory. (see below)

![image](https://github.com/user-attachments/assets/b354b6da-a44c-42f2-8b97-a68e679cd778)

  2) **Create the environment/ OPTIMA Platform**: Once your terminal is open run the following commands to create the environment based on the `BCI_demo.yaml` file:
  
     ```bash
     mamba env update --file BCI_demo.yaml
     
     mamba init bash
     
- **Create the environment/ OPTIMA Platform**: You will now need to close the terminal and open a new teminal session as seen previously. Then type the follo the following commands to add the Kernel to the Jypeter notebook.:

    ```bash
     mamba activate BCI_demo
  
     R -e "IRkernel::installspec(name = 'BCI_demo', displayname = 'BCI_demo')"

3) **Change to the created kernel**: Open the Jupyter Notebook and click on the **kernel** tab this will open up a dropdown select **change kernel**. (see below)
  
  ![image](https://github.com/user-attachments/assets/a91fa0cd-3f6a-4bbf-aab6-9d937cfe5098)

- This will bring up a popup. select the **BCI_demo** from the drop-down.

  ![image](https://github.com/user-attachments/assets/6e529941-56ec-4267-835d-81b63732aba1)


- You should now be using the Kernel with the required libraries for the analysis.
