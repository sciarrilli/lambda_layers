# Steps to create a lambda layer

1. Create a python virtual environment

    ```bash
    python3 -m venv ~/faker
    ```

2. Activate the virtual environment
    
    ```bash
    source ~/faker/bin/activate
    ```

3. Install the packages desired for the layer
    
    ```bash
    pip3 install faker
    ```

4. Make a directory called python and copy the python libraries to it
    
    ```bash
    cd faker && mkdir python
    cp -Rp lib/python3.7/site-packages/ python
    ```

5. Zip the python directory
    
    ```bash
    zip -r faker.zip python
    ```
