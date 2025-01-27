### Step 1: Open MobaXterm on your computer, select 'Start Local Terminal' or use the SSH option, and log in to Quest using your credentials."

![Login](https://raw.githubusercontent.com/mohamedsillahkanu/FE-2023-examples/main/Login.png)

- **Note: MobaXterm is typically used to work on remote servers (e.g., through SSH)**
    - **SSH (Secure Shell) is a network protocol that allows you to securely connect to a remote computer or server over a secured network. It is widely used by system administrators, developers, and IT professionals to manage remote systems, transfer files, and execute commands.**

### Step 2: Screen that appears after you successfully log in.

![Aftter_Login](https://raw.githubusercontent.com/mohamedsillahkanu/FE-2023-examples/main/After%20login.png)

### Step 3: Load the Python module in the terminal as it is already pre-installed.

```python
module load python/3.8.4
```
- Note: idmtools require python 3.7 or higher


### **Step 4: Create and Activate a Virtual Python Environment**

1. **Create the Virtual Environment**:
   Run the following command to create a virtual environment named `test`:
   ```python
   python -m venv test
   ```
2. **Activate the Virtual Environment**:
   Activate the virtual environment using the following command:
   ```python
   source /home/wko2809/test/bin/activate
- Note: **test** is the name of the virtual environment used in this example.
- **/home/wko2809/test/** is the file path where the virtual environment is located.

### Step 5: Install emodpy-malaria

```python
pip install emodpy-malaria --ignore-installed --index-url=https://packages.idmod.org/api/pypi/pypi-production/simple
```

### Step 6: Install idmtools_platform_slurm

```python
 pip install idmtools_platform_slurm --ignore-installed --index-url=https://packages.idmod.org/api/pypi/pypi-production/simple
```

### Step 7: Update the .bashrc file to automatically activate the virtual environment by adding the following command:

```python
alias load_emodpy='source /home/wko2809/test/bin/activate'
```

### **Step 8: Create a Directory in the Projects Folder**
Run the following commands to navigate to the `/projects/b1139/` folder and create a directory named `FE_test`:

```python
cd /projects/b1139/
mkdir FE_test
```

### **Step 9: Clone the `FE-2023-examples` Repository into the `FE_test` Folder**

Clone the repository:
   ```python
   git clone https://github.com/mohamedsillahkanu/FE-2023-examples.git
   ```
                             OR
```python
git clone https://github.com/numalariamodeling/FE-2023-examples.git
```
**Note:** Ensure you are in the `FE_test` folder before cloning the repository.




