# Block Replacement Policy for Hybrid Cache

This codebase implements a **Block Replacement Policy** in a hybrid cache to enhance the lifetime of the Non-Volatile Cache.

For a detailed discussion, refer to this [slide](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/Slides.pdf).

---

## Requirements

To build **MacSim**, the following are required:

1. **Operating System:**  
   At present, only Linux distributions are supported. MacSim has been tested on:  
   - Ubuntu  
   - Redhat (TODO)

2. **Compiler:**  
   Any compiler that supports the C++0x (or C++11) standard.  
   Verified to work with:  
   - `gcc` 4.4 or higher  
   - `icc` (work in progress)  

3. **SConstruct:**  
   Install `scons` using the following command:  
      ```bash
        sudo apt-get install scons
      ```

4. **Libraries:**  
   The following libraries are required:  
   - zlib: It can be installed using the command:
        ```bash
        sudo apt-get install zlib1g-dev
        ```
   - Python: Ensure Python is installed for the build process.  
      You can install Python using:
        ```bash
        sudo apt-get install python
        ```
5. **Build Instructions:**  
   To compile MacSim, follow these steps:  
    - Clone the repository (if not already cloned):
        ```bash
        git clone https://github.com/Zeekersky/Block-Replacement-MacSIM
        cd Block-Replacement-MacSIM
        ```
    - Build the project using the following command:
        ```bash
        ./build.py
        ```
    - Verify the build:
        
        If successful, you should see the 'macsim' binary inside the 'bin' directory.

6. **Run Instructions:**  
   After building the project, follow these steps to run MacSim:  
    - Navigate to the bin directory:
        ```bash
        cd bin
        ```
    
    - Ensure the following files are present in the bin directory.  
        - [params.in](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/bin/params.in)
        - [trace_file_list](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/bin/trace_file_list)
    
    - Run the MacSIM binary:
       ```bash
        ./macsim
       ```
