# Block Replacement Policy for Hybrid Cache

This codebase implements a **Block Replacement Policy** in a hybrid cache, aimed at enhancing the lifetime of the Non-Volatile Cache.

For detailed insights, refer to this [slide](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/Slides.pdf).

---

## Requirements

To build **MacSim**, ensure the following are in place:

1. **Operating System:**  
   Currently, only Linux distributions are supported. MacSim has been tested on:  
   - Ubuntu  
   - Redhat (TODO)

2. **Compiler:**  
   Any compiler that supports the C++0x (or C++11) standard.  
   Verified to work with:  
   - `gcc` 4.4 or higher  
   - `icc` (work in progress)  

3. **SConstruct:**  
   Install `scons` using:
   ```bash
   sudo apt-get install scons
   ```

4. **Libraries:**  
   The following libraries are required:  
   - **zlib:** Install using:
   ```bash
   sudo apt-get install zlib1g-dev
   ```
   - **Python:** Ensure Python is installed for the build process.  
     Install Python with:
   ```bash
   sudo apt-get install python
   ```

## Build Instructions  

To compile MacSim, follow these steps:  
1. Clone the repository (if not already done):
   ```bash
   git clone https://github.com/Zeekersky/Block-Replacement-MacSIM
   cd Block-Replacement-MacSIM
   ```
2. Build the project:
   ```bash
   ./build.py
   ```
3. Verify the build:
   - If successful, the 'macsim' binary should be present inside the 'bin' directory.

## Run Instructions  

After building the project, proceed with the following steps to run MacSim:  
1. Navigate to the bin directory:
   ```bash
   cd bin
   ```
2. Ensure the following files are present in the bin directory:  
   - [params.in](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/bin/params.in)
   - [trace_file_list](https://github.com/Zeekersky/Block-Replacement-MacSIM/blob/main/bin/trace_file_list)

3. Run the MacSIM binary:
   ```bash
   ./macsim
   ``` 

For any issues or questions, feel free to reach out!
