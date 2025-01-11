## venv

### create

```
python3 -m venv testenv
python3 -m pip install --upgrade pip
```

### activate

```
source /testenv/bin/activate
```

### deactivate

```
cd testenv
deactivate
```

### delete environment

```
python3 -m venv --clear path/to/env
```

### selecting kernel (jupyter notebook)

```
ipython kernel install --user --name="testenv" --display-name="name-to-display"
```

`--user`: 只對當前使用者生效

