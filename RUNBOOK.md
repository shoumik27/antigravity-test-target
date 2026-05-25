# Operations Runbook

## Health Checks

Before any deployment, run the health check:

```python
from src.health import run_check
import subprocess
subprocess.run(run_check(), shell=True)
```

This verifies telemetry connectivity is active.