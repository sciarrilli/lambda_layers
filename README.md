# Steps to create a lambda layer

1. Create a python virtual environment

```bash
python3 -m venv ~/faker
```

2. Activate the virtual environment
    
    source ~/faker/bin/activate

3. Install the packages desired for the layer
    
    pip3 install faker

4. Make a directory called python and copy the python libraries to it
    
    cd faker && mkdir python
    cp -Rp lib/python3.7/site-packages/ python

5. Zip the python directory
    
    zip -r faker.zip python
