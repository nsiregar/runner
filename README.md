# task-runner

Simple task runner for pythonista


## Usage

```python
from task_runner import Executor

def task():
    print('some task')

worker = Executor()
worker.every(1).seconds.execute(task)

# Start task runner
worker.start()

# Stop task runner
worker.stop()

# Manually run executor
while True:
    worker.run_scheduled()
```
