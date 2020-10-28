**Create the virtual environment (one time activity if already created)**
Step 1
```
pip install -U pip virtualenv
```
Step 2
```
virtualenv --system-site-packages -p python ./blockchain-env
```

**Activate the virtual environment-Linux**
```
source blockchain-env/scripts/activate
```

**Activate the virtual environment-Windows 10**
```
.\blockchain-env\Scripts\activate
```

**Install all packages**
```
pip install -r requirements.txt
```

**Run the tests**
Make sure to activate the virtual environment.

```
python -m pytest backend/tests
```

**Run the application and API**

Make sure to activate the virtual environment.

```
python -m backend.app
```

**Run a peer instance**

Make sure to activate the virtual environment.
```
export PEER=True && python -m backend.app
```

**Run the frontend**
```

In the frontend directory
```
npm run start
```

**Seed the backend with data**

Make sure to activate the virtual environment.

```
export SEED_DATA=True && python -m backend.app
```

